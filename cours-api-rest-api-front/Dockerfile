# Utilisation d'une image Node
FROM node:18-alpine

# répertoire de travail
WORKDIR /app/server

# Copier les fichiers de configuration
COPY package*.json .

# Installer les dépendances
RUN npm install

# Copier le reste des fichiers
COPY . .

# Exposer le port 3000 (ou le port de votre choix)
EXPOSE 3000

# Commande pour lancer le serveur
CMD ["npm", "run", "dev"]