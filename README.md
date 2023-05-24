# Matrix42-EmpCrypt
Matrix42 executable and DLL to generate or decrypt password hashes (v14.2).

## How to

````
# install wine
sudo dpkg --add-architecture i386
sudo apt update
sudo apt install wine32:i386
sudo apt install wine

# optional; delete configuration dir to force config-renewal
rm -rf ~/.wine

# clone this repository
git clone https://github.com/Haxxnet/Matrix42-EmpCrypt && cd Matrix42-EmpCrypt

# create hash
# the hash will be generated and stored in the clipboard only, no printout
wine EmpCrypt.exe /SYNC "P@ssw0rd"

# decrypt Matrix42 hashes
# the password will be decrypted and stored in the clipboard only, no printout
wine EmpCrypt.exe /D /SYNC "4CC7FE0A2C9F92BA646E4F89775D8DC3F5C4CC3D1F65142565D0167E56E6929F4BBD5C6F129C8F33303E53141A6F31C1"
````
