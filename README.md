# passphrase_generator
[Latest Releases](https://github.com/ShadowLugia650/passphrase_generator/releases)

Because Passphrases are more secure and easier to remember


## Examples
You can always use the program with no input arguments to see the usage information..

NOTE: Don't use any of these examples as your password!

`python passgen.py 4 -p` or `.\passgen.exe 4 -p`

BeheeyemScytherOmanyteElgyem

`python passgen.py 4 -p -g 3` or `.\passgen.exe 4 -p -g 3`

TorkoalBlazikenCorphishSeedot

`python passgen.py 4 -p -c` or `.\passgen.exe 4 -p -c`

Drowz]eeBasti!odonConkeld$urrDub?wool

`python passgen.py 4 -p -c -n 256` or `.\passgen.exe 4 -p -c -n 256`

218Bunnel\by223Vanilli}sh168@Naganadel163[Impidimp

`python passgen.py 4 -c 2 -p -n 256` or `.\passgen.exe 4 -c 2 -p -n 256`

110Za_mazenta160ChAarjabug112Vi|ctreebel71Et.ernatus

`python passgen.py 4 -c -p -n 256 -u` or `.\passgen.exe 4 -c -p -n 256 -u`

33sKitt@Y242c%RAnIDOs111i[NKAY166MUd|braY


## Usage
`python passgen.py <len> [flags]` OR `.\passgen.exe <len> [flags]`
  
* len: length of passphrase to generate (in number of words)
  
* flags: optional flags to modify passphrase
  * -u: include both uppercase and lowercase characters within words, instead of just title case (technically more secure)
  * -c: include special characters within words (more secure)
  * -c X, where X is a small integer: place special characters at index X of words (less secure than -c, but more secure than without any special chars)
  * -n X, where X is an integer: include numeric values from 0 to X (more secure)
  * -p: include pokemon names (significantly more secure if you don't have a large database of words lying around)
  * -f <filename>: filename to read in words from (necessary if you don't use -p)
  * -g X, where X is a pokemon generation number: only use pokemon from generation X (not necessarily less secure...)
  
Note: you can make a file with some words and use both -f and -p to include the both pokemon db and the words in your file.

  
## Don't trust my sketchy exe?
Compile the python yourself (or, you know, just run the python with python...): 

### Requisites
- Python (3.9 recommended)
- Git (alternatively you can download passgen.py directly from here)

### Setup:
```
git clone https://github.com/ShadowLugia650/passphrase_generator
pip install pyinstaller
pip install pokebase
```

### Build:
```
cd passphrase_generator  # if you're using git
pyinstaller passgen.py --onefile --hidden-import sys --hidden-import os --hidden-import pokebase
```
The executable file should be in ./dist
  
### Check Checksum:
  
Windows:
```
certutil -hashfile .\dist\passgen.exe SHA256
```
verify the generated sum with the latest posted one. If it doesn't match, you decide who you want to trust.
  
Unix:
```
sha256sum ./dist/passgen
```
I didn't build on unix so I don't have a checksum for it
