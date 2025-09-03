# WordpressCertbotDocker
https://wirelessdan.net/2025/09/03/dockerized-wordpress-with-ssl/

This is a easy to use template for deploying Wordpress with SSL certification.

To install on your Linux server run these commands (if you need to set up a server see below):

"sudo git clone https://github.com/WirelessDan/WordpressCertbotDocker"
"cd WordpressCertbotDocker"

"sudo nano docker-compose.yml"
Change the values for your registered domain and user and login. Press CTRL+X to exit and select yes to save.

"sudo docker-compose up -d"
The container will start and if there are not problems a Wordpress site will be deployed at your registered domain from your server.

To set up a cloud server with a dedicated user for your WordPress site:

1. Create a VPS on Linode or Akamai using Debian or Ubuntu. The cheapest option should be enough for a simple site. After it launches for the fist time, ssh into it using the root credentials and check for updates with:
   "apt update && apt upgrade"
2. Create a dedicated user with:
   "useradd -m -s /bin/bash YOUR_NEW_USERNAME && usermod -aG sudo YOUR_NEW_USERNAME && passwd YOUR_NEW_USERNAME" Enter your new password
3. Switch user with "su YOUR_NEW_USERNAME", then switch to that user's home directory with "cd ~" and follow the installation instructions above.
