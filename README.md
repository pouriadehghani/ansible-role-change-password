# Change root passowrd
This project automatically generate random password and combined with your pattern, Then you can memorize your pattern and put the random section in your password managers like lastpass.

## Getting Started
```
sudo apt install whois
pip install pexpect
```

## Vars 

`change_password_user`: username

`change_password_pattern`: passwordPattern

`change_password_random_size`: sizeOfRandomCharsForPassword


## Outputs are in passwd.csv
```
cat $PWD/passwd.csv
```

*Tested on Ubuntu/Debian
