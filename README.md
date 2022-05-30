# Python-SimplePasswordEncrpytion

A simple python code for password encryption using mix of uppercase, lowercase, and numbers.

I create this code because of my awareness of password security that really harmful when people use the same password for all of their account.
So I create this code so people can have their unique password for each platform that really easy to convert from normal text.
The code works by converting the first four characters into new encrypted password. You can change the numbers to match with your preference.

The code requires one of the Python library to run.
The library used is "random" library that used for one of the method in the program.
Make sure to have it installed using pip command before importing it.

This code consist of 3 methods:
1. createEncryption() used for generating encryption dictionary.
2. encrypt() used to convert normal text into encrypted password              
3. decrypt() used to convert encrypted password into normal text     

<h3>createEncryption()</h3>

The method is used for generating new encryption dictionary.
This method works by creating an encrypted text for each word that consist from the mix of one uppercase, one lowercase, and one numbers in random order.
Every word with it's representative encrypted text will be added into dict variable, so in the end every word have their encrypted text.
This dictionary will be returned as a return value for this method.

<h3>encrypt()</h3>

The method is used to convert normal text into encrypted password.
This method requires two parameters: word that will be encrypted and withpunc boolean if the password requirement need to use punctuation.
To use this method properly, the dictionary that generated before is required and placed into passdict as a dict that will be used as a encryption dictionary.
This method works by converting the first 4 characters into new encrypted password.
If the withpunc boolean is True, there will be "-" character added in the end of the ecrypted password.

<h3>decrypt()</h3>
The method is used to convert encrypted password into normal text.
This method requires one parameters, which is the encrypted password that will be decrypted
To use this method properly, the dictionary that generated before is required and placed into passdict as a dict that will be used as a encryption dictionary.
Opposite from the previous methode, this method works by getting each 3 characters from the encrypted text and match it with the key from the dictionary.
Because of the limitation, only the first 4 words will be decrypted from normal text (eg. decrypting password that used for "google" will only have "goog" as an output).
