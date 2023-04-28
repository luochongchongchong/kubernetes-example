FROM node:16-alpine

WORKDIR /frontend

COPY . .
RUN ping www.baidu.com -c  5 && echo "网络正常"
RUN wget https://registry.npmmirror.com/css.escape/-/css.escape-1.5.1.tgz && echo "下载成功"
RUN yarn config set ignore -engines true && yarn config set registry https://registry.npm.taobao.org -g && yarn install
 
CMD ["yarn", "start"]
