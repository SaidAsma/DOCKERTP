# Utiliser l'image de base légère de Node.js
FROM node:lts-alpine

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier les fichiers package.json et package-lock.json dans le conteneur
COPY package*.json ./

# Installer les dépendances du serveur
RUN npm install

# Copier le reste des fichiers du serveur dans le conteneur
COPY . .

# Exposer le port utilisé par l'application (9000)
EXPOSE 9000

# Commande pour démarrer l'application
CMD ["npm", "start"]
