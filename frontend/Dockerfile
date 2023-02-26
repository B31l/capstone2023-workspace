FROM node:18.14.2

WORKDIR /code

# COPY package.json ./
# COPY package-lock.json ./
COPY . .
RUN npm install
RUN npm run build
# RUN npm run prune --production

EXPOSE 5000
ENV HOST=0.0.0.0

CMD ["npm", "start"]