# CIS7-Project
Project Portfolio
Date published: 6/6/2022
Welcome to our Vignere Cryptography project! The people who worked on this project are Moises Santiago, Youssef Koreatam, and Adrian Acevado.
How-to-Use Instructions: When running the code, you will get the a message asking if you would like to encrypt or decrypt the text. You enter "1" to encrypt and "2" to decrypt and then you write the text that you wish to decrypt or encrypt.
Psuedo Code:
  This program encrypts and decrypts text using a key.

Include libraries
Use namespace std

Prototype functions

Main function(){

Print welcome message
Print  menu

Take input as an integer variable called choice
Take text as input
Take key as input

Call functions to stretch the key and convert key and text to upper case then save them in new variables: newTxt and newKey

If ( choice is 1)
	Use the encryption function(newTxt, key)
Else if (choice is 2)
	Use the decryption function(newTxt, key)

Return 0
}

keyGen function(the text, the key){
For the number of letters in the text string
	Add to the new key an uppercase version of each letter of key mod key length
Return newKey
}
txtUpr(text){
For the length of txt
	Convert evey character in it to uppercase
Return newTxt
}
encrypt( the new text, the new key){
Print the txt then encrypt it by adding the value of each char of the key and txt then mod 26 then save it to a character called num
Then add 65 to num then add this char to encrypted
Then repeat that process for every character in the text
Then print the encrypted message
}
decrypt(the text, key){
Print the new txt and that it was decrypted then decrypt by subtracting key character from text character add 26 then mod 26, save it to a char called num
Add num to 65 then add the result to a string called decrypted
Then repeat that process for every character in the text
Then print the denrypted message
}
