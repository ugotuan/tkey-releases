<div align="center">
  <h1>TKey for macOS</h1>
  <p><strong>Bộ gõ tiếng Việt native, xử lý cục bộ với Telex và VNI.</strong></p>
  <p><a href="https://raw.githubusercontent.com/ugotuan/tkey-releases/main/TKey-1.6.37.zip"><img src="https://img.shields.io/badge/T%E1%BA%A3i_TKey-1.6.37-DB3A34?style=for-the-badge&logo=apple&logoColor=white" alt="Tải TKey 1.6.37"></a></p>
  <p>
    <img src="https://img.shields.io/badge/macOS-13%2B-111827?style=flat-square&logo=apple" alt="macOS 13 trở lên">
    <img src="https://img.shields.io/badge/Universal-Apple_Silicon_%26_Intel-111827?style=flat-square" alt="Apple Silicon và Intel">
    <img src="https://img.shields.io/badge/Phi%C3%AAn_b%E1%BA%A3n-1.6.37-DB3A34?style=flat-square" alt="Phiên bản 1.6.37">
    <img src="https://img.shields.io/badge/C%E1%BA%ADp_nh%E1%BA%ADt_t%E1%BB%B1_%C4%91%E1%BB%99ng-Sparkle-059669?style=flat-square" alt="Cập nhật tự động">
  </p>
</div>

---

## Tải và cài đặt

1. Tải [TKey 1.6.37](https://raw.githubusercontent.com/ugotuan/tkey-releases/main/TKey-1.6.37.zip).
2. Giải nén và kéo `TKey.app` vào thư mục `/Applications`.
3. Mở TKey. Nếu macOS yêu cầu, xác nhận mở ứng dụng rồi cấp quyền bàn phím tại **Cài đặt hệ thống → Quyền riêng tư & Bảo mật → Trợ năng** và **Theo dõi đầu vào**.
4. Chọn bố cục bàn phím phù hợp và bật TKey từ biểu tượng trên thanh menu.

> Bản cài được ký bằng chứng thư cục bộ và chưa được notarize bằng Apple Developer ID. Nếu Gatekeeper chặn lần mở đầu, nhấp phải `TKey.app`, chọn **Mở**, rồi xác nhận. Chỉ tải gói từ repo phát hành này.

## TKey 1.6.37 (46)

- Thêm bảng emoji, kaomoji và biểu tượng cảm xúc dạng chữ, có tìm kiếm và nhóm theo chủ đề; dữ liệu được đóng gói sẵn để tìm kiếm cục bộ.
- Thêm phím tắt mở bảng emoji và chèn mục được chọn vào ô nhập đang focus.
- Thêm cập nhật tự động qua Sparkle 2, xác minh gói cập nhật bằng chữ ký EdDSA; kiểm tra mỗi 12 giờ, có nút kiểm tra thủ công và tùy chọn trong phần Giới thiệu.
- Cải thiện kiểm tra quyền bàn phím và chẩn đoán trạng thái Secure Input.
- Dùng glyph E/V do TKey vẽ trực tiếp cho trạng thái trên menu bar.

[Ghi chú phát hành](TKey-1.6.37.md) · [Mã nguồn](https://github.com/ugotuan/tkey)

## Cập nhật tự động

TKey kiểm tra appcast công khai mỗi 12 giờ qua HTTPS. Sparkle xác thực chữ ký EdDSA của ZIP trước khi cài đặt. Feed: [appcast.xml](appcast.xml). Khóa riêng dùng ký cập nhật chỉ nằm trong Keychain của người phát hành và không được lưu trong repo.

Bản 1.6.37 là phiên bản đầu tiên tích hợp Sparkle; người dùng bản cũ cần cài bản này thủ công một lần. Các phiên bản sau có thể cập nhật trực tiếp trong ứng dụng.

## SHA-256

| Tệp | SHA-256 |
|---|---|
| `TKey-1.6.37.zip` | `92c80e4f3eccca04f6eec74e9ca8c5eb202bad3031c086fbecdd2215bb705b15` |

Kiểm tra bằng `shasum -a 256 TKey-1.6.37.zip`.
