### Modes

#### John the ripper Single crack mode
john --single --format=raw-sha1 file.txt

#### John the ripper Wordlist crack mode
john --wordlist=/usr/share/john/password.lst --format=raw-sha1 file.txt

#### Incremental Mode
john --incremental crack.txt

  
### Extras
  
**View all formats**  
To view all encryption formats that John the ripper uses -  
john --list=formats  

**Cracking multiple files**  
john -form=raw-md5 file1.txt file2.txt

**Creating a new user**  
sudo useradd -r <name>  
sudo passwrd <name>
