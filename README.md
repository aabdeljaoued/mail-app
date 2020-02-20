### Installation prerequisite :

At least, JRE 1.7.0_51

You can check your installation by typing this command in terminal : `java -version`

These messages must appear :
```
java version "1.7.0_51"
Java(TM) SE Runtime Environment (build 1.7.0_51-b13)
Java HotSpot(TM) Client VM (build 24.51-b03, mixed mode, sharing)
```



### Configuration :

Edit the file `mail.properties`

ics.mail.authentication : true or false, use smtp server with/without authentication

ics.mail.protocol : let the protocol smtp, so don't modify this value

ics.mail.starttls : true or false, some smtp server need this value to use authentication, put true if authentication

ics.mail.host : put the host of the smtp server here

ics.mail.port : put the port of the smtp server here

ics.mail.login : put the login of the smtp server here, if authentication / let blank if no authentication

ics.mail.password : put the login of the smtp server here, if authentication / let blank if no authentication

ics.mail.notify : don't modify

ics.mail.address.generic : put the generic address mail of the sender

ics.mail.address.from : put the same address



### Use :

icsmail is an web application, using spring-boot. You have to start it :
- go into the `icsmail-1.0.0.war` directory
- edit the file `mail.properties`
- open a terminal
- go into the `icsmail-1.0.0.war` directory
- type : `java -jar icsmail-1.0.0.war --spring.config.name=mail`
- open your browser at : `http://localhost:8080`

In the case the port 8080 is `already in use` :
- type instead : `java -jar icsmail-1.0.0.war --spring.config.name=mail --server.port=18080`
- open your browser at : `http://localhost:18080`

