FROM node:16 as base

WORKDIR /app

ENV NODE_ENV=prod

COPY package.json ./
RUN npm install

COPY . .

CMD [ "npm", "run", "start" ]

FROM base as dev

ENV NODE_ENV=development

RUN npm install