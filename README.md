# DataEncryptionStandard
Implementation of DES in C

Compile the c code using the below command:
gcc des.c -o des

Then use the below commands to encrypt and decrypt the text files:
ENCRYPTION:
./des -e -i plain.txt -o enc.txt -k key.txt

DECRYPTION:
./des -d -i enc.txt -o plain.txt -k key.txt


Note: Please do not change the order of the flags as the code has been implemented such that the command line arguments 
are considered in the given order.

Also, encryption and decrytpion of very large text files might give segmentation fault as the character arrays are 
defined of fixed length i.e. 1000 Bytes.
