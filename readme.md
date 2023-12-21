# Application API REST

## Commandes

### Lancer l'application

```docker-compose up```

### Crer un utilisateur ADMIN

route : http://localhost:3000/api/register

method : POST

JSON : ```{"email": "ADMIN@ADMIN.fr", "password": "ADMIN", "role": "ADMIN"}```

Role existant : ADMIN, USER, RESTAURANT

### Application front sur le port 8080 