# w1
1. Khởi chạy: Cài Docker, chạy container nginx ngầm (detach), map port 8080:80.
2. Tương tác: Chui vào bash container nginx, sửa nội dung file index.html mặc định.
3. Đóng gói: Viết Dockerfile build image cho một web app đơn giản tự chọn.
Tối ưu: Áp dụng .dockerignore, base image alpine, và Multi-stage build để ép size image nhỏ nhất.
4. Dữ liệu (Volume): Chạy DB container mount Volume, xóa container chạy lại để chứng minh dữ liệu không mất.
5. Multi-container: Viết docker-compose.yml chạy đồng thời Web và DB.
6. Mạng nội bộ: Cấu hình Web gọi DB qua DNS nội bộ Docker, cấm map port DB ra máy ngoài.
7. Bảo mật: Dùng công cụ Trivy scan image, trích xuất lỗi CRITICAL/HIGH và nêu cách fix.
