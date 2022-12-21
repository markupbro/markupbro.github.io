---
layout: post
title: "Web UI markup development"
date: 2022-12-17 00:47:11 +0900
categories: stories
---

안녕하세요!

마크업브로는 웹 UI 마크업(퍼블리싱) 작업자의 블로그입니다.

<div class="ham-wrap">
  <button type="button" class="ham-btn">
    <span></span>
  </button>
</div>

<script>
  $(function() {
    $('.ham-btn').on('click', function(e) {
      var cl = $(e.target);
      if (cl.hasClass('open'))
        cl.removeClass('open').addClass('close');
      else {
        cl.removeClass('close').addClass('open');
      }
    });
  })
</script>

<!-- {% highlight ruby %}
def print_hi(name)
puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %} -->

보이는 블로그는 [Jekyll][jekyll-docs] + [Github][github-pages] Pages로 작성되었습니다.

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]: https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
[github-pages]: https://talk.jekyllrb.com/
