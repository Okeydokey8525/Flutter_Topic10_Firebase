# 🔥 Firebase Real-time Demo - HUIT (Chương 6)

Dự án này là bản Demo tách biệt nhằm minh họa các tính năng cốt lõi của **Firebase** trong lập trình di động, bám sát nội dung lý thuyết Chương 6 của học phần.

---

## 🎯 Mục Tiêu Demo
Bản demo này tập trung vào 4 nội dung chính:
1.  **6.1. Cấu hình:** Kết nối Flutter với Firebase qua tệp `google-services.json`.
2.  **6.2. Xác thực (Auth):** Đăng ký/Đăng nhập tài khoản bằng Email & Password.
3.  **6.3. Firestore:** Hệ thống Chat Real-time (Đồng bộ dữ liệu tức thì).
4.  **6.4. Storage:** Tải lên và hiển thị hình ảnh/video từ đám mây.

---

## 📂 Cấu Trúc Mã Nguồn (Logic Layers)
Để giảng viên dễ theo dõi, mã nguồn được chia thành các phần tương ứng với lý thuyết:

* **`lib/main.dart`**: Thực hiện **Mục 6.1** - Khởi tạo Firebase ngay khi App bắt đầu.
* **`lib/services/firebase_service.dart`**: Chứa toàn bộ Logic xử lý Firebase:
    * `signUp()` / `signIn()`: Minh họa **Mục 6.2**.
    * `getMessages()` / `sendMessage()`: Minh họa **Mục 6.3** (Sử dụng Stream).
    * `uploadFile()`: Minh họa **Mục 6.4**.
* **`lib/screens/`**: Giao diện trực quan để trình diễn các tính năng trên.

---

## 🛠️ Hướng Dẫn Cài Đặt Cho Giảng Viên/Hội Đồng

1. **Cấu hình môi trường:**
   * Clone dự án: `git clone [Link_Repo]`
   * Cài đặt thư viện: `flutter pub get`

2. **Kết nối Firebase (6.1):**
   * Đảm bảo tệp `google-services.json` đã được đặt trong `android/app/`.
   * Kiểm tra `applicationId` trong `build.gradle` khớp với cấu hình trên Firebase Console.

3. **Chạy ứng dụng:**
   * Sử dụng máy ảo hoặc thiết bị thật để kiểm tra tính năng Real-time.

---

## 🎬 Kịch Bản Trình Diễn (Demo Script)

### Bước 1: Xác thực (6.2)
Thực hiện tạo tài khoản mới trên App và kiểm tra danh sách User xuất hiện ngay lập tức trên **Firebase Console -> Authentication**.

### Bước 2: Dữ liệu thời gian thực (6.3)
Gửi tin nhắn chat. Sử dụng một thiết bị thứ hai hoặc trình duyệt web để thấy dữ liệu trong **Firestore** thay đổi và đồng bộ lên App mà không cần tải lại trang.

### Bước 3: Lưu trữ đa phương tiện (6.4)
Chọn một hình ảnh từ thư viện máy, thực hiện Upload. Show cho giảng viên thấy tệp tin đã được lưu trữ an toàn trong **Firebase Storage** và hiển thị lại trên giao diện Chat thông qua URL.

---

## 🏫 Thông Tin Sinh Viên
* **Họ tên:** Lê Đức Lương (Huy)
* **MSSV:** 2001230490
* **Lớp:** [Điền tên lớp của Huy vào đây]
* **Trường:** Đại học Công Thương TP.HCM (HUIT)
