# ChainHub Documentation Agent Instructions

Tệp này hướng dẫn các AI Agent (như GitHub Copilot) cách viết, chỉnh sửa và quản lý tài liệu cho ChainHub.

## Mục tiêu dự án
Cung cấp tài liệu kỹ thuật chính xác, dễ hiểu và chuyên nghiệp cho nền tảng tập hợp API AI của ChainHub.

## Quy định về ngôn ngữ và thuật ngữ
- **Ngôn ngữ chính**: Tiếng Anh
- **Thuật ngữ nhất quán**:
  - Giữ nguyên tên các mô hình: GPT-4o, Claude 3.5 Sonnet, Gemini 1.5 Pro, Midjourney, v.v.
  - "API Key", "Endpoint", "Streaming" giữ nguyên định dạng kỹ thuật.

## Phong cách viết tài liệu
- **Giọng văn**: Chuyên nghiệp, hỗ trợ, sử dụng "bạn" (second person).
- **Cấu trúc câu**: Ngắn gọn, mỗi câu tập trung vào một ý chính.
- **Định dạng**:
  - Sử dụng **Bold** cho các phần tử giao diện hoặc điểm quan trọng.
  - Sử dụng `Inline Code` cho tham số, đường dẫn tệp, và lệnh terminal.
  - Tiêu đề dùng Sentence case (Viết hoa chữ cái đầu tiên của câu).

## Hướng dẫn cho Mintlify & MDX
- Luôn kiểm tra cấu trúc điều hướng trong `docs.json` trước khi thêm trang mới.
- Ưu tiên sử dụng các Component của Mintlify (`<Card>`, `<Note>`, `<Warning>`, `<Steps>`, `<Tabs>`) thay vì HTML thuần.
- Mỗi trang `.mdx` hoặc `.md` phải có Frontmatter đầy đủ: `title` và `description`.
- Hình ảnh phải được đặt trong thư mục `images/` và tham chiếu bằng đường dẫn tuyệt đối bắt đầu bằng `/`.

## Ví dụ mã nguồn (Code snippets)
- Luôn chỉ định ngôn ngữ trong khối mã (ví dụ: ```python, ```javascript).
- Thêm tên tệp nếu cần thiết: ```python main.py.
- Cung cấp ví dụ thực tế với các tham số của ChainHub (ví dụ: base_url: `https://api.chainhub.tech/v1`).
- Luôn bao gồm phần xử lý lỗi cơ bản (Try-Catch).

## Môi trường làm việc
- Dự án đang được chạy trong **WSL**. Khi hướng dẫn lệnh terminal, đảm bảo chúng tương thích với Linux/Bash.

## Những điều cần tránh
- Không sửa đổi cấu trúc điều hướng trong `docs.json` mà không cập nhật các liên quan.
- Không sử dụng các placeholder vô nghĩa (như `foo`, `bar`).
- Tránh tạo các trang trống hoặc thiếu mô tả sơ lược.
