#Start with node base image
FROM node:17.4.0

#Metadata
LABEL maintainer="Sheryl Moser"
LABEL description="MongoDB user management webapp"
LABEL cohor="13"
LABEL animal="otter"

#Set working folder for app/current work directory in container
WORKDIR /app

#Copy files from local system current direcory to containers
#current directory
COPY . .

#Port the application will listen on
EXPOSE 3000

#Run npm install to install all supported modules in package.json file
RUN npm install

#Command to run when container starts
CMD ["npm", "start"]