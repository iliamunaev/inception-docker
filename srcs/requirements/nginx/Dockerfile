FROM alpine:latest

# Install nginx
RUN apk update && \
    apk add --no-cache nginx

# Create a directory for NGINX runtime files
RUN mkdir -p /run/nginx

# Copy your config (optional – only if you have a custom one)
# COPY nginx.conf /etc/nginx/nginx.conf

# Expose HTTP port
EXPOSE 80

# Run nginx in foreground
CMD ["nginx", "-g", "daemon off;"]
