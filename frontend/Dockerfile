FROM node:12

ADD package.json /package.json

ENV NODE_PATH=/node_modules
ENV PATH=$PATH:/node_modules/.bin

# RUN yarn config set registry http://registry.npm.taobao.org/
# RUN yarn install

WORKDIR /app
ADD . /app

EXPOSE 8000
EXPOSE 35729

ENTRYPOINT ["/bin/bash", "/app/run.sh"]
CMD ["start"]
