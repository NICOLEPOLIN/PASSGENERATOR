# PASSGENERATOR
#!/bin/bash

# Password Generator

 echo " This is a Password Generator "
echo "Please enter the length of the password : "
read PASS_LENGTH

for p  in $(seq1 5);
do

   openssl rand base64  48 | cut  -c1-$PASS_LENGTH

done
