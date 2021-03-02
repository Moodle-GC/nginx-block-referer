# Nginx block by referer POC

1. clone repo `git clone https://github.com/Moodle-GC/nginx-block-referer`
2. `cd nginx-bloc-referer`
3. `docker-compose up -d`
4. go to http://localhost:8080/test.html . Expect 403
5. go to http://localhost:8080/prueba2.html . Expect 200
6. use the link to access to test.html
