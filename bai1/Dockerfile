# Sử dụng Node.js version 18 làm base image
FROM node:18

# Tạo thư mục ứng dụng trong container
WORKDIR /app

# Copy package.json và cài đặt dependencies
COPY package.json ./
RUN npm install

# Copy tất cả mã nguồn vào container
COPY . .

# Expose cổng 3000
EXPOSE 3000

# Chạy ứng dụng
CMD ["node", "index.js"]
