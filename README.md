# Usage
Each time WiFi connects to a new network, a random MAC address will be selected and the hosts file will be updated. The hosts file update is separate from the MAC address selection and not required. This can be disabled and revert back to originals when connecting to a home network by updating `$HOME_SSID` in `locationchanger`.

# Installation
Unzip and install [SpoofMAC](https://github.com/feross/SpoofMAC)  
Update the `ProgramArguments` path in `LocationChanger.plist` to point to the final location of `locationchanger`  
Install `LocationChanger.plist` to `/Library/LaunchDaemons/org.hardisonbrewing.LocationChanger.plist`  

# Originals
[https://github.com/feross/SpoofMAC](https://github.com/feross/SpoofMAC)  
[http://tech.inhelsinki.nl/locationchanger](http://tech.inhelsinki.nl/locationchanger)
