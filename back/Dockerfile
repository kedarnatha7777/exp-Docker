FROM node:20 
EXPOSE 8081
ENV DB_HOST=mysql
RUN useradd expense 
RUN mkdir -p  /app/server 
RUN chown  expense:expense -R /app/server
WORKDIR /app/server
COPY package*.json .
COPY *.js .
RUN npm install 
CMD [ "node", "index.js" ]