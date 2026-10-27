# Golang Vietnam

Trang tạm thời cho [golangvietnam.org](https://golangvietnam.org), được viết bằng HTML và CSS thuần để xuất bản trực tiếp bằng GitHub Pages.

## Chạy tại máy

```sh
python3 -m http.server 8000
```

Mở `http://localhost:8000`.

## Triển khai

GitHub Pages xuất bản thư mục gốc của nhánh `main`. `CNAME` đặt domain chính là `golangvietnam.org`; GitHub Pages sẽ chuyển `www` về domain chính khi cả hai bản ghi DNS được cấu hình đúng.

Các bản ghi web cần thiết ở Cloudflare (chế độ **DNS only**):

- Apex A: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
- `www` CNAME: `and1truong.github.io`.

Không chỉnh các bản ghi khác chỉ để triển khai trang này. Sau khi DNS và chứng chỉ sẵn sàng, bật **Enforce HTTPS** trong GitHub Pages.
