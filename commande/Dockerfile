# Utilise l'image officielle Node.js 16 comme image parente
FROM node:16-alpine
# Définit le répertoire de travail dans le conteneur sur /app
WORKDIR /app
# Copie les fichiers package.json et package-lock.json dans le conteneur
COPY package*.json ./
# Exécute npm install pour installer les dépendances dans le conteneur
RUN npm install
# Copie le reste des fichiers de l'application dans le conteneur
COPY . .
# Démarre le serveur en exécutant la commande node index.js
CMD ["node", "index.js"]