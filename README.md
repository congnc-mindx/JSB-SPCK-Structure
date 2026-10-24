# 🌱 Web Basic Starter

Bộ khởi đầu website **đa trang** để luyện HTML, CSS và Bootstrap 5. Mỗi trang là một file HTML riêng, chuyển trang bằng thẻ `<a>`.

## Bắt đầu

1. Chọn **Use this template** nếu repo đã bật chế độ template, hoặc **Code → Download ZIP** rồi giải nén.
2. Mở thư mục dự án bằng VS Code.
3. Mở `index.html` bằng trình duyệt. Nếu đã cài extension Live Server, có thể chọn **Open with Live Server**.
4. Tìm `TODO` và các bình luận hướng dẫn trong HTML, thay nội dung mẫu bằng bài của em. Lưu file và tải lại trình duyệt.

Không cần Node.js, npm hay bước build. Cần Internet để tải Bootstrap từ CDN.

## Đặt file ở đâu?

```text
web-basic-starter/
├── index.html             # Trang chủ
├── about.html             # Giới thiệu
├── contact.html           # Liên hệ
├── assets/
│   ├── css/
│   │   └── style.css      # CSS tự viết dùng chung
│   ├── js/
│   │   └── main.js        # JS tự viết, chưa cần dùng
│   └── images/
│       └── .gitkeep       # Giữ thư mục ảnh trên GitHub
└── README.md
```

- Đặt tên file không dấu, không có khoảng trắng: `san-pham.html`, `anh-nhom.jpg`.
- Giữ các trang HTML cùng cấp trong giai đoạn đầu để dễ viết đường dẫn.
- Ảnh đặt trong `assets/images/`; ví dụ: `<img src="assets/images/anh-nhom.jpg" alt="Các thành viên trong nhóm" class="img-fluid">`.
- CSS tự viết trong `style.css`, được nạp sau Bootstrap. JS tự viết trong `main.js`.
- Không sửa URL CDN tùy ý. Nếu đổi phiên bản Bootstrap, cập nhật cả URL và mã `integrity` theo tài liệu chính thức.

## Chưa dùng hết template thì sao?

**Không cần dùng hết mọi phần.** Đây là khung gợi ý; làm theo yêu cầu bài tập của thầy cô.

- Chưa học JS: giữ `main.js` chỉ có comment cũng được. Nếu xóa file, xóa luôn dòng `<script src="assets/js/main.js"></script>` ở các trang.
- Chưa có ảnh: để trống thư mục `images`. `.gitkeep` chỉ giữ thư mục trên GitHub, không phải ảnh và không ảnh hưởng website.
- Không cần một section hoặc thẻ nội dung: xóa cả khối HTML tương ứng; giữ các thẻ còn lại đóng/mở đầy đủ.
- Không cần một trang: có thể xóa nếu đề bài cho phép, rồi xóa mọi liên kết tới trang đó. Nếu bài yêu cầu đa trang, vẫn giữ ít nhất hai trang HTML liên kết với nhau.
- Xóa/đổi tên file nào thì cập nhật các đường dẫn đang trỏ tới file đó.

Giữ Bootstrap CSS và `bootstrap.bundle.min.js` để giao diện và nút menu trên điện thoại hoạt động.

## Thêm một trang mới

1. Sao chép `about.html` thành `products.html` ở cùng thư mục.
2. Sửa `<title>`, `<h1>` và nội dung trang.
3. Thêm liên kết `products.html` vào navbar của **tất cả các trang**.
4. Ở mỗi trang, chỉ gắn `active` và `aria-current="page"` cho liên kết của chính trang đó.

Navbar và footer đang được viết trực tiếp trong từng file để dễ học HTML. Khi sửa phần chung, nhớ sửa các trang còn lại. Khóa học sau có thể chuyển chúng thành phần dùng chung bằng công cụ phù hợp.

## Kiểm tra trước khi nộp

- Bấm thử các liên kết và kiểm tra ảnh có hiển thị không.
- Thu nhỏ trình duyệt, thử mở/đóng menu và kiểm tra nội dung không tràn ngang.
- Kiểm tra tên file đúng chữ hoa/thường; đường dẫn có thể chạy trên máy nhưng lỗi trên hosting nếu viết sai.
- Thay tên tác giả, thông tin mẫu và các nội dung TODO cần dùng.
- Trang liên hệ hiện dùng `mailto:` để mở ứng dụng gửi thư. Nếu thêm form, cần backend/dịch vụ xử lý để gửi hoặc lưu dữ liệu thật.

Tài liệu: [Bootstrap 5.3](https://getbootstrap.com/docs/5.3/getting-started/introduction/).
