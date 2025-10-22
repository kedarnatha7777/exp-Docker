FROM nginx
RUN rm -rf /usr/share/nginx/hmtl/
RUN rm -rf /etc/nginx/conf.d/default.conf 
RUN rm -rf /etc/nginx/nginx.conf 
COPY expense.conf /etc/nginx/nginx.conf 
COPY *.html /usr/share/nginx/hmtl/