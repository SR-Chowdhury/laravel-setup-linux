<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

# Laravel Setup on Linux [Ubuntu 20.04 lts]

## First we need to install XAMPP in Linux
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
        
        php -r "if (hash_file('sha384', 'composer-setup.php') === '756890a4488ce9024fc62c56153228907f1545c228516cbf63f885e036d37e9a59d27d63f46af1d4d07ee0f76181c7d3') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
        
        sudo​ php composer-setup.php --install-dir=/usr/local/bin --filename=composer
* for confirmation run

        composer

