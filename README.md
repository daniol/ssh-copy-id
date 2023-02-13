# Powershell ssh-copy-id
Powershell script duplicating ssh-copy-id behaviour in Windows.

## Dependencies
It depends on **[plink.exe](http://the.earth.li/~sgtatham/putty/latest/x86/plink.exe)**. Download and place it on the same folder as the script.

## Usage:
 - Default (public key file named `id_rsa.pub`): `.\ssh-copy-id.ps1 user@example.com password`
 - Specify public key file: `.\ssh-copy-id.ps1 -i idtest.pub user@example.com password`
 - Port other than 22: `.\ssh-copy-id.ps1 -P 1234 user@example.com password`

## Desired Features
Pull requests are welcome for the following functionalities:
1. Default mode: prompt for key, host/port and password
2. Check .authorized_keys to see if the key already exists

## Credits
Original work from [VijayS1](https://github.com/VijayS1/Scripts/tree/master/ssh-copy-id).
