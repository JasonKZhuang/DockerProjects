# download basic node runtime package from docker hub
FROM node:16

# setting a working director, so all command will be executed in this folder
WORKDIR /app

# copy the package dependence file first, docker build image will use cache due to the layer archiecture of image
COPY package.json /app

# run npm install command in the working directory
RUN npm install

# copy all file in current host folder to image directory /app
COPY . /app

# The EXPOSE instruction indicates the ports on which a container listens for connections. 
EXPOSE 80

# run command when the container started based on the image
CMD [ "node", "server.js" ]

