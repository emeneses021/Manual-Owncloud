# Manual-Owncloud
1. primero ponemos mkdir (example)

2. despues cd example

3. ahora ponemos vagrant init ubuntu/jammy64

4. ahora seguimos con vagrant up --provider=virtualbox

5. vagrant ssh

6. sudo -s

7. apt-get install software-properties-common gnupg2 -y
add-apt-repository ppa:ondrej/php
apt-get update -y
apt-get install php7.4 php7.4-fpm php7.4-cli -y
apt install zip
sudo apt install smbclient redis-server unzip openssl rsync imagemagick
sudo apt install php7.4 php7.4-intl php7.4-mysql php7.4-mbstring \
   php7.4-imagick php7.4-igbinary php7.4-gmp php7.4-bcmath \
   php7.4-curl php7.4-gd php7.4-zip php7.4-imap php7.4-ldap \
   php7.4-bz2 php7.4-ssh2 php7.4-common php7.4-json \
   php7.4-xml php7.4-dev php7.4-apcu php7.4-redis \
   libsmbclient-dev php-pear php-phpseclib


8. sudo apt install libapache2-mod-php7.4 php7.4-mysql

9. php -v

10. apt update

11. apt upgrade

12. apt install -y apache2

13. apt install -y mysql-server

14. systemctl restart apache2

15. mysql

16. CREATE DATABASE bbdd;

17. CREATE USER 'usuario'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';

18. GRANT ALL ON bbdd.* to 'usuario'@'localhost';

19. exit

20. https://owncloud.com/download-server/ 
 
21. Mover el zip a la carpeta

22. mv /vagrant/owncloud-complete-20230906.zip /var/www/html/

23. cd /var/www/html/

24. ls

25. unzip owncloud-complete-20230906\(1\).zip

26. ls

27. cd owncloud

28. cp -R * ..

29. ls
30. cd ..

31. ll

32. ls

33. rm -r owncloud

34. rm -r owncloud-complete-20230906\(1\).zip

35. rm -r index.html

36. cd /var/www/html

37. chmod -R 775 .

38. chown -R root:www-data .

39. exit

40. logout

41. vi Vagrantfile
Quitar hashtag a...
config.vm.network "forwarded_port", guest: 80, host: 8080
config.vm.network "public_network"

42. vagrant reload

43. vagrant ssh

44. logout

45. vagrant reload

46. vagrant ssh

47. Cuando ya tenemos todo cogemos la IP y la ponemos en google y iniciamos session

