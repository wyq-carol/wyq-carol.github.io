---
layout: post
title: "My first blog"
author: "wyq-carol"
tags: Algebra
excerpt_separator: <!--more-->
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas tincidunt ornare nibh, non elementum augue tempus eget. Pellentesque tempus scelerisque iaculis.<!--more--> Nullam interdum ultricies nibh quis sollicitudin. Donec ornare fermentum facilisis. Ut at sem ac sem imperdiet varius a eget tortor. Nam eu augue eget orci semper maximus in eget augue. Mauris ornare, nisl ut suscipit consectetur, mi quam interdum tellus, at rutrum quam eros ultrices mi.

# Up-Looking Cholesky

$\left(\begin{matrix}l_{11} & 0 & 0 \\ l_{12} & l_{22} & 0 \\ l_{13} & l_{23} & l_{33} \end{matrix}\right)\left(\begin{matrix}l_{11} & l_{12} & l_{13} \\ 0 & l_{22} & l_{23} \\ 0 & 0 & l_{33} \end{matrix}\right) = \left(\begin{matrix} a_{11} & a_{12} & a_{13} \\ a_{12} & a_{22} & a_{23} \\ a_{13} & a_{23} & a_{33} \end{matrix}\right)$

1. $\left(\begin{matrix} l_{11} \end{matrix}\right)\left(\begin{matrix} l_{11} \end{matrix}\right) = \left(\begin{matrix} a_{11} \end{matrix}\right)$ 
   * $l_{11} ^2 = a_{11}$ 解 $l_{11}$
2. $\left(\begin{matrix} l_{11} & 0 \\ l_{12} & l_{22} \end{matrix}\right) \left(\begin{matrix} l_{11} & l_{12} \\ 0 & l_{22} \end{matrix}\right) = \left(\begin{matrix} a_{11} & a_{12} \\ a_{12} & a_{22} \end{matrix}\right)$
   * $\left(\begin{matrix} l_{12} \end{matrix}\right)\left(\begin{matrix} l_{11} \end{matrix}\right) = \left(\begin{matrix} a_{12} \end{matrix}\right)$ 解 $l_{12}$
   * $l_{12}^2+l_{22} ^2 = a_{22}$ 解 $l_{22}$
3. $\left(\begin{matrix}l_{11} & 0 & 0 \\ l_{12} & l_{22} & 0 \\ l_{13} & l_{23} & l_{33} \end{matrix}\right)\left(\begin{matrix}l_{11} & l_{12} & l_{13} \\ 0 & l_{22} & l_{23} \\ 0 & 0 & l_{33} \end{matrix}\right) = \left(\begin{matrix} a_{11} & a_{12} & a_{13} \\ a_{12} & a_{22} & a_{23} \\ a_{13} & a_{23} & a_{33} \end{matrix}\right)$
   * $\left(\begin{matrix} l_{13} & l_{23} \end{matrix}\right) \left(\begin{matrix} l_{11} & l_{12} \\ 0 & l_{22} \end{matrix}\right) = \left(\begin{matrix} a_{13} & a_{23} \end{matrix}\right)$ 解 $l_{13}$ $l_{23}$ （同 $xb = y$ 已知 $b,y$ 求 $x$）
   * $l_{13}^2+l_{23} ^2+l_{33} ^2= a_{33}$ 解 $l_{33}$

# Headers

{% highlight markdown %}

# H1

## H2

### H3

#### H4

##### H5

###### H6

{% endhighlight %}

# H1

## H2

### H3

#### H4

##### H5

###### H6

# Text formatting

{% highlight markdown %}

- **Bold**

- _Italics_

- ~~Strikethrough~~

- <ins>Underline</ins>

- <sup>Superscript</sup>

- <sub>Subscript</sub>

- Abbreviation: <abbr title="HyperText Markup Language">HTML</abbr>

- Citation: <cite>&mdash; Chester How</cite>
  {% endhighlight %}

- **Bold**

- _Italics_

- ~~Strikethrough~~

- <ins>Underline</ins>

- <sup>Superscript</sup>

- <sub>Subscript</sub>

- Abbreviation: <abbr title="HyperText Markup Language">HTML</abbr>

- Citation: <cite>&mdash; Chester How</cite>

# Lists

{% highlight markdown %}

1. Ordered list item 1
2. Ordered list item 2
3. Ordered list item 3
* Unordered list item 1
* Unordered list item 2
* Unordered list item 3
  {% endhighlight %}
1. Ordered list item 1
2. Ordered list item 2
3. Ordered list item 3
* Unordered list item 1
* Unordered list item 2
* Unordered list item 3

# Links

{% highlight markdown %}
Check out tale on [GitHub](https://github.com/chesterhow/tale).
{% endhighlight %}

Check out tale on [GitHub](https://github.com/chesterhow/tale).

# Images

{% highlight markdown %}
![Placeholder image](https://placehold.it/800x400 "Placeholder image")

![Image with caption](https://placehold.it/700x400 "Image with caption")
_This is an image with a caption_
{% endhighlight %}

![Placeholder image](https://placehold.it/800x400 "Placeholder image")

![Image with caption](https://placehold.it/700x400 "Image with caption")
_This is an image with a caption_

# Code and Syntax Highlighting

Use back-ticks for `inline code`. Multi-line code snippets are supported too through Pygments.

{% highlight js %}
// Sample javascript code
var s = "JavaScript syntax highlighting";
alert(s);
{% endhighlight %}

{% highlight python %}

# Sample python code

s = "Python syntax highlighting"
print s
{% endhighlight %}

Adding `linenos` to the highlight tag enables line numbers.

{% highlight js  linenos %}
// Sample javascript code
var s = "JavaScript syntax highlighting";
alert(s);
{% endhighlight %}

# Blockquotes

{% highlight markdown %}

> Curabitur blandit tempus porttitor. Nullam quis risus eget urna mollis ornare vel eu leo. Nullam id dolor id nibh ultricies vehicula ut id elit.

{% endhighlight %}

> Curabitur blandit tempus porttitor. Nullam quis risus eget urna mollis ornare vel eu leo. Nullam id dolor id nibh ultricies vehicula ut id elit.

# Horizontal Rule & Line Break

{% highlight markdown %}
Use `<hr>` for horizontal rules

<hr>

and `<br>` for line breaks.

<br>
{% endhighlight %}

Use `<hr>` for horizontal rules

<hr>

and `<br>` for line breaks.

<br>

_The end_
