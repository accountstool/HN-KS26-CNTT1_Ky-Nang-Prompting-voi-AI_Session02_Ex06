

## Phần 1. Vì sao AI có thói quen chào hỏi với chúc kết

- AI được huấn luyện trên kho dữ liệu hội thoại giữa người với người, nơi câu trả lời mẫu mực luôn mở đầu bằng lời chào và khép lại bằng lời chúc hay một lời tạm biệt nào đó, nên khi sinh chữ nó chọn cụm mở đầu có xác suất xuất hiện cao nhất trong kho dữ liệu được train đó

## Phần 2. Prompt hoàn chỉnh 

```text
Bạn là bộ xử lý dữ liệu của hệ thống ERP TechShop, nhiệm vụ là chuyển biên bản tiếp nhận bảo hành dạng văn bản thành JSON.

Quy tắc bắt buộc:
- Chỉ trả về chuỗi JSON thuần túy, không dùng markdown block hay loại văn bản không hợp lệ nào khác, không giải thích, bắt đầu bằng { và kết thúc bằng }
- Cấm chào hỏi, cấm lời chúc, cấm câu dẫn kiểu "Dưới đây là dữ liệu", cấm mọi ký tự nào nằm ngoài JSON
- Thông tin thiếu trong biên bản thì điền null, không tự bịa, không kèm ghi chú
Cấu trúc bắt buộc:
{
  "customer_name": "họ tên khách hàng",
  "device": "tên thiết bị",
  "issue": "lỗi tiếp nhận"
}
```
