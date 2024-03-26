# use the official node image
FROM node:14

# set the working directory
WORKDIR /usr/src/app

# copy package.json and package-lock.json
COPY package*.json ./

# install dependencies
RUN npm install

# copy app files
COPY . .

# expose port 3000
EXPOSE 3000

# define environment variable
ENV PORT=3000

# define the command to run
CMD ["npm", "start"]
