FROM nginx

RUN rm /etc/nginx/conf.d/default.conf
COPY ./moodle.conf /etc/nginx/conf.d/moodle.conf

# logs on stdout
RUN ln -sf /dev/stdout /var/log/nginx/access.log \
    && ln -sf /dev/stderr /var/log/nginx/error.log
