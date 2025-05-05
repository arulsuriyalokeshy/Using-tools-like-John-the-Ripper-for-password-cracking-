# Using-tools-like-John-the-Ripper-for-password-cracking
## AIM:
To crack password hashes using John the Ripper in Kali Linux.

## DESIGN STEPS:
### Step 1:
Install John the Ripper using the command:

### Step 2:
Prepare the password hash file (e.g., using unshadow for Linux password and shadow files).


### Step 3:
Use John the Ripper to crack the hashes:

## PROGRAM:

## Install the John Ripper
```
sudo apt install john
```
## Create a Password-Protected ZIP File Archive a normal file (secret.txt) into a password-protected ZIP file
```
zip --password 123abc secret.txt.zip secret.txt
``` 
## Extract the Hash from the ZIP File
```
zip2john secret.txt.zip > zip_hash.txt
```
## Crack the ZIP Password using John
```
john --format=zip zip_hash.txt
```
## Show the Cracked Password
```
john --show zip_hash.txt
```
## OUTPUT:
Cracked Passwords from Hash File
## Create a password protected zip file
![image](https://github.com/user-attachments/assets/462e2d2a-44a6-4d47-bb0d-5d0b766aa48e)

## EXTRACT THE HASH FROM THE ZIP FILE
![image](https://github.com/user-attachments/assets/cc5c77c4-052f-4d1f-93ae-33569303b0e9)

## CRACK THE ZIP PASSWORD USING JOHN
![image](https://github.com/user-attachments/assets/bff3f810-b2d4-47d8-b570-2bea69325713)

![image](https://github.com/user-attachments/assets/f59ea89f-dcc6-4b62-8467-345411eaf344)

## SHOW THE CRACKED PASSWORD
![image](https://github.com/user-attachments/assets/c18d13db-7b69-4bca-a2c6-1979360f0beb)


## RESULT:
The password hashes were successfully cracked using John the Ripper.

