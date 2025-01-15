---
layout: post
title:  "Multiples of 3 or 5"
date:   2025-01-15 01:25:31 -0500
categories: euler
---

Solution below

{% highlight rust %}
fn main() {
    let mut r = 0;

    for i in 1..1000 {
        if [3, 5].iter().any(|x| i % x == 0) {
            r += i;
        }
    }

    println!("{r}");
}
{% endhighlight %}