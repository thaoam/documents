---
layout: default
title: Cấu hình cPanel & WHM
nav_order: 2
---

# Configuration Cấu hình cho root cPanel & WHM
{: .no_toc }

Tài liệu này dành cho root server cấu hình cho server trên WHM để đáp ứng hiệu suất của server máy chủ phục vụ hosting WHM hệ thống.
{: .fs-6 .fw-300 }

## Mục lục
{: .no_toc .text-delta }

1. TOC
{:toc}

---

Bắt đầu nhanh với việc chỉ cần tải profile EasyApache4 này của Thaoam.net [**thaoam_easyapache4_config_profile.json**](https://github.com/thaoam/documents/tree/main/thaoam_easyapache4_config_profile.json) và upload lên EasyApache4 profile của server WHM và cho chạy mặc định profile này.

## Cài ionCube PHP Loader

ionCube PHP Loader cân thiết để cho WHMCS chạy trên server và làm client billing system bán hàng, chăm sóc khách hàng.


```yaml
Site error: the ionCube PHP Loader needs to be installed. This is a widely used PHP extension for running ionCube protected PHP code, website security and malware blocking. Please visit get-loader.ioncube.com for install assistance.
```
Đây là lỗi do chưa cài đặt và kích hoạt ionCube PHP Loader trên WHM.

### Cách 1: Cài ionCube PHP Loader trong WHM Tweak Settings

Để làm điều này ta sẽ:
1. Đăng nhập vào **cPanel & WHM** dành cho root.
2. Tìm tới **Tweak Settings**.
3. tìm **PHP**.
4. trong thông số **cPanel PHP loader** ta click chọn vào **ioncube**.

### Cách 2: Cài ionCube PHP Loader từ WHM 

Cài **IonCube trên WHM bằng EasyApache** trong WHM

Cách thức này sử dung GUI version của easyapache để cài đặt ioncube loader, nếu bạn không muốn cài đặt lại Apache và PHP thì đừng nên dùng phương thức này.

1. Đăng nhập vào WHM bằng tài khoản **root**.
2. Bên tay trái, hoặc trong ô tìm kiếm gõ **EasyApache** link
3. Trong '**Profile**', chọn '**Previous Saved Config**' và bấm tiếp vào nút '**Start customizing based on profile**' button.
4. Trong '**Apache Version**' bấm '**Next Step**'
5. Trong '**PHP Version**' bấm '**Next Step**'
6. Trong '**Short Options List**' bấm tích chọn vào '**Ioncube Loader for PHP**' và bấm vào nút '**Save and Build**' button.
7. Sau đó cần chờ hệ thống build đồng bộ, có thể mất từ **10-30 phút tùy độ mạnh yếu của hệ thống** phần cứng.

## Hướng dẫn cài SoapClient trên WHM, cPanel
```yaml
Your server does not support SOAPClient. Please install and activate it 
```
Đây là cách cài **SoapClient**, hay **soap** php extention khi cần thiết các module của WHMCS cần dùng tới.

1. Đăng nhập vào WHM bằng tài khoản **root**.
2. Bên tay trái, hoặc trong ô tìm kiếm gõ **EasyApache** link
3. Trong '**Currently Installed Packages**' Bấm vào nút '**Customize**' button.
4. Bấm vào '**PHP Extensions**' trong ô tìm kiếm gõ chữ "**soap**"
5. nó sẽ hiện ra các extensions liên quan dùng cho soapclient như là '**php74-php-soap**' hay '**php80-php-soap**' hoặc các phiên bản cao hơn về sau, chỉ cần **tích chọn cho nó sang màu xanh nước biển** để kích hoạt nó.
6. Bấm vào '**Next**' để tiếp tục
7. Đến phần '**Review**' Sau đó cần chờ hệ thống build đồng bộ, có thể mất từ **10-30 phút tùy độ mạnh yếu của hệ thống** phần cứng. thì kéo xuống dưới bấm vào nút '**Provision**' để hệ thống lưu lại, và kích hoạt soap, soapclient cho toàn bộ WHM và cPanel.
8. Sau đó cần chờ hệ thống build đồng bộ, có thể mất từ **10-30 phút tùy độ mạnh yếu của hệ thống** phần cứng.

## Xử lý lỗi cPanel/WHM Connection Refused
```yaml
đã từ chối kết nối. ERR_CONNECTION_REFUSED
```
Khi quá trình xử lý WHM gặp lỗi hệ thống kết nối bị từ chối, cách tốt nhất là update cPanel và WHM từ console.

Hướng dẫn vào console rồi gõ mã sau:

**/scripts/upcp --force**

## Upload Max. Filesize và Max. Post Size

Đây là những thông số hết sức cần thiết cho việc import những site lớn đã có sẵn vào hệ thống hosting

Hướng xử lý bật

1. Đăng nhập vào **WHM** bằng tài khoản root.
2. Bên trong "**Software**" mở "**MultiPHP INI Editor**" hoặc trong thanh tìm kiếm gõ vào "**MultiPHP INI Editor**".
3. bấm Ctrl + F bàn phím và gõ "**upload_max_filesize**" trong hộp giá trị gõ vào "**256M**".
4. bấm Ctrl + F bàn phím và gõ "**post_max_size**" trong hộp giá trị gõ vào "**256M**".
5. Apply thay đổi. Xong.


