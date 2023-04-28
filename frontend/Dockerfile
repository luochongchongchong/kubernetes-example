FROM node:16-alpine

WORKDIR /frontend

COPY . .
RUN ping www.baidu.com -c  5 && echo "网络正常"
RUN curl https://cdn.npmmirror.com/css.escape/-/css.escape-1.5.1.tgz && echo "下载成功"
RUN yarn config set registry https://cdn.npmmirror.com -g && yarn install
 
CMD ["yarn", "start"]
