# Bash script for impressing multiple PDF pages on sheets (signatures) for folding and binding

## Requirements:

- od (8.26) 
- pdflatex (3.14159265)
- pdfinfo (0.48.0)
- pdftk (2.02)
- dc (1.3.95)
- bc (1.06.95)

od, dc and bc, can be installed throught **coreutils** package:

**$ sudo apt-get install coreutils**

## Installation:

Copy makebook bash script into /usr/bin

**$ sudo cp makebook /usr/bin**

Copy makebook.1.gz into /usr/share/man/man1

**$ sudo cp makebook.1.gz /usr/share/man/man1**

For makebook options, open a terminal and type:

**$ man makebook**

That's it.

## Examples:

For doubleletter:

**makebook -v -t folio -i original-file.pdf -o output-file.pdf**

For oficiopaper:

**makebook -v -t folio -H 216mm -w 340mm -s 0.8333 -i original-file.pdf -o output-file.pdf**

For letterpaper:*

**makebook -v -t folio -H 8.5in -w 11in -s 0.6333 -i original-file.pdf -o output-file.pdf**

*Use it under your own risk! You're warned!

### This project originally is hosted in:

https://gitlab.com/dgoodmaniii/makebook/

under **GNU General Public License v3.0.**
