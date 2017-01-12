# tiactl
TIA Controller - Proof of concept for now.. HOBBY PROJECT!! Be warned!
# Project Purpose - to make the installs of TIA ALOT simpler



## Create TIA Install interactively 
    tiactl init 
    Welcome to the TIA Installer
    1) Identify your oracle database

    T) TNSNAMES defined in TNSNAMES.ORA
    H) Path
    A) All (host, port, location, etc) 

    2) TSFA location
    enter the path to TSFA
    e.g. \\file01\tsfa\<ssid>

    tiactl core install 
    tiactl ext install dk-dmr
    > Loading tia-ext-dk-dmr.7.4.1.0.12123.zip 

The command above would automatically find the latet DMR software that matches the TIA version you are on. 
It would then download it, and install it on your system.

    tiactl config save
    > config file saved as tiactl-dk0dev.yaml

## Load from control file 
    tiactl load tiactl-dk0dev.yaml
    > Config loaded
    > SSID: dk0dev
    > host:...
    > tsfa...

    tiactl config install 
    > deploys the current install including 





