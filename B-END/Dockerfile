FROM node:20
 
WORKDIR /usr/src/app
 
RUN apt-get update && apt-get install -y --no-install-recommends  postgresql-client postgresql nano vim libaio1 
 
COPY package*.json ./
 
RUN npm install
 
COPY . .
 
EXPOSE 3005
 
CMD ["node", "Server.cjs"]