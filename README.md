# HỌ VÀ TÊN: **LÂM HỮU NGHỊ**
# LỚP: **HCM_KS26_LAMHUUNGHI_CNTT1**
## 1. Bug Report Template (4 mảnh ghép)

Quy định: không điền đủ 4 mục thì chưa được hỏi. Tạo issue trên Jira, gắn tag #BUG, dán nội dung bên dưới vào mô tả.

```
Tiêu đề: [BUG] <lỗi gì> khi <làm gì> (ví dụ: [BUG] Port 3306 already in use khi chạy docker compose up)

1. Context (bối cảnh)
- Hệ điều hành và phiên bản: 
- Phiên bản Docker / công cụ liên quan: 
- Đang làm việc gì thì gặp lỗi (nhánh Git, lệnh đã chạy): 
- Lỗi xảy ra lần đầu lúc nào, trước đó có thay đổi gì không: 

2. Expected (mong đợi)
- Lẽ ra phải xảy ra: 

3. Actual (thực tế)
- Thực tế xảy ra: 
- Tần suất: luôn luôn / thỉnh thoảng

4. Log (bằng chứng)
- Dòng lỗi nguyên văn (copy chữ, không gõ lại): 
- Ảnh chụp đã khoanh vùng lỗi, đã che thông tin nhạy cảm (token, mật khẩu, email): 

Đã tra cứu (bắt buộc ghi):
- Bước 1 Google, từ khóa đã dùng: 
- Bước 2 Community (StackOverflow, GitHub Issues), link đã đọc: 
- Bước 3 AI, đã hỏi gì và kết quả: 
- Đã thử cách nào, kết quả ra sao: 
```

## 2. Quy trình 3 bước tra cứu bắt buộc

Mục tiêu: tự xử lý khoảng 80% lỗi vặt trước khi nhờ người khác. Mỗi bước nên giới hạn khoảng 10 đến 15 phút.

Bước 1, Googling. Copy nguyên dòng lỗi, bỏ phần đường dẫn riêng của máy, thêm tên công cụ và hệ điều hành. Ví dụ: "port is already allocated" docker windows. Đọc tài liệu chính thức trước (site:docs.docker.com).

Bước 2, Community Search. Tìm trên StackOverflow và GitHub Issues của chính dự án. Ưu tiên bình luận có nhiều reaction, của maintainer, khớp phiên bản và hệ điều hành, đăng gần đây. Không chạy lệnh nào chưa đọc hiểu, nhất là lệnh có sudo, rm -rf hoặc xóa dữ liệu.

Bước 3, AI Translation. Dùng AI để dịch lỗi và giải thích, không phải để tin mù quáng. Dùng prompt 3 thành phần (vai trò, bối cảnh, yêu cầu) và hỏi ngược lại: "Lệnh này làm gì, có an toàn không, nguồn nào xác nhận?". Đối chiếu kết quả với bước 2 trước khi chạy.

Nếu cả 3 bước vẫn không xong: tạo issue theo template ở mục 1, gắn tag #BUG và báo trưởng nhóm. Chỉ nhắn vào nhóm chung một dòng kèm link issue, không dán log dài hay chat lan man trong nhóm.