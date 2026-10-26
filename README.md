# PAYKX – PHÂN TÍCH VÀ KIỂM THỬ DỮ LIỆU

## Phần 1. Phân tích Record và Field

- **Record:** Là một hàng dữ liệu, đại diện cho một giao dịch trong bảng Excel.
- **Field:** Là một cột dữ liệu, ví dụ: Mã giao dịch, Mã người dùng, Tên người dùng, Số tiền, Phí ngân hàng và Trạng thái.

**Yêu cầu dữ liệu:** Không Merge Cells trong vùng dữ liệu, không để hàng trống giữa các bản ghi và mỗi cột chỉ chứa một loại thông tin.

## Phần 2. Triển khai

Nộp riêng file khác

## Phần 3. Kiểm thử lỗi #N/A

Khi hàm VLOOKUP trả về lỗi `#N/A`, cần kiểm tra theo bốn bước:

1. **Kiểm tra mã:** Đảm bảo mã giao dịch hoặc mã người dùng được nhập đúng và tồn tại trong bảng.
2. **Kiểm tra khoảng trắng:** Sử dụng hàm TRIM để loại bỏ khoảng trắng thừa.
3. **Kiểm tra vùng tra cứu:** Đảm bảo cột đầu tiên của vùng tra cứu chứa mã cần tìm.
4. **Kiểm tra công thức:** Kiểm tra vùng dữ liệu, số thứ tự cột và tham số FALSE để tìm kiếm chính xác.

## Giải thích thêm

Hàm TRIM giúp làm sạch dữ liệu trước khi tra cứu. Hàm VLOOKUP kết hợp với FALSE giúp tìm đúng thông tin theo mã. Việc chuẩn hóa bảng dữ liệu giúp hạn chế lỗi và thuận tiện hơn khi đối soát giao dịch PayKX.
