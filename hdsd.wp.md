# Hướng dẫn sử dụng công cụ Wordpress

## Lời mở đầu
Sau khi xem xét kĩ lưỡng các nội dung để hướng dẫn, chúng tôi quyết định sẽ hướng dẫn những vấn đề chung nhất. Những vấn đề liên quan đến chi tiết cách thức viết bài, tuỳ chỉnh giao diện sẽ được hướng dẫn trong buổi gặp mặt trực tiếp và sẽ bổ sung vào tài liệu hướng dẫn sau nếu có yêu cầu.

## Điều kiện tiên quyết
1. Biết cách dùng máy tính và trình duyệt web
2. Luôn ghi nhớ mật khẩu tài khoản hoặc nhớ chỗ lưu mật khẩu

## Cài đặt (triển khai trên hosting)
(sẽ bổ sung sau)

## Giới thiệu chung
### Thanh công cụ

![thanh công cụ](https://github.com/PurpleLover/hdsdWp/blob/master/assets/tool_sets.png)

Vị trí ở phía bên tay trái màn hình, bao gồm một sổ dọc dài, có các phân vùng cơ bản:
* Posts: viết bài tại đây
* Media: các phương tiện sẽ lưu tại đây (bao gồm hình ảnh, video, âm thanh)
* Pages: các trang của website sẽ lưu tại đây
* Comments: kiểm soát bình luận
* Appearance: kiểm soát Themes và Menu chính
* Plugins: cài đặt thêm các Plugins hỗ trợ
* Users: kiểm soát người dùng và phân quyền
* Tools: các công cụ để export/import dữ liệu (dùng cho việc backup dữ liệu định kỳ)
* Settings: các cài đặt chung được cấu hình trong này
Ngoài những phân vùng kể trên, với mỗi plugin sau khi được cài đặt sẽ (có thể có) thêm các phân vùng tương ứng với plugin sử dụng, trong dự án này dùng thêm các Plugin sau:
* Elementor: dùng để chỉnh sửa giao diện
* Statistics: dùng để thống kê
* Polang: dùng để đa ngôn ngữ (song ngữ)
* Smart Slider, Orbit Fox, AE Templates, WPForms, Snippets và một số plugins khác để hỗ trợ giao diện
Cách sử dụng các plugin này, đặc biệt là Elementor sẽ được hướng dẫn trực tiếp.

### Giao diện
Bao gồm hai kiểu
* Đứng
  * Ưu điểm: lạ, khác biệt
  * Nhược điểm: không thể áp dụng khi nội dung phình to ra
* Ngang
  * Ưu điểm: dễ nhìn, không gặp vấn đề khi nội dung phình to ra
  * Nhược điểm: phổ biến
Để thay đổi giữa hai giao diện này đòi hỏi phải thực hiện các bước thật chuẩn, bằng không sẽ gây ra lỗi.

### Song ngữ
Wordpress hỗ trợ đa ngôn ngữ thông qua plugin của Polang, sẽ được cài đặt sẵn khi triển khai trên hosting thuê ngoài. Lưu ý, Polang chỉ hỗ trợ biên dịch vài đoạn, các nội dung còn lại trên trang cần phải được biên dịch (bằng tay) ra ngôn ngữ khác nếu muốn sử dụng đa ngôn ngữ.

Để thêm phiên bản song ngữ cho một trang, tích vào dấu + như hình,

![thêm bản song ngữ](https://github.com/PurpleLover/hdsdWp/blob/master/assets/translate_1.png)

rồi nhập tiêu đề và chọn Publish

## Đăng nhập và phân quyền
### Đăng nhập
Thêm `/wp-admin` vào thanh địa chỉ để vào trang đăng nhập. Tên tài khoản và mật khẩu sẽ được gửi qua kênh khác vì lý do bảo mật.

![trang đăng nhập](https://github.com/PurpleLover/hdsdWp/blob/master/assets/login_screen.png)

**Lưu ý**: thay đổi mật khẩu sau khi triển khai trên hosting.
### Phân quyền
Sau khi đăng nhập thành công vào tài khoản quản trị viên (`admin`), vào phân vùng Users trên thanh công cụ bên tay trái, chọn:

![phân quyền](https://github.com/PurpleLover/hdsdWp/blob/master/assets/user_section.png)

* `All Users` để xem các tài khoản
* `Add New` để thêm mới tài khoản
* `Your Profile` để chỉnh sửa lại thông tin tài khoản (và đổi mật khẩu)

## Cách chuyển giao diện
### Giao diện đứng
1. Vào Appearance/Themes và chọn Activate trên GeneratePress
2. Vào Appearance/Customize, chọn Additional CSS và dán đoạn code sau vào
```
@media (min-width: 769px) {
  .site-header {
    display: none;
  }

  .gen-sidebar-nav {
    width: 20%;
    height: 100%;
    position: fixed;
    top: 0px;
    left: 0px;
    opacity: 1;
    background-color: white;
    background-repeat: no-repeat;
    background-position: top center;
    border-style: hidden;
    border-top-width: 20px;
    border-top-style: solid;
    border-top-color: white;
	}
	.site-footer {
		display: none;
	}
	#page {
		height: 100vh;
		width: 100%;
	}
	.site-main{
		margin-left:0px !important;
	}
	.tablet-push-25{
		left: 20% !important;
	}
	.tablet-grid-75, grid-75 {
		width: 80% !important;
	}
	.site-logo {
		max-width: 50%;
		display: block;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 10%;
	}
	
	.main-title, .main-title a {
		font-size: 1.2rem;
		color: black!important;
		text-align: center;
		margin-bottom: 40%;
	}
	.main-title a:hover {
		color: #e96656 !important;
	}
	
	.eael-img-accordion {
		height: 100vh !important;
	}
	.menu-item {
		border-bottom: 1px solid black;
	}
	.menu-item:first-child {
		border-top: 1px solid black;
	}
	.menu-item a:hover {
		color: #e96656 !important;
	}
}
.site-info {
	display: none;
}
```
3. Vẫn trên trang Customize, tìm Homepage Settings và chuyển Homepage sang `[VerticalLayout] Home` và chọn Publish.

### Giao diện ngang
1. Vào Appearance/Themes và chọn Activate trên Neve
2. Vào Appearance/Customize và chỉnh Homepage Settings về `Trang chủ` và chọn Publish.

## Sử dụng các công cụ
### Menu
Để tạo mới một menu, chọn Menus trong Appearance, chọn create a new menu, đặt tên cho Menu và thêm các đầu mục như hình:
![menu_custom](https://github.com/PurpleLover/hdsdWp/blob/master/assets/menu_trans_1.png)
* URL là đường link dẫn tới trang cần hiển thị, hiện tại đang sử dụng localhost
* Link Text là tên đầu mục sẽ hiển thị lên trên menu
