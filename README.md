# FileMaker-LetsEncrypt-Ubuntu-MacOS
A bash script for fetching and renewing Let's Encrypt (certbot) certificates for FileMaker Server running Linux (Ubuntu) and Mac OS


### Initial Setup Instructions:
1. Setup Ubuntu + install FMS
2. Install `Homebrew` only on MacOS
3. Install `certbot`
4. Download `wget https://raw.githubusercontent.com/jon91/FileMaker-LetsEncrypt-Ubuntu-MacOS/main/get-ssl_Ubuntu.sh` on Ubuntu 
5. Download `wget https://raw.githubusercontent.com/jon91/FileMaker-LetsEncrypt-Ubuntu-MacOS/main/get-ssl_Mac.sh` on Mac
6. add execution `chmod ./get-ssl.sh`
7. edit content of script `nano ./get-ssl.sh`
8. run `sudo ./get-ssl.sh`


### Renewal Setup Instructions:
1. Download `wget https://raw.githubusercontent.com/jon91/FileMaker-LetsEncrypt-Ubuntu-MacOS/main/renew-cert.sh` on Ubuntu
2. Download `wget https://raw.githubusercontent.com/jon91/FileMaker-LetsEncrypt-Ubuntu-MacOS/main/renew-cert_Mac.sh` on Mac 
3. add execution `chmod ./renew-cert.sh`
4. edit content of script `nano ./renew-cert.sh` (only fms usr/pwd edit needed)
5. run `sudo ./renew-cert.sh`


Original Script (Mac): https://github.com/BlueFeatherGroup/FileMaker-LetsEncrypt-Mac

Modified with help from: https://the.fmsoup.org/t/use-of-free-letsencrypt-ssl-certificates-with-fms/1019/7
` --- changed serverKey path`

Modified from https://github.com/jon91/FileMaker-LetsEncrypt-CentOS-7
` --- Adapted for Ubuntu and MacOS`
