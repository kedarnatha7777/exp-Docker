FROM node:20 
EXPOSE 8081
RUN useradd expense 
RUN mkdir -p  /app/server 
RUN chown  expense:expense /app/server
WORKDIR /app/server
COPY package.json .
COPY *.js .
CMD [ "node", "index.js" ]