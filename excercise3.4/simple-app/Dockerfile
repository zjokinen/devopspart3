FROM node:latest
COPY . .
EXPOSE 3000:3000
RUN useradd -m app
USER app
cmd [ "node", "app.js" ]
