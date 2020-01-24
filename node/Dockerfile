FROM node:latest

WORKDIR /app/hello

COPY /app/hello/package*.json .

RUN yarn install

COPY  /app/hello .

RUN yarn ssr:build

EXPOSE 8000

CMD ["yarn", "run", "ssr:start"]
