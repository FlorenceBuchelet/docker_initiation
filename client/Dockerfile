# De quel environnement de départ ai-je besoin ?
FROM node:lts-alpine

# De quels fichiers ai-je besoin pour mon application ?
RUN mkdir /app
WORKDIR /app
COPY package*.json ./
RUN npm i
COPY src src
COPY public public

# Quelle commande me permet de démarrer mon projet ?
CMD npm start