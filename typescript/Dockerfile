FROM node:16

WORKDIR /api

COPY package.json ./

RUN yarn install --dev --frozen-lockfile

COPY ./ ./

RUN yarn build

EXPOSE 4000

CMD ["yarn", "start"]
