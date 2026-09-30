FROM nginxinc/nginx-unprivileged:stable-alpine

COPY --chown=nginx:nginx index.html styles.css script.js /usr/share/nginx/html/

EXPOSE 8080