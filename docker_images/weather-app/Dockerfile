# Create an image for the weather-app
# The repository for the weather app code is here - https://github.com/linuxacademy/content-weather-app.git src

# Initializes a new build stage and sets the Base Image
FROM node
# Adds metadata to the image. This example uses abitrary metada - it can be
# anything
LABEL org.label-schema.version=v1.1
# Will execute any commands in a new layer. Bash comands
RUN mkdir -p /var/node
# Copies new files, directories or remote file URLs from <src> and adds them to
# the filesystem of the image at the path <dest>. Also, check COPY command
ADD src/ /var/node
# Sets the working directory for any RUN, CMD, ENTRYPOINT, COPY and ADD
# instructions that follow it in the Dockerfile
WORKDIR /var/node
# Will execute any commands in a new layer
RUN npm install
# Informs Docker that the container listens to the specified network ports at
# runtime
EXPOSE 3000
# Provides a default for an executing containe. There can only be one CMD
# instruction in a Dockerfile
CMD ./bin/www

