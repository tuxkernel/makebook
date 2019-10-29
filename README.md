# Impress PDF pages on sheets for folding and binding

## Installation:

1. Copy makebook bash script into /usr/bin

$ sudo cp makebook /usr/bin

2. Copy makebook.1.gz into /usr/share/man/man1

$ sudo cp makebook.1.gz /usr/share/man/man1

3. For detailed makebook options, open a terminal and type:

$ man makebook

That's it.

Examples:

Command for doubleletter:

makebook -v -t folio -i original-file.pdf -o output-file.pdf

Command for Oficio paper:

makebook -v -t folio -H 216mm -w 340mm -s 0.8333 -i original-file.pdf -o output-file.pdf

Command for Letterpaper:*

makebook -v -t folio -H 8.5in -w 11in -s 0.6333 -i original-file.pdf -o output-file.pdf

*Use it under your own risk! You're warned!
