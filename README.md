# TP10 - Spring Security

## Objectif

Ce projet suit les etapes montrees dans les images :

- configuration d'un projet Spring Boot avec `Spring Web`, `Spring Security` et `Thymeleaf`
- ajout de `Spring Boot DevTools` pour le rechargement en developpement
- creation de deux utilisateurs en memoire
- protection des routes selon les roles
- personnalisation de la page de connexion
- redirection vers `/home` apres authentification

## Comptes de test

- `user / 1111` : acces a `/home` puis a `/user/dashboard`
- `admin / 1234` : acces a `/home`, `/user/dashboard` et `/admin/dashboard`

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

## Bonnes pratiques

- En production, il faut encoder les mots de passe avec `BCryptPasswordEncoder`.
- Il vaut mieux eviter de coder les roles en dur dans une vraie application.
- Les regles de securite doivent rester centralisees dans une configuration dediee.

## Important

Spring Boot `3.3.x` demande Java `17` ou plus. Si la machine utilise encore Java 8, il faut installer un JDK 17+ avant de lancer l'application.
