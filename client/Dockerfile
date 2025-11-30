FROM node:24-alpine

WORKDIR /usr/src/app

COPY . .

RUN npm install

RUN npm install -g serve

RUN npm run build

EXPOSE 5173

CMD [ "serve", "-l", "5173" , "-s", "dist" ]

