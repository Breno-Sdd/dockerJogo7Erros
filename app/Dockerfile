FROM node:16

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

# ERRO 1: Porta exposta incorreta (deveria ser 3000)
EXPOSE 8080

# ERRO 2: Comando de inicialização incorreto (deveria ser "npm start" ou "node index.js")
CMD ["node", "app.js"]