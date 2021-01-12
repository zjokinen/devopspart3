FROM ubuntu:16.04
RUN apt-get update && apt-get install -y curl && apt-get install -y sudo
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN sudo apt install -y nodejs
COPY . .
RUN npm install
EXPOSE 8000 8000
ENV FRONT_URL=http://localhost:5000
CMD [ "npm", "start" ]