<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

# Laravel Setup on Linux [Ubuntu 20.04 lts]

## First we need to install XAMPP on Linux
* Download XAMPP (https://www.apachefriends.org/index.html)
* Go to download folders

        cd Downloads/
        
 * Type sudo chmod +x xampp-linux-.........-installer
 
        sudo chmod +x xampp-linux-x64-8.0.3-0-installer
        sudo ./xampp-linux-x64-8.0.3-0-installer
## Now Download Composer
* First go to home directory [back from Downloads using `cd ..`]
* Go to (https://getcomposer.org/download/)
* Then run

        php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" 
-- If you get an error than install php-7.4.3 cli `sudo​ apt-get install php-cli`
        
        php -r "if (hash_file('sha384', 'composer-setup.php') === '756890a4488ce9024fc62c56153228907f1545c228516cbf63f885e036d37e9a59d27d63f46af1d4d07ee0f76181c7d3') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
        
        sudo​ php composer-setup.php --install-dir=/usr/local/bin --filename=composer
* for confirmation run

        composer
## Now install PHP extensions
* run in terminal

        sudo​ apt-get install php-zip
        sudo​ apt install php-mbstring
        sudo​ apt install php-xml
        sudo​ apt install php-bcmath
        
## Create Laravel Project
* Now go to the directory where you want to create your project like `cd Documents/`
* Go to laravel documentation (https://laravel.com/docs/8.x#installation-via-composer)

* **Installation Via Composer**

        composer create-project laravel/laravel example-app
_You may got an error like Http://repo.packagist.org could not be fully loaded, package information was loaded from the local cache and may be out of date_
**Fix this error**
* Clear the cache 

        composer clear-cache   
OR

    composer config -g repo.packagist composer https://packagist.org
    
**After fixing issue**

    cd example-app

    php artisan serve


# EXPL:first_quarter_moon:RE SUPER:star2: W:last_quarter_moon:RLD 
    
