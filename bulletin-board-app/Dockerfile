
FROM node:20


WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .

EXPOSE 8080
CMD [ "npm", "start" ]

HEALTHCHECK --interval=5s CMD curl --fail http://localhost:8080 || exit 1  