FROM nginx:alpine
LABEL org.opencontainers.image.source=https://github.com/Qwer2333wwww/docker-study
RUN rm /etc/nginx/conf.d/default.conf
COPY default.conf /etc/nginx/conf.d/
COPY hcf.html /usr/share/nginx/html/
COPY 404.html /usr/share/nginx/html/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]