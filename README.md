# Hướng dẫn sử dụng

## 1. Clone repository với submodule

Để clone repository này cùng với các submodule, bạn cần chạy lệnh sau:

```bash
git clone --recursive https://github.com/BDuong31/Baso-Spark.git
```

Nếu bạn đã clone repository mà chưa tải submodule, bạn có thể chạy các lệnh sau để cập nhật submodule:

```bash
git submodule init
git submodule update
```

Hoặc sử dụng lệnh gọn hơn:

```bash
git submodule update --init --recursive
```

## 2. Cách chạy với Docker Compose

### Bước 1: Cài đặt Docker và Docker Compose
- Đảm bảo bạn đã cài đặt Docker và Docker Compose trên máy của mình.
- [Hướng dẫn cài đặt Docker](https://docs.docker.com/get-docker/)
- [Hướng dẫn cài đặt Docker Compose](https://docs.docker.com/compose/install/)

### Bước 2: Chạy Docker Compose
Trong thư mục gốc của dự án, chạy lệnh sau để khởi động các container:

```bash
docker-compose up --build
```

### Bước 3: Truy cập ứng dụng
- Sau khi các container được khởi động thành công, bạn có thể truy cập ứng dụng thông qua địa chỉ được chỉ định (ví dụ: `http://localhost:8000`).

### Bước 4: Dừng container
Để dừng các container, bạn có thể sử dụng lệnh:

```bash
docker-compose down
```

## 3. Lưu ý
- Đảm bảo các tệp cấu hình như `.env` đã được thiết lập đúng trước khi chạy Docker Compose.
- Nếu có thay đổi trong submodule, hãy cập nhật bằng lệnh:

```bash
git submodule update --remote
```
