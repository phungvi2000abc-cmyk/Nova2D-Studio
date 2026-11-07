NOVA 2D STUDIO — BẢN NGUYÊN MẪU ALPHA
====================================

Đây là bản thử nghiệm độc lập được xây dựng sau khi tham khảo cấu trúc gói Builda 1.86.0 do người dùng cung cấp. Nó không phải bản sửa đổi hay bản sao của Builda.

CÁCH MỞ TRÊN ĐIỆN THOẠI ANDROID
1. Giải nén Nova2D_Studio_Source.zip.
2. Mở thư mục Nova2D_Studio và mở index.html bằng Chrome hoặc trình duyệt tương thích.
3. Nếu trình duyệt không cho mở tệp HTML trực tiếp, hãy dùng một ứng dụng chạy máy chủ web cục bộ để mở thư mục này, hoặc lưu trang trên một máy chủ HTTPS.
4. Khi được phục vụ qua HTTPS, có thể thêm vào màn hình chính như một web app. Gói này KHÔNG phải APK Android.

CÁCH THỬ
- Mẫu game mặc định là Phiêu lưu 2D.
- Chỉnh PlayerController.cs rồi nhấn “Áp dụng code”.
- Nhấn “Chạy game”. Dùng phím A/D hoặc mũi tên, Space để nhảy; trên điện thoại dùng nút cảm ứng.
- Chọn đối tượng trong “Cấu trúc cảnh” để sửa thuộc tính.
- Nhấn “Lưu” để lưu cục bộ trong trình duyệt.
- “Xuất dự án” tạo tệp JSON .nova2d.json; menu “Dự án mới” có các mẫu game.
- Dùng nút “Nhập dự án” trên thanh công cụ để mở lại tệp .nova2d.json đã xuất trước đó.

API C#-STYLE ĐANG HỖ TRỢ
- MonoBehaviour, Start(), Update()
- trường public float/int/bool/string
- Input.GetAxisRaw("Horizontal"/"Vertical")
- Input.GetKeyDown(KeyCode.Space), KeyCode.R
- transform.position, transform.Translate(x, y)
- GetComponent<Rigidbody2D>(), body.velocity
- new Vector2(x, y), Time.deltaTime, Debug.Log(...)

GIỚI HẠN RẤT QUAN TRỌNG
- Trình soạn thảo dùng cú pháp C#-style và bộ chuyển đổi tập lệnh nhỏ do Nova 2D định nghĩa; không phải trình biên dịch C# đầy đủ và không chạy toàn bộ dự án Unity.
- Vật lý hiện là bản cơ bản: trọng lực, va chạm nền tảng và nhặt xu.
- Chưa có nhập sprite/âm thanh, animation editor, tilemap, shader, scene nhiều màn, AI pathfinding, multiplayer hoặc plugin.
- Chưa có chức năng xuất APK cho từng game được tạo.
- Tệp này là web app/PWA prototype, không phải file APK cài trực tiếp.

MÃ NGUỒN
index.html             Giao diện, runtime canvas 2D, trình soạn thảo và API mẫu
manifest.webmanifest   Khai báo web app
service-worker.js      Cache ngoại tuyến khi chạy từ HTTPS/localhost
README_VI.txt          Hướng dẫn tiếng Việt
