FROM node:lts-alpine

ENV LANG C.UTF-8
ENV TZ Asia/Tokyo

WORKDIR /app

ENV PATH /app/node/node_modules/.bin:$PATH

RUN yarn global add @vue/cli@4.5.13

COPY app/node/skill-creator/package.json .
COPY app/node/skill-creator/package-lock.json .

CMD ["yarn",  "serve"]