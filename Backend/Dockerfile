FROM nodejs:20
RUN useradd expense 
RUN mkdir -p /app/server 
RUN chown -R expense:expense /app/server
WORKDIR /app/server
COPY  package.json .
COPY  *.js . 
RUN npm install 
CMD [ "npm","index.js" ]