---
title:  "Algebra II Unit 1"
mathjax: true
layout: post
categories: media
---

## 1.2 Expressions

#### Variable:
Letters used to represent unknown quantities.

#### Constant:
A number on its own.

#### Coefficient:
A number used to multiply a variable.

#### Term:
The monomials that make up a polynomial.

#### Expression:
A mathematical statement that contains at least one variable.

#### Equation:
A mathematical sentence stating that two expressions are equal.

### Example 1

m+(n-1)^2 if m = 3 and n = -4

-> 3+(-4-1)^2

-> 3+(-5)^2

-> 3+25 = 28

---

## Properties

| Property         | Addition         | Multiplication  |
|------------------|------------------|-----------------|
| Commutative      | a+b=b+a          | ab=ba           |
| Associate        | (a+6)+c=a+(6+c)  | (ab)c=a(bc)     |
| Identity         | a+0=a            | a1=a            |
| Inverse          | a+(-a)=0         | a * 1/2 = 1     |
| Distributive     | a+(b+c)=ab+ac    | (b+c)a=ba+ca    |



## 1.3 Equations

Embed code by putting `{{ "{% highlight language " }}%}` `{{ "{% endhighlight " }}%}` blocks around it. Adding the parameter `linenos` will show source lines besides the code.

{% highlight c %}

static void asyncEnabled(Dict* args, void* vAdmin, String* txid, struct Allocator* requestAlloc)
{
    struct Admin* admin = Identity_check((struct Admin*) vAdmin);
    int64_t enabled = admin->asyncEnabled;
    Dict d = Dict_CONST(String_CONST("asyncEnabled"), Int_OBJ(enabled), NULL);
    Admin_sendMessage(&d, txid, admin);
}

{% endhighlight %}

## 1.4 Solving Absolute Value Equations

With the `jekyll-gist` plugin, which is preinstalled on Github Pages, you can embed gists simply by using the `gist` command:

<script src="https://gist.github.com/5555251.js?file=gist.md"></script>

## Images

Upload an image to the *assets* folder and embed it with `![title](/assets/name.jpg))`. Keep in mind that the path needs to be adjusted if Jekyll is run inside a subfolder.

A wrapper `div` with the class `large` can be used to increase the width of an image or iframe.

![Flower](https://user-images.githubusercontent.com/4943215/55412447-bcdb6c80-5567-11e9-8d12-b1e35fd5e50c.jpg)

[Flower](https://unsplash.com/photos/iGrsa9rL11o) by Tj Holowaychuk

## Embedded content

You can also embed a lot of stuff, for example from YouTube, using the `embed.html` include.

{% include embed.html url="https://www.youtube.com/embed/_C0A5zX-iqM" %}
