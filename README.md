# Instructions
Borrowed from: https://medium.com/bros/enabling-https-with-lets-encrypt-over-docker-9cad06bdb82b
All credit to those folks.  I just built my own Docker image so I know what was in it.

# Command to run
`docker run --rm -it -v "/root/letsencrypt/log:/var/log/letsencrypt" -v "/var/www/html/shared:/var/www/" -v "/etc/letsencrypt:/etc/letsencrypt" -v "/root/letsencrypt/lib:/var/lib/letsencrypt" lojzik/letsencrypt certonly --webroot --webroot-path /var/www --email EMAIL -d domain`
