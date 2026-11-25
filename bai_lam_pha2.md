# BÀI LÀM PHA 2 (ĐỀ LUYỆN TẬP CHỦ ĐỀ CHẠY AFFILIATE)

- **Họ tên:** Phạm Viết Toàn
- **Lớp:** HNKS26CNTT3
- **Link repository Pha2:** 
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** ChatGPT

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đăng ký gói Affiliate ra JSON

**KET QUA AI**

```text
[
  {
    "ma_goi": "TT",
    "ngay_bat_dau": "2026-12-20",
    "creator_chinh": 2,
    "thuc_tap_sinh": 1,
    "hang_tai_khoan": "thuong",
    "ghi_chu": null
  },
  {
    "ma_goi": "SP",
    "ngay_bat_dau": "2027-01-08",
    "creator_chinh": 3,
    "thuc_tap_sinh": 0,
    "hang_tai_khoan": "thuong",
    "ghi_chu": "cần ngồi bàn gần cửa ra vào"
  },
  {
    "ma_goi": "PRO",
    "ngay_bat_dau": null,
    "creator_chinh": 4,
    "thuc_tap_sinh": 0,
    "hang_tai_khoan": "vip",
    "ghi_chu": "cần mượn thêm đèn trợ sáng và phông xanh để quay mẫu"
  }
]
```

**Link trò chuyện:** https://chatgpt.com/share/6b06fc52-2270-83ec-9200-f1711664088c

## 4.3. Báo giá gói Affiliate bằng Chain-of-Thought

**KET QUA AI**

```text
### **1. Chuẩn hóa dữ liệu**

| Trường dữ liệu        | Giá trị       |
| --------------------- | ------------- |
| Gói dịch vụ           | TT            |
| Giá Creator chính     | 1.500.000đ    |
| Số Creator chính      | 4             |
| Số thực tập sinh      | 2             |
| Độ tuổi thực tập sinh | 16 và 17      |
| Trẻ nhỏ đi cùng       | 1 bé (7 tuổi) |
| Số bộ mic thuê        | 2             |

### **2. Tính toán chi tiết**

**Bước 1: Tiền Creator chính**

4 × 1.500.000 = 6.000.000đ

**Bước 2: Tiền thực tập sinh**

1.500.000 × 60% = 900.000đ/người

2 × 900.000 = 1.800.000đ

Bé 7 tuổi ngồi khu chờ: Miễn phí.

**Bước 3: Tổng tiền gói**

6.000.000 + 1.800.000 = 7.800.000đ

**Bước 4: Giảm giá team**

Team có 4 Creator chính nên được giảm 10%.

7.800.000 × 10% = 780.000đ

Tiền gói sau giảm:

7.800.000 - 780.000 = 7.020.000đ

**Bước 5: Phụ thu thuê mic**

2 × 250.000 = 500.000đ

**Bước 6: Tổng tiền**

7.020.000 + 500.000 = 7.520.000đ

Hoàn tất báo giá

# **[RESULT: 7.520.000 đồng]**
```

**Link trò chuyện:** https://chatgpt.com/share/6b06fc91-5330-83ec-9c4a-3ea2a51d6c1a

### b) Kiểm tra kết quả AI

Kết quả của AI đúng

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
[
  {
    "loai_su_co": "sai_phong",
    "so_khach": 3,
    "so_ca_bi_anh_huong": 2,
    "tom_tat": "3 Creator bị xếp vào phòng thiếu đèn livestream và cách âm trong 2 ca thực hành đầu."
  }
]
```

**Link trò chuyện:** https://chatgpt.com/share/6b06fcf9-6a14-83ec-b03d-251777d7bff3

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
Tiêu chí	Điểm	Minh chứng	Đề xuất sửa
1. Đúng thông tin (50%)	1/5	- Sai giá: “Gói TikTok Affiliate bên mình giá chỉ 1.200.000đ/người thôi” → Giá chuẩn là 1.500.000 đồng/Creator chính.

- Sai chính sách: “Bạn báo huỷ trước 5 ngày thì được hoàn lại đủ 100% tiền” → Huỷ trước 3–6 ngày chỉ được hoàn 50%.

- Cam kết sai: “gắn link là nổ đơn hoa hồng trăm triệu luôn” → Không có căn cứ đảm bảo doanh thu hoặc hoa hồng.	- “Gói TikTok Affiliate hiện có giá 1.500.000 đồng/Creator chính ạ.”

- “Nếu chị/anh huỷ trước ngày bắt đầu 5 ngày, trung tâm sẽ hoàn lại 50% phí đăng ký ạ.”

- Không cam kết doanh thu hoặc hoa hồng.
2. Đầy đủ (30%)	1.5/3	- Đã trả lời câu hỏi về giá và chính sách huỷ nhưng thông tin chính sách sai.

- “cứ chốt lẹ kẻo hết slot nè!” → Không hỏi khách hàng ngày đợt thực chiến và số lượng suất muốn đăng ký.	“Anh/chị dự kiến đăng ký đợt thực chiến ngày nào và muốn đăng ký bao nhiêu suất ạ?”
3. Giọng điệu (20%)	0.5/2	- “Dạ hello bạn nha!” → Cách chào thiếu chuyên nghiệp.

- “nổ đơn hoa hồng trăm triệu luôn ạ” → Cam kết hoa hồng thiếu căn cứ.

- “cứ chốt lẹ kẻo hết slot nè!” → Ngôn ngữ suồng sã, tạo áp lực chốt đơn.	Sử dụng cách diễn đạt lịch sự, chuyên nghiệp, cung cấp thông tin khách quan và không gây áp lực đăng ký.
Tổng kết	3/10	Nhân viên trả lời đủ chủ đề nhưng sai cả giá và chính sách hoàn tiền, đồng thời sử dụng ngôn ngữ thiếu chuyên nghiệp.	Cần kiểm tra thông tin chuẩn trước khi tư vấn và cải thiện cách giao tiếp với khách hàng.

Tổng điểm: 3/10
```

**Link trò chuyện:** https://chatgpt.com/share/6b07004e-fac4-83ec-a3f1-1b0d40c01b5a
