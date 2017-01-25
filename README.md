# heroku-laravel

#Laravel frameworkaren instalazio eta konfigurazioa laravelen defektuzko home page bistaratzeko
 
    1 sudo add-apt-repository ppa:ondrej/php -y 
    2  sudo apt-get update -y
    3  sudo apt-get install php7.0-curl php7.0-cli php7.0-dev php7.0-gd php7.0-intl php7.0-mcrypt php7.0-json php7.0-mysql php7.0-opcache php7.0-bcmath php7.0-mbstring php7.0-soap php7.0-xml php7.0-zip -y
    4  sudo mv /etc/apache2/envvars /etc/apache2/envvars.bak 
    5  sudo apt-get remove libapache2-mod-php5 -y
    6  sudo apt-get install libapache2-mod-php7.0 -y 
    7  sudo cp /etc/apache2/envvars.bak /etc/apache2/envvars
    8   
        8.1 sudo nano /home/ubuntu/.bashrc
        8.2 fitxategiaren bukaeran hau itsatsi  --> export PATH=$PATH:/home/ubuntu/.composer/vendor/bi
    9  
        9.1 sudo nano /etc/apache2/sites-available/001-cloud9.conf 
        9.2 DocumentRoot /home/ubuntu/workspace jarri beharrean --> DocumentRoot /home/ubuntu/workspace/public
    10  composer global require "laravel/installer"
    11  composer create-project --prefer-dist laravel/laravel <project name>
    12 laravel proiektuko edukia homean kopiatu nahi badugu, .env fitxategia kopiatu dela ziurtatu behar dugu
    