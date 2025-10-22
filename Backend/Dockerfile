FROM node:20
EXPOSE 8080
RUN useradd expense 
RUN mkdir -p /app/server 
RUN chown expense:expense -R /app/server
WORKDIR /app/server
COPY package.json .
COPY *.js .
RUN npm install 
CMD [ "npm","index.js" ]