# Utilisez une image officielle Node.js en tant qu'image parent
FROM node:21

# Définissez le répertoire de travail dans le conteneur sur /app
WORKDIR /usr/src/app

# Copiez package.json et package-lock.json dans /app
COPY package*.json .

# Installez les dépendances à l'aide de npm
RUN npm install

# Copiez le contenu du répertoire actuel dans le conteneur dans /app
COPY . .

# Rendez le port 4000 disponible pour le monde extérieur à ce conteneur
EXPOSE 4000

# Exécutez npm start lorsque le conteneur démarre
CMD ["npm", "run", "dev"]
