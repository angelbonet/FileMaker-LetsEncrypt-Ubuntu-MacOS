# FileMaker-LetsEncrypt-Ubuntu-MacOS
A bash script for fetching and renewing Let's Encrypt (certbot) certificates for FileMaker Server running Linux (Ubuntu) and Mac OS


### Initial Setup Instructions:
1. Setup Ubuntu + install FMS
2. Install `certbot`
3. download `wget https://raw.githubusercontent.com/jon91/FileMaker-LetsEncrypt-Ubuntu_MacOS/main/get-ssl.sh`
4. add execution `chmod ./get-ssl.sh`
5. edit content of script `nano ./get-ssl.sh`
6. run `sudo ./get-ssl.sh`


### Renewal Setup Instructions:
1. download `wget https://raw.githubusercontent.com/jon91/FileMaker-LetsEncrypt-Ubuntu_MacOS/main/renew-cert.sh`
2. add execution `chmod ./renew-cert.sh`
3. edit content of script `nano ./renew-cert.sh` (only fms usr/pwd edit needed)
4. run `sudo ./renew-cert.sh`


### Troubleshooting
+ To avoid problems restarting FM Server service you must use...
```bash
# Stop FM service Ubuntu
sudo service fmshelper restart
```


Original Script (Mac): https://github.com/BlueFeatherGroup/FileMaker-LetsEncrypt-Mac

Modified with help from: https://the.fmsoup.org/t/use-of-free-letsencrypt-ssl-certificates-with-fms/1019/7
` --- changed serverKey path`
