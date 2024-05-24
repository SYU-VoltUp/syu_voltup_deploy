FROM nginx:1.19.0

COPY nginx-nossl.conf /etc/nginx/nginx.conf

COPY --from=migusdn/syu-voltup:frontend /app/build /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]