# How to install Laravel globally in Ubuntu
===================================================================

Open your terminal using `Ctrl+Alt+T` and type the following commands

## Step 1: Install Laravel
```bash
composer global require "laravel/installer"
```

## Step 2: Add composer to path .bashrc file to access laravel globally
```bash
cd
sudo nano .bashrc
```

## Edit environment config file and add this line
```bash
export PATH="$PATH:$HOME/.config/composer/vendor/bin"
```

## Reload config path
```bash
source ~/.bashrc
```

## Step 3: Create a new Laravel application
```bash
laravel new blog
```

## Step 4: Install missing packages and their dependencies
```bash
cd blog
composer install
```

## Step 5: Test the application
```bash
php artisan serve
```
Open a web browser and visit `localhost:8000` to see the laravel welcome page

## Step 6: Stop server
Terminate php server in terminal by pressing `Ctrl+C`	

Thus you have successfully installed laravel globally.
