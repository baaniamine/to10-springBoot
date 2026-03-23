# TP10 - Spring Security

## Objectif

Ce projet suit les etapes montrees dans les images :

- configuration d'un projet Spring Boot avec `Spring Web`, `Spring Security` et `Thymeleaf`
- ajout de `Spring Boot DevTools` pour le rechargement en developpement
- creation de deux utilisateurs en memoire
- protection des routes selon les roles
- personnalisation de la page de connexion
- redirection vers `/home` apres authentification

## Demo


https://github.com/user-attachments/assets/b93fdecc-411d-4346-aca7-8f090b74f4df



## URLs utiles

- `http://localhost:8080/login`
- `http://localhost:8080/home`
- `http://localhost:8080/user/dashboard`
- `http://localhost:8080/admin/dashboard`
- `http://localhost:8080/logout`

## Structure

```text
tp10/
|- pom.xml
|- mvnw
|- mvnw.cmd
|- src/
|  |- main/
|  |  |- java/ma/fstg/security/
|  |  |  |- Tp10Application.java
|  |  |  |- config/SecurityConfig.java
|  |  |  `- web/AuthController.java
|  |  `- resources/
|  |     |- application.properties
|  |     `- templates/
|  |        |- login.html
|  |        |- home.html
|  |        |- admin-dashboard.html
|  |        `- user-dashboard.html
|  `- test/java/ma/fstg/security/Tp10ApplicationTests.java
`- README.md
```

