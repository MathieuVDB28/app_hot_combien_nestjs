# Utilisez une image officielle Node.js en tant qu'image parent
FROM node:14-alpine

# Définissez le répertoire de travail dans le conteneur sur /app
WORKDIR /app

# Copiez package.json et package-lock.json dans /app
COPY package*.json ./

# Installez les dépendances à l'aide de npm
RUN npm install

# Copiez le contenu du répertoire actuel dans le conteneur dans /app
COPY . .

# Rendez le port 3000 disponible pour le monde extérieur à ce conteneur
EXPOSE 3000

# Exécutez npm start lorsque le conteneur démarre
CMD ["npm", "run", "start:dev"]
