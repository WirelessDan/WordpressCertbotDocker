# WordpressCertbotDocker
This is a easy to use template for deploying Wordpress with SSL certification.

To install on your Linux server run:

"git clone https://github.com/WirelessDan/WordpressCertbotDocker"
"cd WordpressCertbotDocker"

"sudo nano docker-compose.yml"
Change the values for your registered domain and user and login. Press CTRL+X to exit and select yes to save.

"sudo docker-compose up -d"
The container will start and if there are not problems a Wordpress site will be deployed at your registered domain from your server.
