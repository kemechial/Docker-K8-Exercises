FROM node:12

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

ENV PORT=80

#EXPOSE 80  
EXPOSE $PORT
# VOLUME [ "/app/feedback" ] This is for anonymous volume comment out
# for using a named volume

#CMD [ "node" , "server.js"]
CMD [ "npm" ,"start"]