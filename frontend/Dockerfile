FROM node:16-alpine

WORKDIR /frontend

COPY . .

RUN yarn config set registry https://registry.npm.taobao.org -g && yarn install
 
CMD ["yarn", "start"]
