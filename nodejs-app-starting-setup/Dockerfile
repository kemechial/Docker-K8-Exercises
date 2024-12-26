FROM node:14

WORKDIR /app
# set the working directory

COPY package.json . 
# This is for optimization, "npm install" does not change 
# so we move it to lower layer
RUN npm install 
# by default all commands executed in the working directory

# This would copy to an app directory and would create if it did not exist
COPY . /app
# COPY . .  or COPY . ./ also works because we 
# already set the working directory /app

EXPOSE 8000 
# This EXPOSE is actually just for documentation if you 
# docker run -p it would still work without expose
CMD [ "node" , "server.js"]

