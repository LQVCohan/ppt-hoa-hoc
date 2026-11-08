# Kiểm tra PowerPoint phân bón vô cơ — Luobo navy/teal

## Kết quả

- 32 slide, giữ nguyên số lượng và thứ tự của bản gốc.
- Đối chiếu từng đơn vị văn bản với slide nguồn sau khi bỏ khác biệt khoảng trắng/ngắt dòng: không thiếu đơn vị nào. Công thức, chỉ số, điện tích, phương trình và số liệu gốc được giữ lại; không bổ sung số liệu khoa học.
- Câu 4 ở slide 9; câu 5 ở slide 10; câu 6 ở slide 27; câu 7 ở slide 30. Giữ nguyên câu hỏi và đáp án tương ứng.
- Speaker Notes: 2 câu ngắn trên mỗi slide, không nhắc SGK.
- QA chính thức của skill: 0 ERROR, 0 WARN, 0 INFO. Đã xem ảnh render của toàn bộ 32 slide, rà công thức, dấu tiếng Việt, ngắt dòng, khoảng cách và thành phần bị thiếu.
- Văn bản, công thức, đường nối, hình học và sơ đồ là đối tượng PowerPoint chỉnh sửa được. Ảnh quặng apatite gốc và các biểu tượng Lucide là ảnh raster. Không biến cả trang thành ảnh.
- Font khai báo Arial; phân cấp chữ dùng 9 cỡ. Đã kiểm tra hiển thị qua LibreOffice và ảnh render; chưa mở trực tiếp bằng Microsoft PowerPoint trên Windows/macOS. Font thay thế và cách ngắt dòng có thể khác nhẹ giữa phần mềm.

## Thiết kế

Bảng màu navy, xanh ngọc, trắng; nền phẳng, chữ lớn, khoảng trắng thoáng. Dùng sơ đồ quy trình, phân chia theo bước, so sánh hai cột, chữ số lớn và trang chuyển phần tối màu. Ảnh khoáng sản lấy từ file gốc; minh họa cây và bao phân bằng hình học chỉnh sửa được. Không tạo ảnh AI hoặc số liệu mới.

Các trang được dựng bằng chế độ `free` của skill để chủ động bố cục và giữ toàn bộ kiến thức. Vì vậy báo cáo tự động đếm một mã layout, dù bố cục thực tế thay đổi giữa các trang.

## Quy trình và môi trường

Đã đọc hướng dẫn cài đặt, SKILL.md và các tài liệu beautify của https://github.com/zhouwei713/luobo-ppt. Cài bản 2.9.0 tại commit `5bc279e2e0729a7d13956b360c206338eb9c7c74` bằng trình cài chính thức cho Codex. Đã kiểm tra/cài thư viện, chạy self-test dựng và render hai trang thành công trước khi dựng bài.

Chạy route beautify/full: extract → plan → make_assets → build → render → qa → compare → review. Không sửa mã nguồn skill. Bộ chuyển tiếp bên ngoài chỉ chuyển đường dẫn cache vào thư mục dự án và cấu hình LibreOffice cục bộ. Không có nhà cung cấp ảnh được cấu hình nên dùng tài nguyên gốc và minh họa hình học.

File gốc không được ghi đè. LibreOffice không mở được gói nguồn ban đầu; bản sao phục vụ render được lưu lại bằng python-pptx để tạo ảnh trước. Dữ liệu đối chiếu vẫn lấy từ file gốc. Ảnh so sánh có bản trước bên trái, bản sau bên phải, đủ 32 slide theo thứ tự.

SHA-256 file gốc: `b5a3ed8a648d1119cddd93271c5f9fba4da8967acd7604d05443daf60d580438`.

## Tự đánh giá thiết kế

Điểm do người thực hiện đánh giá, không phải điểm kiểm thử tự động:

