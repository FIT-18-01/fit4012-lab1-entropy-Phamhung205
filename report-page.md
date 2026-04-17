# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Nắm vững lý thuyết Entropy, Redundancy và hoàn thiện kỹ năng cài đặt thuật toán tìm nghịch đảo Modulo.
## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|:---|---:|---:|:---|
| aaaa | 0.00 | 100% | Chuỗi lặp lại hoàn toàn, không chứa thông tin mới. |
| abcd | 2.00 | thấp | Các ký tự xuất hiện với xác suất bằng nhau, độ hỗn loạn cao. |
| hello world | ~2.85 | Trung bình | Có sự lặp lại nhẹ (ký tự 'l', 'o'), cấu trúc ngôn ngữ tự nhiên. |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|:---|:---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | không tồn tại |

## 4. Kết luận
- Khó khăn: Việc xử lý các trường hợp số âm trong thuật toán Euclid mở rộng và định dạng số thập phân cho Entropy.Điều giúp hiểu rõ: Việc trực quan hóa các bước chia dư trong thuật toán Euclid và so sánh sự khác biệt giữa chuỗi `aaaa` (dễ đoán) với chuỗi ngẫu nhiên đã giúp em nắm bắt khái niệm nhanh hơn.
