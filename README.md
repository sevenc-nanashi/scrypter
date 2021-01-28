# scrypter
[![PyPI - Downloads](https://img.shields.io/pypi/dm/scrypter?style=flat-square)](https://pypi.org/project/scrypter)  
An encrypter.

## Example

`40387509113504109504119407395111045161094023441493410324129951111941790502111507119510108511100413295091254129950512551810841442` - Key: No key

`3184323731963185319531793127312031923242319231783126323231943176312732333194318431863222317931893127323631793187320132333196317431943168` - Key: `PyPI`


## Use with arguments

```
usage: scrypter [-h] [-e | -d | -g] [-k KEY] [text]

this script will encrypt/decrypt text.

positional arguments:
  text               Text to encrypt/decrypt.

optional arguments:
  -h, --help         show this help message and exit
  -e, --encrypt      do encrypting.
  -d, --decrypt      do decrypting.
  -g, --gui          show gui.
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
