FROM node:16
WORKDIR /app
COPY ["package.json", "package-lock.json", "./"]
COPY . .
RUN rm -rf node_modules
RUN rm -rf package-lock.json
RUN npm cache clean --force
RUN npm install -g npm@latest
CMD ["node", "app.js"]
