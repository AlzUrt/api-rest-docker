# Utilisation d'une image Node
FROM node:18-alpine AS build

# répertoire de travail
WORKDIR /app/back

# Copier les fichiers de configuration
COPY package*.json .
RUN npm install


COPY . .

# Installer les dépendances
RUN npm run build

FROM nginx:alpine

# Copier le reste des fichiers
COPY --from=build /app/back/dist /usr/share/nginx/html

# Exposer le port 80 (ou le port de votre choix)
EXPOSE 80

# Commande pour lancer le back
CMD ["nginx", "-g", "daemon off;"]