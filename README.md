# scrypter
An encrypter.

## Use with arguments

```
usage: scrypter [-h] [-e | -d] [-k KEY] [text]

this script will encrypt/decrypt text.

positional arguments:
  text               Text to encrypt/decrypt.

optional arguments:
  -h, --help         show this help message and exit
  -e, --encrypt      do encrypting.
  -d, --decrypt      do decrypting.
  -k KEY, --key KEY  key for encrypting/decrypting.
```

## Use on script
```python
>>> import scrypter
>>> scrypter.encrypt("Hello, Python!")
'4017350610750811650110951610541242416264058551012150111751110351310850911941033'
>>> scrypter.encrypt("Good morning, Python!", "Python")
'315132323227320431433219319132353226320932213213312431533196322532273214319132313149'
>>> scrypter.decrypt('4017350610750811650110951610541242416264058551012150111751110351310850911941033')
'Hello, Python!'
>>> scrypter.decrypt('315132323227320431433219319132353226320932213213312431533196322532273214319132313149',
...                  "Python")
'Good morning, Python!'
```