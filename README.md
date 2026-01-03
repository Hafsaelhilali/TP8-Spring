Description
Ce projet est une application RESTful développée avec Spring Boot pour gérer les comptes bancaires. Il permet de créer, lire, mettre à jour et supprimer des comptes en utilisant JSON et XML comme format d’échange.

Fonctionnalités
Créer un compte : POST /banque/comptes

Lire un compte : GET /banque/comptes/{id}

Mettre à jour un compte : PUT /banque/comptes/{id}

Supprimer un compte : DELETE /banque/comptes/{id}

Support pour JSON et XML

Validation des données

Retour d’un code HTTP approprié pour chaque opération (200 OK, 201 Created, 204 No Content, 404 Not Found…)

Structure du projet

<img width="325" height="345" alt="image" src="https://github.com/user-attachments/assets/c83dfa1a-d3bf-4f49-b7a5-39ecc44b6fc7" />
Dépendances principales (pom.xml)
org.springframework.boot spring-boot-starter-web
<!-- Spring Data JPA pour persistance -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>

<!-- H2 Database (en mémoire) -->
<dependency>
    <groupId>com.h2database</groupId>
    <artifactId>h2</artifactId>
    <scope>runtime</scope>
</dependency>

<!-- Jackson XML pour supporter XML -->
<dependency>
    <groupId>com.fasterxml.jackson.dataformat</groupId>
    <artifactId>jackson-dataformat-xml</artifactId>
</dependency>

<!-- Validation -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>

<!-- Tests -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-test</artifactId>
    <scope>test</scope>
</dependency>
Lancer l’application
Cloner le projet

Ouvrir dans IntelliJ IDEA ou Eclipse

Lancer la classe BanqueApplication.java

L’API sera disponible sur : http://localhost:8082/banque/comptes
<img width="1169" height="394" alt="image" src="https://github.com/user-attachments/assets/7c68ca84-9a67-4d35-ae6d-f6843ad12c8e" />
<img width="1434" height="621" alt="image" src="https://github.com/user-attachments/assets/799eb9d8-2002-4500-8450-4b9b280e12fa" />
<img width="1164" height="426" alt="image" src="https://github.com/user-attachments/assets/09dfc1e8-a2f0-47fb-8eeb-6a5e0712957c" />
<img width="1009" height="679" alt="image" src="https://github.com/user-attachments/assets/e8d4d6dc-9d73-4ab0-be43-3202d907961a" />



