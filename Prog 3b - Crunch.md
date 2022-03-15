### Common Arguments

1. -t is used to specify our own patterns of characters. The symbols used to represent some group of characters are as follows,  
- , for all uppercase letters.
- @ for all lowercase letters.
- % for all numeric characters.
- ^ for all special characters.  
2. -c is used to create a file based on breaking output with respect to the number of lines that were specified.  
3. -b is used to split and create files based on the size specified.  
4. -z is used to compress the files created in compressed format, for example gzip, bzip, lzma, 7z.  
5. -i is used to generate all the possible passwords from the specified wordlist in inverted format.  

### Examples

1. crunch 3 5 -f /usr/share/crunch/charset.lst mixalpha -o file.txt
2. crunch 3 3 -t ,%% -b 1kb -o file.txt
3. crunch 5 5 -f  /usr/share/crunch/charset.lst ualpha -t A@@D@ -l a@aaa -c 100 -o file.txt
4. crunch 4 6 -p ankit is great
