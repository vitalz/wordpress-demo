# WordPress demo
Try WordPress easy with no affect and disaster to your system like new complicated services installed. Need only Docker on a local machine.

### Start services
```
docker-compose up -d db wp
```
#### First start
Open browser to register admin account:
```
http://127.0.0.1:8080/wp-admin
```
and create your admin account.  
<sup>(to fill in email field you can use a fake email at *example.org* domain; for example: iam@example.org)</sup>  
### Log in
```
http://127.0.0.1:8080/wp-login.php
```
### Make your first posts and view them.
Admin panel is at:
```
http://127.0.0.1:8080/wp-admin/
```  
Some comments:  
- Published blog is available via `http://127.0.0.1:8080`  
- Files uploaded for posts are stored on */var/www/html* path on WordPress server: there is an attached volume *blog* in docker-compose.  

### Clean up
Remove these external volumes *db* and *blog* on your docker system. Start from scratch.
