# wp-increase-upload-limit
```bash
sudo sed -i.bak -e 's/^upload_max_filesize.*/upload_max_filesize = 512M/g' /etc/php/*/apache2/php.ini;\ 
sudo sed -i.bak -e 's/^post_max_size.*/post_max_size = 512M/g' /etc/php/*/apache2/php.ini;\ 
sudo sed -i.bak -e 's/^max_execution_time.*/max_execution_time = 300/g' /etc/php/*/apache2/php.ini;\ 
sudo sed -i.bak -e 's/^max_input_time.*/max_input_time = 300/g' /etc/php/*/apache2/php.ini;\ 
sudo service apache2 restart
```
