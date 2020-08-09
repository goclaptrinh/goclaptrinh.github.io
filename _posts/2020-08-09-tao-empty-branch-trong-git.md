---
layout: post
title: Tạo empty branch trong git
published: true
---
Khi làm việc với git, thông thường chúng ta sẽ có nhu cầu tạo một nhánh mới được sao chép từ một nhánh có sẵn. Nhưng cũng có lúc chúng ta cần tạo một nhánh mới hoàn toàn trống. Chẳng hạn như chúng ta cần phát triển một nhánh mới với nội dung hoàn toàn khác và không dính líu gì tới những nhánh đã tồn tại. Nếu bạn đang loay hoay tìm cách để làm việc này thì bài viết này sẽ giúp bạn một cách nhanh chóng.

Chúng ta bắt đầu từ câu lệnh như sau:
{% highlight bash %}
git checkout --orphan <tên_nhánh>
{% endhighlight %}

Sau đó một bước quan trọng chúng ta cần làm là xoá tất cả nội dung trong nhánh mới đi, để tạo nhánh trống rỗng:
{% highlight bash %}
git rm -rf .
{% endhighlight %}

Cuối cùng, kiểm tra lại kết quả:
{% highlight bash %}
ls -la
{% endhighlight %}