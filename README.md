# Usage
Each time WiFi connects to a new network, a random MAC address will be selected and the hosts file will be updated. The hosts file update is separate from the MAC address selection and not required. This can be disabled and revert back to originals when connecting to a home network by updating `$HOME_SSID` in `locationchanger`.

# Installation
1. Unzip and install [SpoofMAC](https://github.com/feross/SpoofMAC)
2. Verify that you can run `spoof-mac list`. You may need to add it to your `.bash_profile`.
3. Update the `ProgramArguments` path in `LocationChanger.plist` to point to the final location of `locationchanger`
4. Copy/Move `LocationChanger.plist` to `/Library/LaunchDaemons/org.hardisonbrewing.LocationChanger.plist`
5. Set the PLIST permissions `sudo chown root:wheel /Library/LaunchDaemons/org.hardisonbrewing.LocationChanger.plist`
6. Load the PLIST `sudo launchctl load /Library/LaunchDaemons/org.hardisonbrewing.LocationChanger.plist`

# Originals
[https://github.com/feross/SpoofMAC](https://github.com/feross/SpoofMAC)  
[http://tech.inhelsinki.nl/locationchanger](http://tech.inhelsinki.nl/locationchanger)
