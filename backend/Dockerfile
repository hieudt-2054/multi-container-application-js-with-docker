FROM node:14-alpine

WORKDIR /app

RUN chown node:node /app

COPY --chown=node:node package*.json ./

USER node

RUN npm install

COPY --chown=node:node . .

EXPOSE 3000

ENV MONGODB_USERNAME goals
ENV MONGODB_PASSWORD goals2123

CMD ["npm", "start"]