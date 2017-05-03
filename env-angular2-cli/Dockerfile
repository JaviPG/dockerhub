# Create image based on the official Node 7.9 image from dockerhub
FROM node:7.9-alpine

MAINTAINER javipg92@gmail.com



# Create a directory where our app will be placed
RUN apk update && apk upgrade && \
    apk add --no-cache bash git openssh && \
	mkdir -p /project && \
	npm install -g typescript@2.3.2 && \
	npm i -g @angular/cli@1.0.1

# Expose the port the app runs in
EXPOSE 4200

# Serve the app
CMD ["/bin/sh"]