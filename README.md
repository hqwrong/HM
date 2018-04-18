# HM

This is A HangMan Game implemented by Bash Script.

make hm executable and just run it.

You'll need a vocab file, which can be set in hm Script.

## Description

To play with this game. You should have a vocabulary file which is just
a plain text file with each line a word.

`hm' will pick randomly a word from this file to play with. You can query
the word definition using external dictionary program -- the default is to
use program 'dictd'--you can set yours by editing function 'hm_dict', but try to
make the query answer to be output to stdout using plain text.

Type `hm -h' to get help message.

## Note 

Only work on GNU/Linux system.

## USAGE

Play Game:
	./hm [vocab]
Get Help:
	./hm [--help|help]
Add Words to vocabulary:
	./hm [vocab] (-a | --add) WORD...
Note: vocab is for vocabulary file path. the default is ./vocab.txt

## PLAY RULES

  You have $MAX_GUESS chances to guess a word. You can query its definition
(the word in the output will be replaced by ### literally),and it will cost you
$DIC_COST chances.
  While guessing, you can type multple guesses at once,for example,you guess this
word consists 'e','a' and 'c', it's ok to type in "eac RET" at once.

while playing, some character you input has special meaning:
?    query dictionary the meaning of the word you are guessing;
:    print the candidate character for guess;
^    quit guessing this word.


# Enjoy!
