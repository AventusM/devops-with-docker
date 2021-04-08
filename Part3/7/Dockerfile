FROM node:15

WORKDIR /usr/src/app
COPY . .

RUN npm install
# Postintall script in package.json converts ts to js
CMD ["npm", "start"]