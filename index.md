---
layout: default
title: Lời mở đầu
nav_order: 1
description: "Đây là tài liệu mở dành cho nội bộ DNTN Thảo Am, root, manager, user, khách hàng, đối tác, clients, reseller, đại lý sử dụng nâng cao kiến thức và tư liệu công việc."
permalink: /
---

# Tài liệu kỹ thuật hướng dẫn của Thảo Am.
{: .fs-9 }

Tài liệu này nhằm bổ sung kiến thức và tránh nhầm lẫn, quên dành cho root, quản trị viên và đối tượng khách hàng, đối tác, reseller, quản trị viên WHM, WHMCS.
{: .fs-6 .fw-300 }

[Đặt mua Hosting](https://thaoam.net){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Bắt đầu tài liệu](#lời-mở-đầu){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## Lời mở đầu

### Đơn giản hóa

Sau khi đăng ký tên miền Tiếp mới thấy hết được sự phiền phức của nó khi chuyển đổi. Lên kế hoạch chuyển qua dùng miền quốc tế thôi. Khi đăng ký tên miền mới với chi phí quá cao 750.000đ một năm khi đăng ký mới, kèm phí gia hạn khủng khiếp lên đến 460.000đ các năm tiếp theo, và vì đăng ký tên miền qua một nhà cung cấp trung gian là công ty TNHH strongwings ở Hóc Môn, hiện tên miền đã bị kẹp 2 đầu quản lý bởi những người xa lạ. Do đó để đơn giản hóa sau các sự cố của doanh nghiệp, chúng tôi tạo ra tài liệu hướng dẫn này nhằm đơn giản hóa vận hành, và giúp khách hàng sử dụng dịch vụ đơn giản hơn.

Tài liệu kỹ thuật này dành cho nhân viên, đối tác của [Doanh nghiệp tư nhân Thảo Am](https://thaoam.net), trong việc hỗ trợ cấu hình máy chủ server, WHM & cPanel, root, domain, tên miền, và automation system billing WHMCS. Việc này giúp cho quá trình đồng bộ cấu hình server diễn ra ổn định, đáp ứng nhu cầu khách hàng, và giải quyết nhanh hoàn toàn các sự cố và đưa mọi thứ trở nên hoạt động ổn định.

### Cài đặt nhanh All-in-one tất cả trong một

Bắt đầu nhanh với việc chỉ cần tải profile EasyApache4 này của Thaoam.net [\thaoam_easyapache4_config_profile.json](https://github.com/just-the-docs/just-the-docs/tree/main/thaoam_easyapache4_config_profile.json) và upload lên EasyApache4 profile của server WHM và cho chạy mặc định profile này.

### tài liệu riêng về cấu hình WHM & cPanel

- [Xem tài liệu configuration cấu hình WHM & cPanel]({{ site.baseurl }}{% link docs/configuration.md %})

---

## Về dự án

Tài liệu này thuộc bản quyền của &copy; 2022-{{ "now" | date: "%Y" }} của Doanh nghiệp tư nhân Thảo Am, chịu trách nhiệm bởi [Phạm Xuân Tiếp](https://thaoam.net).

### License Bản quyền

Tài liệu hướng dẫn của Thảo Am tuân theo quy định và chứng thực theo [MIT license](https://github.com/just-the-docs/just-the-docs/tree/main/LICENSE.txt).

### Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. Read more about becoming a contributor in [our GitHub repo](https://github.com/just-the-docs/just-the-docs#contributing).

#### Những thành viên tham gia đóng góp dự án tài liệu này!

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul>

### Quy định về ứng xử

Tài liệu này là mở rộng cho các thành viên tham gia như nhân viên, đối tác, kỹ thuật.

[Xem chi tiết tài liệu quy định ứng xử bằng English](https://github.com/Thao-Am-Private-Charity-Funds-Vietnam/documents/tree/main/CODE_OF_CONDUCT.md) trên GitHub của doanh nghiệp.
