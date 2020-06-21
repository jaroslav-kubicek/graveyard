FROM node:14-slim

EXPOSE 3000

COPY package.json .
RUN yarn install --production

COPY . .

CMD [ "yarn", "start" ]
