FROM node:16-alpine

WORKDIR /frontend

COPY . .
RUN ping www.baidu.com -c  5 && echo "网络正常"
RUN yarn config set registry https://registry.npm.taobao.org -g && yarn install
 
CMD ["yarn", "start"]
