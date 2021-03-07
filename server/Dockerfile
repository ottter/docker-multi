FROM node:14.14.0-alpine

WORKDIR /app

# Global dependencies
RUN npm install -g npm@latest

# Local package dependencies
COPY ./package*.json ./
RUN npm install

COPY . .

CMD ["npm", "run", "start"]
