---
layout: post
title:  "Pre-compiling css"
date:   2019-11-14 01:27:55 -0600
permalink: /pre-compiling-css/
comments: true
---

# What do you think of pre-compiling your CSS?

- Compare to regular CSS
- Which techniques did you use?
- Pros and cons?

<br>
I think the best benefit of using CSS-pre-processors compared to regular CSS is their improved syntax. It allows me to use variables for whatever I want. By using this technique I can easily and quickly do changes on all my web pages. It is user-friendly and doesn't take hours and hours spent before being able to start to use it. Here is an example whose variable has been assigned a color.
{% highlight ruby %}
$blue: #004BB4;
{% endhighlight %}

Another huge benefit of CSS-pre-processors is that it allows me to use a nested syntax which allows a cleaner way of targeting elements. I think the syntax becomes more natural and easily read. I feel like the code becomes more organized and structured in a way that it also becomes more maintainable.
For example:
{% highlight ruby %}
.navbar {
  font: $ubuntu-font;
  color: $blue;
  li {
    margin-left: 1rem;
    a {
      padding: 5px;
    }
  }
}
{% endhighlight %}
The cons I would say is that it becomes abit more difficult to debug, and I quess u have to learn a new syntax aswell. However I undoubtedly feel like the pros outweigh the cons.

I didn't do any major changes. Changed some main, header and footer colors,set some borders with a color, changed the post layout and centered it. Here is an example of a part of my code which has a nested syntax with variables.
{% highlight ruby %}
 a {
  color: $brand-color;
  text-decoration: none;

  &:visited {
    color: $visited-color;
  }

  &:hover {
    color: $text-color;
    text-decoration: underline;
  }

  .social-media-list &:hover {
    text-decoration: none;

    .username {
      text-decoration: underline;
    }
  }
}
{% endhighlight %}