| Tiêu chí | Điểm /10 |
|---|---:|
| Thống nhất | 8.5 |
| Phân cấp thị giác | 8.5 |
| Chi tiết | 8 |
| Truyền đạt | 8 |
| Nhịp trình bày | 8 |

Giữ: bảng màu nhất quán, công thức nổi bật, sơ đồ dễ theo dõi, chuyển phần rõ.

Cần sửa trước khi bàn giao: không còn lỗi được phát hiện trong phạm vi kiểm tra này.

Có thể cải thiện thêm: một số trang nhiều kiến thức như 24 và 31 vẫn khá nhiều chữ do yêu cầu giữ nguyên nội dung và số slide. Truyền đạt là điểm hạn chế chính; khi trình bày nên dẫn từng cụm nội dung.

## Đối chiếu từng slide

| Slide | Đơn vị văn bản gốc | Đơn vị có công thức/quy trình | Thiếu | Số câu notes | Rà ảnh |
|---|---:|---:|---:|---:|---|
| 1 | 8 | 0 | 0 | 2 | Đạt |
| 2 | 7 | 0 | 0 | 2 | Đạt |
| 3 | 18 | 8 | 0 | 2 | Đạt |
| 4 | 14 | 3 | 0 | 2 | Đạt |
| 5 | 11 | 5 | 0 | 2 | Đạt |
| 6 | 18 | 9 | 0 | 2 | Đạt |
| 7 | 14 | 5 | 0 | 2 | Đạt |
| 8 | 13 | 4 | 0 | 2 | Đạt |
| 9 | 14 | 3 | 0 | 2 | Đạt |
| 10 | 14 | 2 | 0 | 2 | Đạt |
| 11 | 14 | 3 | 0 | 2 | Đạt |
| 12 | 12 | 3 | 0 | 2 | Đạt |
| 13 | 12 | 3 | 0 | 2 | Đạt |
| 14 | 10 | 4 | 0 | 2 | Đạt |
| 15 | 19 | 4 | 0 | 2 | Đạt |
| 16 | 19 | 3 | 0 | 2 | Đạt |
| 17 | 12 | 2 | 0 | 2 | Đạt |
| 18 | 14 | 6 | 0 | 2 | Đạt |
| 19 | 7 | 0 | 0 | 2 | Đạt |
| 20 | 18 | 0 | 0 | 2 | Đạt |
| 21 | 14 | 0 | 0 | 2 | Đạt |
| 22 | 14 | 1 | 0 | 2 | Đạt |
| 23 | 14 | 0 | 0 | 2 | Đạt |
| 24 | 15 | 3 | 0 | 2 | Đạt |
| 25 | 14 | 0 | 0 | 2 | Đạt |
| 26 | 14 | 0 | 0 | 2 | Đạt |
| 27 | 13 | 0 | 0 | 2 | Đạt |
| 28 | 18 | 0 | 0 | 2 | Đạt |
| 29 | 14 | 0 | 0 | 2 | Đạt |
| 30 | 16 | 0 | 0 | 2 | Đạt |
| 31 | 11 | 1 | 0 | 2 | Đạt |
| 32 | 12 | 0 | 0 | 2 | Đạt |

Các số đếm công thức/quy trình dùng để hỗ trợ đối chiếu, không phải số phương trình phản ứng riêng biệt.

Tổng: 437 đơn vị văn bản nguồn; 487 khung chữ chỉnh sửa được.

## Ghi công và giấy phép

Luobo PPT của zhouluobo; biểu tượng Lucide. Ảnh quặng giữ từ bài gốc.

```text
MIT License

Copyright (c) 2026 zhouluobo (周萝卜)

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

Icons in this folder are rasterized from Lucide (https://lucide.dev), via react-icons.

ISC License

Copyright (c) for portions of Lucide are held by Cole Bemis 2013-2022 as part of Feather (MIT). All other copyright (c) for Lucide are held by Lucide Contributors 2022.

Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.

```
