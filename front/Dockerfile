FROM node:10-alpine

RUN mkdir -p /app/node_modules && chown -R node:node /app

WORKDIR /app

COPY --chown=node:node . .

USER node

RUN npm install

EXPOSE 3000

CMD ["npm", "start"]