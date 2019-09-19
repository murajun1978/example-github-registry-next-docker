FROM node:12.10-alpine as build

WORKDIR /usr/src

COPY package.json package-lock.json ./
RUN npm install

COPY . .
RUN npm run build


FROM node:12.10-alpine

ENV NODE_ENV="production"

WORKDIR /usr/src

COPY package.json package-lock.json ./
RUN npm install

COPY --from=build /usr/src/.next ./.next

EXPOSE 3000

ENTRYPOINT "npm start"
