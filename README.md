# linux-server
p address: 52.33.247.117
ssh port: 2200
complete url: http://52.33.247.117

installed the following:
1. apache2
2. libapache2-mod-wsgi
4. pip
5. flask
6. psycopg2
7. postgresql
8. git
9. oauth

command/area where configuration changes are made:
1. adduser - created user 'grader'
2. visudo - grant  user 'grader' privileges
3. apt-get update, apt-get upgrade - update current applications
4. update /etc/ssh/sshd_config - update listening port of ssh to 2200, disabled remote login to root, force key authentication
5. ssh-keygen - generate keys for user 'grader'
5. ufw - update firewall to only listen to mentioned ports (2200, 80, 123)
6. dpkg-reconfigure tzdata - update timezone to UTC

configuring app with apache:
7. git - copied app to server
8. create/configure  wsgi file
9. update from sqlite to postgresql



references
https://www.digitalocean.com/community/tutorials/how-to-configure-ssh-key-based-authentication-on-a-linux-server
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-14-04
https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
http://killtheyak.com/use-postgresql-with-django-flask/
https://discussions.udacity.com/t/create-a-new-user-named-catalog-that-has-limited-permissions-to-your-catalog-application-database/46363
http://stackoverflow.com/questions/28253681/you-need-to-install-postgresql-server-dev-x-y-for-building-a-server-side-extensi
