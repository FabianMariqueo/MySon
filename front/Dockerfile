FROM node:10-alpine

RUN mkdir -p /front/node_modules && chown -R node:node /front

WORKDIR /front

COPY --chown=node:node . .

USER node

RUN npm install

EXPOSE 3000

CMD ["npm", "start"]