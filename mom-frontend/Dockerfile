FROM node:12.18-alpine
RUN yarn global add @quasar/cli
#ENV NODE_ENV=production
WORKDIR /usr/src/app
COPY ["package.json", "package-lock.json*", "npm-shrinkwrap.json*", "./"]
#RUN npm install --production --silent && mv node_modules ../
RUN yarn
COPY . .
EXPOSE 8080
CMD ["quasar", "dev", "-m", "pwa"]
