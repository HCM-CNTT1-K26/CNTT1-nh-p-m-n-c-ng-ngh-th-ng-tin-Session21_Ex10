# CNTT1-nh-p-m-n-c-ng-ngh-th-ng-tin-Session21_Ex10
## Phần 1: So sánh hai phương án

| Tiêu chí | Phương án 1: Hỗ trợ Cảm tính | Phương án 2: Troubleshooting 4 Chặng |
| --- | --- | --- |
| **1. Thời gian xử lý** | Lâu, phụ thuộc vào việc Senior Dev có rảnh hay không | Nhanh, tự xử lý tại chỗ trong 5-10 phút |
| **2. Áp lực cho Senior Dev** | Cao, liên tục bị ngắt gián đoạn bởi các câu hỏi lặp lại | Tối ưu, chỉ nhận ca khó đã có Bug Report |
| **3. Năng lực KTV** | Thụ động, ngại đọc tiếng Anh, khó nâng cao tay nghề | Chủ động, tư duy phân tích tốt, nắm vững hệ thống |
| **4. Lưu trữ tri thức** | Dễ mất, tin nhắn trôi trên nhóm chat Zalo | Tập trung, tích lũy thành tài liệu Wiki nội bộ |

**Kết luận của Ban Giám đốc:** VoltCharge phải chọn **Phương án 2**. Khi mở rộng quy mô lớn, cách làm cảm tính sẽ gây điểm nghẽn nghiêm trọng vì chi phí gián đoạn dịch vụ cao (500k/giờ) và đội ngũ kỹ sư cấp cao không thể gánh nổi lượng câu hỏi lặp đi lặp lại.

---

## Phần 2: Sơ đồ Luồng Quyết Định Gỡ Lỗi

**Chặng 1: Tìm kiếm trên Google**

* **Việc cần làm:** Lọc lấy đúng mã lỗi chính, bỏ các thông tin rác. Dùng dấu ngoặc kép `" "` để tìm chính xác cụm từ lỗi và dùng `site:` để giới hạn trang web uy tín.
* **Hướng xử lý:** Nếu tìm thấy cách sửa thì làm ngay. Nếu chưa được, chuyển sang Chặng 2.

**Chặng 2: Tra cứu StackOverflow / GitHub**

* **Việc cần làm:** Đọc nhanh trong 30 giây, chọn các câu trả lời có tích xanh (Accepted) hoặc có nhiều lượt bình chọn tốt (Upvote).
* **Hướng xử lý:** Nếu đúng lỗi và sửa được thì hoàn thành. Nếu thông báo vẫn khó hiểu, chuyển sang Chặng 3.

**Chặng 3: Nhờ Trợ lý AI hỗ trợ**

* **Việc cần làm:** Viết câu hỏi theo 3 phần (Ngữ cảnh + Lỗi nguyên văn + Yêu cầu). Nhớ xóa các thông tin bảo mật như API Key trước khi gửi.
* **Hướng xử lý:** Nhờ AI dịch lỗi và đưa ra 3 bước xử lý. Nếu thử 2 cách của AI mà sau 15 phút vẫn chưa xong, chuyển sang Chặng 4.

**Chặng 4: Gửi phiếu Bug Report về IT Helpdesk**

* **Việc cần làm:** Điền đầy đủ phiếu báo lỗi gồm hiện trạng, log lỗi và các bước đã tự thử.
* **Hướng xử lý:** Chuyển ticket về cho Senior Dev xử lý chuyên sâu, đồng thời bật phương án dự phòng tại trạm.
