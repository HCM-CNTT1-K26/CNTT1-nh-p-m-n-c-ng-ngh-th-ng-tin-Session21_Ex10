# CNTT1-nh-p-m-n-c-ng-ngh-th-ng-tin-Session21_Ex10
## Phần 1: Bảng so sánh Trade-off

| Tiêu chí | Phương án 1: Hỗ trợ Cảm tính | Phương án 2: Troubleshooting 4 Chặng |
| --- | --- | --- |
| **1. Thời gian xử lý** | Lâu, phụ thuộc vào việc Senior Dev có bận hay không | Rút ngắn 80%, tự xử lý xong trong 5-10 phút |
| **2. Áp lực cho Senior Dev** | Rất cao, liên tục bị quấy rầy bởi lỗi lặp lại | Tối ưu, chỉ nhận ca khó khi đã có Bug Report |
| **3. Năng lực KTV** | Thụ động, sợ tiếng Anh, không tiến bộ | Chủ động, tư duy phân tích sắc bén |
| **4. Lưu trữ tri thức** | Mất mát, trôi tin nhắn trên nhóm Zalo | Lưu tập trung thành tài liệu Wiki nội bộ |

**Kết luận của Ban Giám đốc:**
VoltCharge bắt buộc phải chọn **Phương án 2**. Khi mở rộng lên hàng nghìn trạm, mô hình cảm tính sẽ gây sập hệ thống vì chi phí downtime quá lớn (500k/giờ) và đội ngũ kỹ sư cấp cao không thể gánh nổi lượng câu hỏi khổng lồ.

---

## Phần 2: Sơ đồ Luồng Quyết Định (Decision Flowchart)

text

[Kiosk gặp lỗi / Error Pop-up]

 └──> ⏱ Bắt đầu tính giờ (0 phút)

       │
 
       ▼

[CHẶNG 1: Googling thông minh]

 ├── Lọc từ khóa cốt lõi của lỗi.
 
 └── Dùng toán tử tìm kiếm chính xác (site:, dấu ngoặc kép).
 
       └──> [Thành công?] ➔ Xong. Nếu không ➔ Chặng 2.
       
             │
             
             ▼

[CHẶNG 2: Đọc StackOverflow / GitHub]

 ├── Lướt nhanh trong 30 giây.
 
 ├── Kiểm tra dấu tích xanh (Accepted Answer) hoặc Upvote cao.
 
       └──> [Thành công?] ➔ Xong. Nếu không ➔ Chặng 3.
       
             │
             
             ▼

[CHẶNG 3: Hỏi Trợ lý AI]

 ├── Viết Prompt chuẩn 3 phần (Context + Raw Error + Instruction).
 
 ├── Nhớ xóa bỏ thông tin nhạy cảm (API Key).
 
 └── Nhờ AI dịch lỗi và đưa ra hướng sửa.
 
       └──> [Thành công?] ➔ Xong. Nếu sau 15 phút vẫn kẹt ➔ Chặng 4.
       
             │
             
             ▼

[CHẶNG 4: Gửi Bug Report]

 ├── Điền phiếu báo lỗi chuẩn 4 bước.
 
 └── Gửi trực tiếp về phòng IT Helpdesk / Senior Dev xử lý chuyên sâu.

