# Sử dụng image chính thức của Nginx từ Docker Hub
FROM nginx:alpine

# Copy cấu hình Nginx vào container
COPY nginx.conf /etc/nginx/nginx.conf

# Nếu cần, bạn có thể copy các file frontend (từ Next.js build) vào Nginx
# COPY ./nextjs_build_folder /usr/share/nginx/html

# Expose cổng 80
EXPOSE 80
