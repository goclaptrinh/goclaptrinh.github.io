---
layout: post
title: "Hướng dẫn tạo môi trường ảo cho Python"
published: true
---
Mở terminal, sau đó change directory đến thư mục chứa project:

{% highlight bash %}
$ cd my-project
{% endhighlight %}

Tạo môi trường ảo, đặt tên là “venv”:

{% highlight bash %}
$ virtualenv venv
{% endhighlight %}

Vẫn đứng ở thư mục hiện tại, tiến hành kích hoạt môi trường ảo:

{% highlight bash %}
$ venv\Scripts\activate
{% endhighlight %}

Make sure file requirements.txt tồn tại trong thư mục gốc của project, tiến hành cài đặt các gói cần thiết:

{% highlight bash %}
$ pip install -r requirements.txt
{% endhighlight %}

Sau khi cài đặt xong, kiểm tra lại version của python, và các gói vừa cài đặt:

{% highlight bash %}
$ python --version
$ pip freeze
{% endhighlight %}
