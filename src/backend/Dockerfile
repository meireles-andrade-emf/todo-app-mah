# 1️⃣ Image de base Node.js légère
FROM node:20-alpine

# 2️⃣ Définir le dossier de travail
WORKDIR /app

# 3️⃣ Copier package.json et package-lock.json pour installer les dépendances
COPY package*.json ./

# Installer les dépendances
RUN npm install --production

# 4️⃣ Copier tout le code backend
COPY . .

# 5️⃣ Exposer le port sur lequel ton serveur écoute
EXPOSE 3000

# 6️⃣ Démarrer le serveur Node.js
CMD ["node", "server.js"]