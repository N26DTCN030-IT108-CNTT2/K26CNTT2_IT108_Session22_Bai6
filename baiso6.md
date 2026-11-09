# [D26TXCN02-N]_IT108_[Session 22]_[Bài 6]
**Bài tập: Ứng dụng AI trong khắc phục lỗi Git Permission Denied**

**Thông tin sinh viên:**
- **Họ và tên:** Lê Hồ Thanh Thảo
- **Mã sinh viên:** N26DTCN030
- **Lớp:** D26TXCN02-N
- **Môn học:** Nhập môn Công nghệ Thông tin (IT_108) 

---

## 1. Yêu cầu 1: Công thức Prompt 3 Thành phần (nhờ AI giải thích lỗi)

### 📌 Cấu trúc Prompt 3 thành phần (Role - Context - Task):
* **Bối cảnh (Context):** Tôi đang cần đẩy code lên GitHub để kịp deadline thì Terminal báo lỗi: `error: open(".git/FETCH_HEAD"): Permission denied`.
* **Vai trò (Role):** Hãy đóng vai một chuyên gia lập trình viên kiêm nhà giáo dục CNTT thân thiện.
* **Nhiệm vụ (Task):** Giải thích nguyên nhân gây ra lỗi này theo cách bình dân, dễ hiểu nhất (dùng ví dụ ẩn dụ thực tế) và đưa ra các bước khắc phục an toàn.

---

### 💬 Nội dung Prompt gửi AI:

> "Tôi đang làm bài tập và cần đẩy code lên GitHub cho kịp deadline thì Terminal báo lỗi: `error: open(".git/FETCH_HEAD"): Permission denied`. 
> 
> Bạn hãy đóng vai một đàn anh khóa trên chuyên ngành CNTT rất thân thiện, hãy giải thích giúp tôi lỗi này nghĩa là gì theo cách 'bình dân' nhất (như đang giải thích cho người mới học). Đồng thời hướng dẫn từng bước khắc phục lỗi này một cách an toàn nhất nhé!"

---

### 💡 Câu trả lời kỳ vọng từ AI (Giải thích bình dân):
> **Giải thích kiểu bình dân:** Hãy tưởng tượng thư mục `.git` giống như **cuốn sổ nhật ký** của dự án, còn file `FETCH_HEAD` là **trang giấy ghi chú** vừa được cập nhật. Bạn (tài khoản user hiện tại) đang muốn mở trang giấy đó ra để viết tiếp. Tuy nhiên, trước đó bạn từng lỡ dùng quyền "Chủ nhà / Quản lý" (Administrator / `sudo`) để mở cuốn sổ, khiến trang giấy này bị **khóa lại bằng ổ khóa của Administrator**. Bây giờ bạn dùng tài khoản người dùng thường để mở thì hệ thống báo *"Permission denied"* (Không có quyền truy cập) vì chìa khóa bạn đang cầm không khớp với ổ khóa của Administrator.

---

## 2. Yêu cầu 2: Minh họa thao tác "Run as Administrator" & Quy tắc chụp ảnh

### 🛠️ Các bước thực hiện:
1. Đóng toàn bộ Terminal / VS Code hiện tại.
2. Tìm kiếm **Git Bash** hoặc **PowerShell** trong Menu Start của Windows.
3. Nhấp chuột phải và chọn **"Run as Administrator"** (Chạy với quyền quản trị viên).
4. Điều hướng về thư mục dự án và tiến hành phân quyền lại hoặc sửa lỗi.

### 📸 Minh chứng ảnh chụp màn hình (Tuân thủ tiêu chuẩn báo cáo kỹ thuật):

![Minh họa Run as Administrator và khoanh vùng lỗi](./images/run_as_admin_error.png)

* **Quy tắc khoanh vùng & Bảo mật:**
  * 🔴 **Khoanh vùng đỏ:** Nối bật dòng lệnh lỗi `error: open(".git/FETCH_HEAD"): Permission denied` và menu `Run as Administrator`.
  * ⬛ **Che phủ thông tin nhạy cảm (Blur/Censor):** Che phần đường dẫn cá nhân chứa tên người dùng máy tính (`C:\Users\Admin\...`), địa chỉ IP, Token hoặc Email cá nhân nếu xuất hiện trên màn hình.

---

## 3. Yêu cầu 3: Soạn tin nhắn nhờ Giảng viên hỗ trợ (Bug Reporting Framework)

Nếu đã thử chạy với quyền Administrator nhưng vẫn không sửa được lỗi, ta sử dụng **Bug Reporting Framework** để soạn tin nhắn nhờ giảng viên hỗ trợ chuyên nghiệp và tiết kiệm thời gian:

```text
Kính gửi thầy Lê Hà Thanh Sang,

Em là Lê Hồ Thanh Thảo - Mã SV: N26DTCN030 (Lớp D26TXCN02-N). 
Em đang thực hành Bài tập Session 22 và gặp sự cố với Git trên máy tính cá nhân, em xin phép nhờ thầy hỗ trợ ạ:

1. Bối cảnh & Môi trường (Context):
   - OS: Windows 11 Home
   - Công cụ: Git Bash / VS Code Terminal
   - Thao tác: Em thực hiện lệnh `git pull origin main` thì bị dừng lại.

2. Mã lỗi thực tế (Actual Result):
   - Terminal xuất hiện thông báo: error: open(".git/FETCH_HEAD"): Permission denied

3. Các bước em đã tự khắc phục (Troubleshooting steps taken):
   - Em đã chạy lại Git Bash dưới quyền "Run as Administrator".
   - Em đã hỏi AI và thử lệnh đổi quyền sở hữu thư mục `.git` nhưng Terminal vẫn báo lỗi Permission Denied.

Em có gửi kèm ảnh chụp màn hình terminal khoanh vùng lỗi ở phía dưới. Em cảm ơn thầy nhiều ạ!