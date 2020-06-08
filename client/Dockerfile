FROM node:alpine

ENV CI=true
WORKDIR /app
COPY package.json ./
RUN yarn install
COPY ./ ./
RUN yarn build

CMD ["yarn","start"]