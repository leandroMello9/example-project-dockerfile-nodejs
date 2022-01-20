FROM node:14.17.5
#Diretorio dos arquivos
WORKDIR /app
#Copiando os arquvios packet.json e packet.lock.json = * Informa que queremos ambos os arquivos, package.json e package-lock.json
#./ = Copia o package.json/lock para a pasta do WORKDIR /app
COPY package*.json ./
RUN yarn
##Copiando todos os outros arquivos.
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]