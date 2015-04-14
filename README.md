Sonar
============

Docker recipe for sonar customized container.
 
Run sonar image which is linked to mysql db 
```
sudo docker run -it -d --name sonar -p 9000:9000 -e SONAR_HOST=10.0.0.110 -e SONAR_USER=sonar -e SONAR_PASSWORD=123qwe -e SONAR_CONTEXT=/sonar --link sonar-mysql:sonar-mysql mbocek/sonar:server
```