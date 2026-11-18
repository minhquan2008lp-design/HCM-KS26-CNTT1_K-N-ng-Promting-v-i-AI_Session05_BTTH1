# PROMPT: LẬP KẾ HOẠCH TÀI CHÍNH CÁ NHÂN BẰNG CREATE VÀ CoT

## 1. C – CONTEXT (Bối cảnh)

Một cá nhân có thu nhập biến động hàng tháng, có các khoản chi phí cố định, khoản nợ cần thanh toán và mục tiêu tiết kiệm.

Tôi cần xây dựng kế hoạch tài chính hàng tháng nhằm quản lý dòng tiền hợp lý, trả nợ đúng hạn, tiết kiệm tối thiểu 20% thu nhập sau thuế và duy trì quỹ dự phòng.

Dữ liệu đầu vào gồm:

- Thu nhập hàng tháng: [Số tiền]
- Thuế và các khoản khấu trừ: [Số tiền]
- Chi phí cố định: [Số tiền]
- Các khoản nợ: [Số tiền nợ, lãi suất, khoản trả tối thiểu và hạn thanh toán]
- Mục tiêu tiết kiệm: [Số tiền hoặc tỷ lệ %]

## 2. R – REQUEST (Yêu cầu)

Hãy lập một kế hoạch tài chính cá nhân hoàn chỉnh trong một tháng dựa trên dữ liệu đầu vào.

Yêu cầu:
- Tính toán thu nhập khả dụng.
- Phân bổ ngân sách cho chi phí cố định và trả nợ.
- Đảm bảo mục tiêu tiết kiệm tối thiểu 20% khi ngân sách đủ khả năng.
- Phân bổ phần tiền còn lại theo quy tắc 50/30/20 cải tiến.
- Đưa ra đề xuất giúp tối ưu hóa dòng tiền và hạn chế thiếu hụt tài chính.

## 3. E – EXPLANATION (Giải thích phương pháp)

Sử dụng phương pháp suy luận tuần tự (Chain-of-Thought) để thực hiện bài toán.

Hãy suy nghĩ từng bước một và trình bày các công thức, phép tính trung gian có thể kiểm chứng.

Thực hiện theo 4 bước:

**Bước 1: Tính thu nhập khả dụng**

Thu nhập thực nhận = Thu nhập trước thuế - Thuế và các khoản khấu trừ.

Số tiền còn lại = Thu nhập thực nhận - Tổng chi phí cố định.

Nếu đầu vào đã là thu nhập sau thuế thì không trừ thuế thêm lần nữa.

**Bước 2: Phân bổ trả nợ**

- Tính tổng các khoản trả nợ tối thiểu.
- Kiểm tra thời hạn thanh toán.
- Ưu tiên trả nợ đúng hạn.
- Xác định khả năng trả thêm cho khoản nợ có lãi suất cao.

**Bước 3: Trích lập tiết kiệm**

Tiền tiết kiệm tối thiểu = Thu nhập thực nhận × 20%.

Xác định số tiền dành cho tiết kiệm và quỹ dự phòng dựa trên mục tiêu tài chính.

**Bước 4: Phân bổ ngân sách linh hoạt**

Ngân sách linh hoạt = Thu nhập thực nhận - Chi phí cố định - Trả nợ tối thiểu - Tiền tiết kiệm.

Chia ngân sách linh hoạt theo quy tắc 50/30/20 cải tiến:

- 50%: Nhu cầu thiết yếu phát sinh.
- 30%: Chi tiêu cá nhân và giải trí.
- 20%: Trả nợ thêm hoặc bổ sung quỹ dự phòng.

## 4. A – ACTION (Hành động)

Hãy thực hiện các công việc sau:

**Phần 1: Trình bày các bước tính toán**

Với mỗi bước, cần thể hiện:
- Dữ liệu đầu vào.
- Công thức tính toán.
- Phép tính cộng, trừ, nhân, chia cụ thể.
- Kết quả trung gian.
- Nhận xét về tình hình tài chính.

**Phần 2: Xuất bảng phân bổ ngân sách**

Sử dụng Markdown Table theo mẫu:

| Hạng mục | Số tiền (VNĐ) | Tỷ lệ (%) | Ghi chú |
|---|---:|---:|---|
| Chi phí cố định | ... | ... | ... |
| Trả nợ tối thiểu | ... | ... | ... |
| Tiết kiệm | ... | ... | ... |
| Nhu cầu thiết yếu phát sinh | ... | ... | ... |
| Giải trí và cá nhân | ... | ... | ... |
| Trả nợ thêm / Quỹ dự phòng | ... | ... | ... |
| **TỔNG CỘNG** | **...** | **100%** | ... |

Tất cả số tiền và tỷ lệ phải được tính dựa trên thu nhập thực nhận sau thuế.

## 5. T – TONE (Giọng điệu)

- Sử dụng ngôn ngữ tiếng Việt rõ ràng, dễ hiểu.
- Trình bày ngắn gọn, logic và có tính chuyên nghiệp.
- Giải thích phép tính bằng cách đơn giản, dễ kiểm tra.
- Đưa ra lời khuyên thực tế, phù hợp với khả năng tài chính.
- Không sử dụng thuật ngữ phức tạp nếu không cần thiết.

## 6. E – EXTRAS (Yêu cầu bổ sung)

1. Không tự tạo dữ liệu khi người dùng chưa cung cấp.
2. Không bỏ qua các phép tính trung gian.
3. Không phân bổ ngân sách vượt quá thu nhập thực nhận.
4. Tỷ lệ tiết kiệm tối thiểu 20% nếu ngân sách đủ khả năng.
5. Tính tất cả tỷ lệ phần trăm trên cùng cơ sở thu nhập thực nhận.
6. Tổng số tiền phân bổ phải bằng thu nhập thực nhận.
7. Tổng tỷ lệ phần trăm phải chính xác 100%.
8. Không để trống số tiền trong bảng khi đã có đủ dữ liệu.
9. Nếu ngân sách không đủ, phải cảnh báo và đề xuất phương án điều chỉnh, không tự tạo kế hoạch cân đối giả.
10. Kiểm tra lại toàn bộ phép tính trước khi đưa ra kết quả cuối cùng.
11. Không sử dụng Python hoặc Pydantic, chỉ sử dụng phương pháp Prompting và tính toán số học.