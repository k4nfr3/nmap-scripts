# nmap-scripts
repository containing some nmap scripts


download the script to the script folder "C:\Program Files (x86)\Nmap/scripts/" on Windows or /usr/share/nmap/scripts/ on some Linux

don't forget to update the db if you want the script to be registered as exploit category for example

_nmap --script-updatedb_

## CVE-2024-3400 PANOS - GloablProtect RCE

Testing ETag value if older than 13.04.2024 (ETag = PANOS creation timestamp)

_nmap --script http-panos-cve-2024-3400.nse -p 443 vpn.mycompany.com_  

More information in panos-scanner project (PR ongoing for new signatures)
