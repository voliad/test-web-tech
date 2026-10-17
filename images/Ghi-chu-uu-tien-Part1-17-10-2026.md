# Sửa các ưu tiên Part 1 — 17/10/2026

- Cả bốn trang: bỏ aria-label cố định trên summary mobile và aria-hidden trên chữ Menu/Close. Giữ aria-hidden trên ba gạch trang trí; CSS display:none ẩn chữ không thuộc trạng thái hiện tại.
- Home: thêm aria-hidden=true vào ba khối slider-arrow. Các radio có tên Show image N of 3 và chấm điều khiển vẫn được giữ.
- Footer bốn trang: thêm link live https://voliad.github.io/test-web-tech/.
- Thêm README.md: mô tả dự án, link live, hai repository, Jira, phân công, hướng dẫn chạy, cấu trúc, phạm vi Part 1 và các giới hạn thực tế.
- Bản local chỉ có styles.css. PR #1 xóa style.css cũ khỏi repo sau khi kiểm tra bốn HTML không tham chiếu file đó; giữ nguyên styles.css đang dùng trong repo.

## Kiểm tra

- Cây accessibility Chromium: summary có tên Menu khi đóng, Close khi mở ở cả bốn trang.
- Slider: đủ ba radio có tên, không còn glyph ‹/› trong cây accessibility; ArrowRight chọn slide 2, click mũi tên tiếp chuyển slide 3.
- Bốn trang ở 1280 và 320 px không tràn ngang; mỗi footer có một link live.
- W3C: cả bản local và bộ file dành cho PR đều 0 lỗi HTML/CSS. Jobs còn một cảnh báo cũ về role=list.
- Giữ HTML/CSS thuần và menu desktop kiểu Phương theo yêu cầu.

## Bản GitHub

Draft PR: https://github.com/voliad/test-web-tech/pull/1
Nhánh: fix/part1-menu-slider-readme

PR chỉ áp dụng các ưu tiên này trên nội dung repo hiện tại; không ghi đè styles.css của repo và không gộp các thay đổi form live-region chưa upload ở lượt trước. Bản ZIP local tiếp tục giữ các sửa live-region đã được duyệt trước đó. Nếu muốn đồng bộ toàn bộ bản local mới nhất, cần cập nhật cả styles.css và apply.html cùng nhau.

Chưa merge PR nên GitHub Pages chưa nhận thay đổi. Repo About/topics, 404, og:image và thay đổi giới hạn tuổi/tên không nằm trong nhóm ưu tiên lần này.
