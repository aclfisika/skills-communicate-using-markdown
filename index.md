# Header for Markdown

- I have completed to create my first markdown for in index.md
  
  ![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
- I have completed to insert image into index.md

## Adding Code
``` python
def formatNumberas3DigitString(filename,basename,extension):
    # Initialize a translation table to remove non-numeric characters
    translation_table = str.maketrans('','','abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')
    # Use str.translate() with the translation table to remove non-numeric characters
    numeric_string = filename.translate(translation_table)
    # Use str.split() to split the string into a list of word
    words = numeric_string.split()
    numbers = [int(i) for i in words]
    fn = basename+"{0:0=3d}".format(numbers[0])+extension
    return fn
```
