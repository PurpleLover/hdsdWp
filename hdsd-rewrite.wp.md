# Hướng dẫn sử dụng công cụ Wordpress

## Danh mục từ viết tắt & thuật ngữ
### Từ viết tắt
* HDSD - Hướng dẫn sử dụng

### Thuật ngữ
* Plugin - phần mở rộng, cài thêm, để hỗ trợ công cụ ban đầu
* Post - bài viết
* Page - trang giao diện
* Hosting - nơi lưu trữ mã nguồn của trang web, thường phải thuê ngoài hoặc mua máy chủ về tự làm
* Comment - bình luận


## Mục lục
1. [Giới thiệu](#Giới-thiệu)
2. [Điều kiện tiên quyết](#Điều-kiện-tiên-quyết)
3. [HDSD cơ bản](#HDSD-cơ-bản)
4. [HDSD Plugin](#HDSD-Plugin)
5. [Cài đặt trên Hosting](#Cài-đặt-trên-Hosting)
6. [Tham khảo](#Tham-khảo)

## Giới thiệu
Wordpress là công cụ xây dựng website quảng bá một cách dễ dàng và tiện lợi. Sau đây là giới thiệu khái quát về các tính năng có trong trang web mà chúng tôi xây dựng.

Trước hết là giao diện, giao diện bao gồm hai loại:
* Giao diện đứng: chỉ có các Page
* Giao diện ngang: có cả Page và Post
[Cách chuyển giao diện](#Cách-chuyển-giao-diện)

Tiếp theo là tính năng song ngữ trên trang Web: phải tạo hai trang Anh-Việt (đối với Page và Post) nếu muốn hiển thị song ngữ.

Vào thời điểm viết bài hướng dẫn sử dụng này, chúng tôi chưa có Hosting để đăng lên nên mọi đường dẫn mà chúng tôi cung cấp đều chạy trên `localhost:8080`, tức là máy tính của chúng tôi. Đến khi có Hosting, chúng tôi sẽ chỉnh sửa lại nội dung bài viết.

## Điều kiện tiên quyết
1. Đọc hiểu tiếng Anh ở mức phổ thông
2. Biết cách sử dụng máy vi tính và trình duyệt web

## Đăng nhập
Vào [địa chỉ này](http://localhost:8080/wordpress/) để tới trang chủ của website.

![home_screen](https://github.com/PurpleLover/hdsdWp/blob/master/images/login/home_screen.png)

Thêm `wp-admin` vào cuối trên thanh địa chỉ (có dạng `http://localhost:8080/wordpress/wp-admin`) để vào trang đăng nhập.

![login_screen](https://github.com/PurpleLover/hdsdWp/blob/master/images/login/login_screen.png)

Sau khi đăng nhập màn hình hiện ra sẽ có dạng như sau, với thanh công cụ nằm ở phía bên tay trái.

![dashboard_screen](https://github.com/PurpleLover/hdsdWp/blob/master/images/login/dashboard_screen.jpg)

### HDSD cơ bản
#### Posts
Trên thanh công cụ, chọn mục `Posts`, màn hình mới hiện ra có dạng như sau:

![posts_main](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/posts_main.jpg)

Chọn nút `Add New` để thêm mới bài viết.

![posts_addnew](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/posts_addnew.png)

Đặt tuỳ chỉnh như hình.

![posts_addnew_settings](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/posts_addnew_settings.png)

Chọn nút `Categories` để thêm mới thể loại, hoặc `Tags`. Hai phần này tương tự nhau nên chỉ chụp một hình.

![posts_categories](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/posts_categories.png)

#### Media
Trên thanh công cụ, chọn mục `Media`, màn hình hiện ra có dạng như sau:

![media_main](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/media_main.png)

**Lưu ý**: Mọi tranh ảnh, video khi gửi chọn trong lúc viết bài đều được lưu lại tại đây. Tuy nhiên, việc lưu trữ này sẽ rất tốn dung lượng của trang và sẽ gặp vấn đề với các gói Hosting tiết kiệm. Giải pháp đưa ra cho vấn đề này là dùng một trang thứ ba lưu trữ tranh ảnh/ video (có thể kể đến như _imageshank_, _Google Image_, _Tumblr_, _Blogger_, vân vân và mây mây) và nhúng vào bài viết thay vì lưu trữ trực tiếp bằng wordpress.

#### Pages
Trên thanh công cụ, chọn mục `Pages`, màn hình hiện ra có dạng như sau:

![pages_main](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/pages_main.png)

Khá giống với màn hình `Posts`, kể cả khi thêm mới:

![pages_addnew](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/pages_addnew.png)

Tuy nhiên tuỳ chỉnh có đôi chỗ khác một chút:

![pages_addnew_settings](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/pages_addnew_settings.png)

#### Comments
Trên thanh công cụ, chọn mục `Comments`, màn hình hiện ra có dạng như sau:

![comments_main](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/comments_main.png)

Phần `Comments` này chỉ quản lý những bình luận có trên bài viết và cung cấp các tác vụ đơn giản như xoá hoặc đánh dấu spam. Nếu đó là comment của mình thì có thể chỉnh sửa.

#### Appearance
##### Themes
Trên thanh công cụ, rê chuột mục `Appearance` và chọn `Themes`, màn hình hiện ra có dạng như sau:

![appearance_themes](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/appearance_themes.png)

Chỉ cần chú ý hai theme là:
* Astra: cho giao diện ngang
* GeneratePress: cho giao diện đứng

##### Menus
Trên thanh công cụ, rê chuột mục `Appearance` và chọn `Menus`, màn hình hiện ra có dạng như sau:

![appearance_menus_main](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/appearance_menus_main.png)

Để quản lý vị trí xuất hiện của Menu, làm như trong hình: (hiện giờ chỉ cần quan tâm đặt vị trí cho menu dọc)

![appearance_menus_location](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/appearance_menus_location.png)

Để thêm mới Menu, làm như trong hình:

![appearance_menus_addnew](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/appearance_menus_addnew.png)

#### Plugins
Trên thanh công cụ, chọn mục `Plugins`, màn hình hiện ra có dạng như sau:

![plugins_main](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/plugins_main.png)

Để thêm Plugin mới, làm như hình:

![plugins_addnew](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/plugins_addnew.png)

**Lưu ý**: Trước khi thêm Plugin hoặc huỷ kích hoạt Plugin cũ, hãy đọc kỹ xem Plugin đó có phù hợp với các Plugin đã có sẵn hay không.

#### Users
Trên thanh công cụ, chọn mục `Users`, màn hình hiện ra có dạng như sau:

![users_main](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/users_main.png)

Để thêm mới người dùng, chọn mục `Add New`, làm như hình sau:

![users_addnew](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/users_addnew.png)

Với các `Role` như sau:
* `Administrator`: có toàn quyền với trang web
* `Editor`: gần mạnh bằng admin nhưng không thể thay đổi giao diện và plugin, cũng như lệnh xoá web
* `Author`: chỉ có quyền với các Posts
* `Contributor`: chỉ có quyền chỉnh sửa và xoá Post
* `Subscriber`: chỉ có quyền xem

Để thay đổi thông tin cá nhân, chọn mục `Profile`, làm như hình sau:
* Cá nhân hoá trang

![users_profile_1](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/users_profile_1.png)

* Thay đổi mật khẩu

![users_profile_2](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/users_profile_2.png)

#### Tools
Để export (dùng cho mục đích backup), rê chuột vào `Tools` trên thanh công cụ, chọn `Export`, màn hình sẽ xuất hiện như sau:

![tool_export](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/tool_export.png)

**Lưu ý**: Nên export ít nhất 1 tuần 1 lần.

Để import, chỉ cần chọn `Import` và chọn phần của `Wordpress`.

#### Settings
Đây là tính năng quản lý những hiển thị chung trên trang.

* `General`: những thông tin chung của website, sẽ cập nhật sau khi up lên Hosting

![settings_general](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/settings_general.png)

* `Discussions`: quản lý bình luận (từ cấm, số lượng lượt hiển thị...)

![settings_discussion](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/settings_discussion.png)

* `Permalinks`: quản lý cách hiển thị đường dẫn

![settings_permalink](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/settings_permalink.png)

#### Cách chuyển giao diện
##### Giao diện dọc
Trên thanh công cụ, chọn `Appearance`, chọn kích hoạt (`Activate`) theme `GeneratePress`. Sau đó chọn mục `Customize` trong `Appearance`. Màn hình sẽ hiển thị như sau:

![customizer_main](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/customizer_main.png)

Chọn `Homepage Settings`
* ở mục `Your homepage displays` chọn `A static page` 
* ở dưới trong mục `Homepage`, chuyển sang `[VerticalLayout] Home`

![customizer_homepagesettings](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/customizer_homepagesettings.png)

Sau khi xong xuôi, quay lại màn hình Customizer và chọn `Additional CSS` và copy đoạn mã nguồn sau vào rồi chọn `Publish` (nếu chưa có mã nguồn nào).

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

Sau đó sẽ có dạng thế này.

![customizer_additionalCss](https://github.com/PurpleLover/hdsdWp/blob/master/images/_standard/customizer_additionalCss.png)

##### Giao diện ngang
Làm tương tự như trên nhưng chỉ chỉnh Homepage về `Trang chủ`

### HDSD Plugin
* [Hướng dẫn sử dụng các addon của Elementor](https://docs.elementor.com/) - do chính Elementor viết.

## Cài đặt trên Hosting
* [Chuyển host thủ công lên hosting](https://thachpham.com/wordpress/wordpress-tutorials/localhost-len-host-thu-cong.html#ftoc-heading-1)

## Tham khảo
(Sẽ bổ sung sau)