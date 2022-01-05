# passphrase_generator
Because Passphrases are more secure and easier to remember


## Examples
You can always use the program with no input arguments to see the usage information..

```
python passgen.py 4 -p
```

BeheeyemScytherOmanyteElgyem

```
python passgen.py 4 -p -g 3
```

TorkoalBlazikenCorphishSeedot

```
python passgen.py 4 -p -c
```

Drowz]eeBasti!odonConkeld$urrDub?wool

```
python passgen.py 4 -p -c -n 256
```

218Bunnel\by223Vanilli}sh168@Naganadel163[Impidimp

```
python passgen.py 4 -c 2 -p -n 256
```

110Za_mazenta160ChAarjabug112Vi|ctreebel71Et.ernatus

```
python passgen.py 4 -c -p -n 256 -u
```

33sKitt@Y242c%RAnIDOs111i[NKAY166MUd|braY


## Usage
python passgen.py <len> [flags] OR .\passgen.exe <len> [flags]
  
* len: length of passphrase to generate
  
* flags: optional flags to modify passphrase
  
  * -u: include both uppercase and lowercase characters within words, instead of just title case (technically more secure)
  
  * -c: include special characters within words (more secure)
  
  * -c X, where X is a small integer: place special characters at index X of words (less secure than -c, but more secure than without any special chars)
  
  * -n X, where X is an integer: include numeric values from 0 to X (more secure)
  
  * -p: include pokemon names (significantly more secure if you don't have a large database of words lying around)
  
  * -f <filename>: filename to read in words from (necessary if you don't use -p)
  
  * -g X, where X is a pokemon generation number: only use pokemon from generation X (not necessarily less secure...)
  
Note: you can make a file with some words and use both -f and -p to include the both pokemon db and the words in your file.
