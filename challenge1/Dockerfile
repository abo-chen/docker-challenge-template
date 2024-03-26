# use the official nginx image
FROM nginx:alpine

# copy the contents of the public directory to the nginx root directory
COPY public /usr/share/nginx/html

# expose port 80
EXPOSE 80

# define the command to run
CMD ["nginx", "-g", "daemon off;"]