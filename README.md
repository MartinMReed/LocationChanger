# Usage
Each time WiFi connects to a new network, a random MAC address will be selected and the hosts file will be updated. The hosts file update is separate from the MAC address selection and not required. This can be disabled and revert back to originals when connecting to a home network by updating `$HOME_SSID` in `locationchanger`.

# Installation
1. Unzip and install [SpoofMAC](https://github.com/feross/SpoofMAC) (or follow directions at [https://github.com/feross/SpoofMAC](https://github.com/feross/SpoofMAC))
2. Verify that you can run `spoof-mac list`. You may need to add it to your `.bash_profile`
3. Verify that `$SPOOF_MAC_DIR` in `locationchanger` is pointing to the correct location of spoof-mac (needed when running the LaunchDaemon as root)
4. Update the `ProgramArguments` path in `LocationChanger.plist` to point to the final location of `locationchanger`
5. Move the `LocationChanger.plist` to `/Library/LaunchDaemons/org.hardisonbrewing.LocationChanger.plist`
6. Set the LaunchDaemon permissions: `sudo chown root:wheel /Library/LaunchDaemons/org.hardisonbrewing.LocationChanger.plist`
7. Load the LaunchDaemon: `sudo launchctl load /Library/LaunchDaemons/org.hardisonbrewing.LocationChanger.plist`

# Based On
[https://github.com/feross/SpoofMAC](https://github.com/feross/SpoofMAC)  
[http://tech.inhelsinki.nl/locationchanger](http://tech.inhelsinki.nl/locationchanger)
