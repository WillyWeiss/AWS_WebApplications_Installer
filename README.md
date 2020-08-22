

![](https://www.binadox.com/wp-content/uploads/2019/04/aws-logo.png)

# Amazon Linux 2 Web Application Installer
## What it is?
This script was developed to help Computer Science students pass the Cloud Computing (technologies) exam.
The installer will deploy the fallowing:

1)Apache as httpd

2)MySQL as madiaDB 

3)PHP 

4)phpMyAdmin 

5)WordPress

## Usage:
Just make sure that you have Amazon Linux2 Instance installed with SSH, HTTP and HTTPS enabled.

1)Connect via ssh to your server

2)Paste the command below inside Amazon Linux 2 shell:

```sh
wget --no-check-certificate 'https://docs.google.com/uc?export=download&id=1s55ijGxMAeOckWuAIKN033PRLP_xfBYs' -O AWS_installer.sh && sudo chmod +x AWS_installer.sh && sudo ./AWS_installer.sh
```

3)On the last step of the installer, you will need to setup the WordPress configuration file, which will be opened on the last step of the script. 

All you need to do is:

a)  Type i to start insert mode.

b)  Modify the database connection parameters as follows:

    
    define(‘DB_NAME’, ‘blog’);
    define(‘DB_USER’, ‘root’);
    define(‘DB_PASSWORD’, ‘YOUR_PASSWORD’);
    define(‘DB_HOST’, ‘localhost’);
    
    
c)Type :wq to write the file and quit vi



4)Open a Browser and access your blog via AWS provided address to proceed with Wordpress Installation.

