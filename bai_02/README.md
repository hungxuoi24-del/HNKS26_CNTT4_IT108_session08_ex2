# Bài 2: Kiểm Tra Tài Liệu Trước Khi Xuất Bản

## Phần 1. Phân tích lỗi cú pháp

1. **Lỗi cú pháp chèn ảnh (Logo PTIT):**
   - **Cú pháp sai:** `[Logo PTIT] (https://ptit.edu.vn/logo.png)`
   - **Giải thích:** Dòng này bị thiếu dấu chấm cảm `!` ở đầu và có khoảng trắng thừa giữa dấu ngoặc vuông `]` và ngoặc đơn `(`[cite: 1]. Do đó, Markdown không nhận diện đây là ảnh mà chỉ hiển thị chuỗi chữ thông thường. Cú pháp đúng phải là: `![Logo PTIT](https://ptit.edu.vn/logo.png)`.

2. **Lỗi phân cấp tiêu đề (Heading):**
   - **Cú pháp sai:** Dùng `# Tiêu đề 1` ở trên, sau đó dùng `### Giới thiệu dự án`.
   - **Giải thích:** Vi phạm nguyên tắc phân cấp tiêu đề liên tục ($H1 \rightarrow H2 \rightarrow H3$). Việc nhảy từ H1 thẳng xuống H3 làm cấu trúc bài viết bị lộn xộn. Ngoài ra, việc dùng 2 tiêu đề H1 trong bài cũng vi phạm quy tắc "Mỗi bài chỉ nên có 1 H1 duy nhất"[cite: 1].

3. **Lỗi cú pháp in đậm văn bản:**
   - **Cú pháp sai:** `Đây là đoạn văn bản in đậm.`[cite: 1]
   - **Giải thích:** Thiếu cặp dấu `**` (hoặc `__`) ở hai đầu văn bản. Trình đọc Markdown sẽ hiểu đây là văn bản thường chứ không phải chữ in đậm.

---

## Phần 2. Mã Markdown hoàn thiện

# Quản Lý Dự Án Sinh Viên

![Logo PTIT](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSQ3gTkJtiL3t4ZZutk1mCkBqRvyREPoXoC4DX3gEpRmg&s)

## 1. Giới thiệu dự án
**Đây là đoạn văn bản in đậm.** Tài liệu này dùng để quản lý hệ thống đào tạo và sinh viên.

## 2. Mục tiêu
- Quản lý sinh viên
- Quản lý môn học