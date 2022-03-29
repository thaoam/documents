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

### Quick start: Use as a GitHub Pages remote theme

1. Add Just the Docs to your Jekyll site's `_config.yml` as a [remote theme](https://blog.github.com/2017-11-29-use-any-theme-with-github-pages/)

```yaml
remote_theme: just-the-docs/just-the-docs
```

<small>You must have GitHub Pages enabled on your repo, one or more Markdown files, and a `_config.yml` file. [See an example repository](https://github.com/pmarsceill/jtd-remote)</small>

### Local installation: Use the gem-based theme

1. Install the Ruby Gem
  ```bash
  $ gem install just-the-docs
  ```
  ```yaml
  # .. or add it to your your Jekyll site’s Gemfile
  gem "just-the-docs"
  ```

2. Add Just the Docs to your Jekyll site’s `_config.yml`
  ```yaml
  theme: "just-the-docs"
  ```

3. _Optional:_ Initialize search data (creates `search-data.json`)
  ```bash
  $ bundle exec just-the-docs rake search:init
  ```

3. Run you local Jekyll server
  ```bash
  $ jekyll serve
  ```
  ```bash
  # .. or if you're using a Gemfile (bundler)
  $ bundle exec jekyll serve
  ```

4. Point your web browser to [http://localhost:4000](http://localhost:4000)

If you're hosting your site on GitHub Pages, [set up GitHub Pages and Jekyll locally](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll) so that you can more easily work in your development environment.

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
