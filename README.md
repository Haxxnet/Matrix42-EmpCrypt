# Matrix42-EmpCrypt
Matrix42 executable and DLL to decrypt password hashes.

## How to

````
# install wine
sudo apt install wine
dpkg --add-architecture i386 && apt-get update && apt-get install wine32:i386

# delete configuration dir to force config-renewal
rm -rf ~/.wine

# decrypt Matrix42 hashes
# the password will be decrypted and stored in the clipboard only, no printout
wine EmpCrypt.exe /D /SYNC "4CC7FE0A2C9F92BA646E4F89775D8DC3F5C4CC3D1F65142565D0167E56E6929F4BBD5C6F129C8F33303E53141A6F31C1"
````

