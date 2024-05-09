FROM node:17-alpine

WORKDIR /app
# Dot just means copy it to root

COPY package.json .

RUN npm install
# Copies the source files from current project and place it in the same directory in the container

COPY . .

EXPOSE 3000
# required for docker desktop port mapping

CMD ["npm", "start"]
# Tells docker to use "npm start" as the command to run the container