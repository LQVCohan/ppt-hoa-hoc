# Phân bón vô cơ — bản thiết kế mới

## Tệp bàn giao

- `Phan_bon_vo_co_32_slide_thiet_ke_moi.pptx`: bản chỉnh sửa, 32 slide, khổ 16:9.
- `Phan_bon_vo_co_32_slide_thiet_ke_moi.pdf`: bản xem trước được dựng trực tiếp từ PPTX bằng LibreOffice 25.2.3.2.

## Nội dung và khả năng chỉnh sửa

- Giữ nguyên chữ, số liệu, phương trình và thứ tự 32 trang nguồn. Đối chiếu bằng `beautify_inventory.py --verify`: toàn bộ chuỗi nguồn có mặt trên đúng trang, không thiếu.
- Câu 4: slide 9; câu 5: slide 10; câu 6: slide 27; câu 7: slide 30.
- Chữ và công thức được xuất thành các hộp chữ PowerPoint có thể sửa; sơ đồ và biểu tượng là hình vẽ có thể sửa. Ảnh quặng apatite được giữ dưới dạng ảnh.
- Có 521 hộp chữ chỉnh sửa được, 1 ảnh. Các dòng trong đoạn được tách thành hộp chữ và giữ trong nhóm nội dung để tránh ứng dụng tự ngắt dòng thêm.
- Có ghi chú cho đủ 32 slide, mỗi slide 2 câu ngắn.
- Không thêm số liệu hoặc thay đổi nội dung khoa học, không thêm lời dẫn nhắc SGK.

## Kiểm tra

- Python 3.12.14; cài thư viện theo requirements.txt của ppt-master vào môi trường riêng; pip check không phát hiện phụ thuộc lỗi.
- Đã đọc hướng dẫn cài đặt, SKILL.md, routing và workflow beautify-pptx. attribution_guard thành công.
- Tạo SVG theo từng trang; chạy kiểm tra sớm sau trang 5 và kiểm tra cuối: 32/32 trang đạt, 0 lỗi, 0 cảnh báo.
- Rà trực quan toàn bộ SVG trên Chromium, sửa khoảng cách đoạn trên slide 31.
- Gói PPTX được kiểm tra postflight: passed, quality_gate=passed, 32 trang, 0 nhóm cảnh báo.
- Mở PPTX bằng LibreOffice và dựng đủ 32 trang PDF. Đã sửa tình trạng ứng dụng tự xuống dòng bằng tùy chọn xuất --no-merge, rồi rà lại bản xuất.
- Đã kiểm tra chữ tiếng Việt, chỉ số hóa học, dấu cân bằng và các trang nhiều chữ. Font khai báo Arial; môi trường Linux dùng font thay thế và font ký hiệu khi dựng bản xem trước. Chưa mở trực tiếp trong Microsoft PowerPoint.
- Tệp gốc trên GitHub không thay đổi. Bản tải về và bản lưu nguồn có cùng SHA-256: b5a3ed8a648d1119cddd93271c5f9fba4da8967acd7604d05443daf60d580438.

## Công cụ

Dùng [PPT Master](https://github.com/hugohe3/ppt-master) của Hugo He, giấy phép MIT. Biểu tượng từ Tabler Icons; ảnh apatite lấy từ tệp nguồn do người dùng cung cấp.


## Tabler Icons — MIT notice

Copyright (c) 2020-2026 Paweł Kuna

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
