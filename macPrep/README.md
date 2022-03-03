## Set profile pictures
```console
sudo ./profilepic.sh braingu `pwd`/braingulogo.jpg 
sudo ./profilepic.sh ripplingadmin `pwd`/ripplinglogo.png 
```

## Remove files to force create new profile on login
```console
sudo rm /private/var/db/.Apple*
Or more directly --
    sudo rm /private/var/db/.AppleDiagnosticsSetupDone
    sudo rm /private/var/db/.AppleSetupDone
```