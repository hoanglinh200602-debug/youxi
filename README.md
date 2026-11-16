# YOUXI — 词汇雨 · Pixel Vocabulary Rain

Web game học từ vựng HSK1, song ngữ Trung–Việt. **Bản này viết lại từ đầu bằng HTML/CSS/JavaScript thuần**: không cần npm, Vite, build command hay cài thư viện.

## Triển khai

1. Tạo repository GitHub mới tên `youxi`.
2. Upload trực tiếp **4 file** `index.html`, `style.css`, `app.js`, `vocab.js` vào gốc repository (không đặt trong thư mục con).
3. Trên Vercel → Add New → Project → Import repository `youxi`.
4. Framework Preset: **Other**; Root Directory: `./`; Build Command: **để trống / Override off**; Output Directory: **để trống / Override off**.
5. Deploy. Vercel phục vụ trực tiếp file `index.html`.

Có thể thử offline bằng cách mở `index.html` trong trình duyệt. Không cần máy chủ.

## Tính năng

- 15 bài và 335 mục từ (gồm từ lặp lại giữa các bài và danh từ riêng), lấy từ danh sách người dùng cung cấp.
- Nhân vật quả sồi pixel vẽ bằng canvas, đón giọt mưa bằng phím mũi tên hoặc nút chạm.
- 3 chế độ 越译汉 / 汉译越 / 混合挑战; 3 độ khó 小雨 / 中雨 / 暴雨.
- Popup hướng dẫn Trung–Việt trước khi chơi; nhập Pinyin dạng số thanh 1–5, `v` cho `ü`.
- 3 mạng, điểm, màn kết quả, tiến độ và sổ từ sai.
- Giáo viên sửa/thêm/xóa từ, bật/tắt từ, xuất/nhập JSON; lưu bằng localStorage.

## Lưu ý học thuật

Các mục từ vựng được chuyển từ danh sách do người dùng gửi. Một số Pinyin, biến điệu và các nghĩa tiếng Việt của từ chức năng có thể cần được giáo viên rà soát. Phần nhập Pinyin chấp nhận dạng số theo ngân hàng dữ liệu (có thể có khác biệt giữa cách đọc theo ngữ cảnh và dạng từ điển). Không có tài khoản hay đồng bộ giữa thiết bị.
