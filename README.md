![alt text][logo]

[logo]:https://github.com/Miku-UI/manifesto/blob/Udon_v2/img/MikuUI.png "Miku-UI Android"

# Miku-ui-build-signed-script
Script for creating a signing build environment

## Disclaimer
This script only works for password-less keys (DO NOT SET A PASSWORD) *This is due to building inline, other steps are necessary for a password*

*Works with Miku-ui TDA or Miku-ui Udon(v2) *

## How to run
1. Download the script in your root build directory and run it

`git clone https://github.com/MaloyBegonia/Miku-ui-build-signed-script-Public miku (In rom folder)`

`chmod +x create-signed-env.sh`

`./create-signed-env.sh`

2. Enter info for certificate subject line and confirm

3. Hit enter to set no password for each certificate. **Cannot set a password to build inline with this method!**

### Prep device tree (for other ROMs)
In your device tree (or common device tree) add:

`-include vendor/miku/keys/keys.mk`

Build as usual!
