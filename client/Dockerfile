FROM node:10.14-alpine

RUN mkdir /app
WORKDIR /app

COPY ./package.json ./

RUN yarn install
COPY . .

RUN yarn run build

ENV HOST 0.0.0.0
ENV PORT 3000

CMD ["yarn", "run", "start"]
