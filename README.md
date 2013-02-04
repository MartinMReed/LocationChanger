# Usage
Each time WiFi reconnects, a new random MAC address will be selected. This can be disabled when connecting to a home network by updating `$HOME_SSID` in `locationchanger`.

# Installation
Unzip and install [SpoofMAC](https://github.com/feross/SpoofMAC)  
Update the `ProgramArguments` path in `LocationChanger.plist` to point to the final location of `locationchanger`  
Install `LocationChanger.plist` to `/Library/LaunchDaemons/org.hardisonbrewing.LocationChanger.plist`  

# Originals
[https://github.com/feross/SpoofMAC](https://github.com/feross/SpoofMAC)  
[http://tech.inhelsinki.nl/locationchanger](http://tech.inhelsinki.nl/locationchanger)
