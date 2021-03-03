# Nginx block by referer POC

el archivo `default.conf.template` se sumará a la configuración de NginX de docker.

Hay 3 archivos, 
/prueba3.html se puede acceder normalmente
/playback/test.html y /playback/prueba2.html sólo se pueden acceder desde /prueba3.html


1. clone repo `git clone https://github.com/Moodle-GC/nginx-block-referer`
2. `cd nginx-bloc-referer`
3. `docker-compose up -d`
4. go to http://localhost:8080/test.html . Expect 403
5. go to http://localhost:8080/prueba2.html . Expect 200
6. use the link to access to test.html
