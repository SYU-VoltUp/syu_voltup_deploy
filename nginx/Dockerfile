FROM nginx:1.19.0

COPY ./nginx.conf /etc/nginx/nginx.conf

COPY --from=migusdn/syu-voltup:frontend /app/build /usr/share/nginx/html

EXPOSE 80
EXPOSE 443

CMD ["nginx", "-g", "daemon off;"]