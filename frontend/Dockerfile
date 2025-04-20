# Sử dụng Node.js làm base image
FROM node:18-alpine

# Thiết lập thư mục làm việc
WORKDIR /app

# Copy package.json và cài đặt dependencies
COPY package.json ./
RUN npm install

# Copy toàn bộ source code
COPY . .

# Build ứng dụng
RUN npm run build

# Chạy ứng dụng trên cổng 3000
CMD ["npm", "start"]
