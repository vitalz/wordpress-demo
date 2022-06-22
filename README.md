# WordPress demo
Try WordPress easy: need only Docker installed on local machine.

### Start services
```
docker-compose up -d db wp
```
### Open browser:
```
http://127.0.0.1:8080/wp-admin
```
and create your admin account (to fill in email field you can use a fake email at *example.org* domain; for example: user@example.org).  
##### log in again
```
http://127.0.0.1:8080/wp-login.php
```
### Make your first posts and view them.
- Admin panel is on `http://127.0.0.1:8080/wp-admin/`  
- Published blog is available via `http://127.0.0.1:8080`  
- Files uploaded for posts are stored on */var/www/html* path on WordPress server: there is an attached volume *blog* in docker-compose.
