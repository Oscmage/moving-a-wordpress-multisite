# How to move a wordpress multisite

1. Backup your local database and move it to the new site, I recommend using something like phpmyadmin. 
2. Make sure you have a .htaccess in the /var/www/html directory like the one below.
3. If you're running apache on your server, make sure that it's possible to rewrite (usually found at: " /etc/apache2/sites-enabled/000-default.conf" ), you can below find an example of an 000-default.conf file. The important part is: 
                "AllowOverride All"
4. Use the following for search and replacing your database with "localhost" to "your ip address" https://github.com/interconnectit/Search-Replace-DB
5. Pray to god it works.
  
