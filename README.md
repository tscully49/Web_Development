# Web_Development-
Just practicing different web development things for a web class 


#### The Virtual host used for this box 
```
<VirtualHost *:80>
        # Set Server name and contact details
        ServerName humerus.cloudapp.net
        ServerAdmin tps9tb@mail.missouri.edu

        # Point apache to the following director...
        DocumentRoot /home/tscully/humerus.cloudapp.net/public_html/

        #Store access and error logs here
        ErrorLog /home/tscully/humerus.cloudapp.net/log/error.log
        CustomLog /home/tscully/humerus.cloudapp.net/log/access.log combined

        # Grant access to the DocumentRoot
        <Directory /home/tscully/humerus.cloudapp.net/public_html/>
                Require all granted
        </Directory>
        ErrorDocument 404 /err-404.html
</VirtualHost>
```
