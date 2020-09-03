+++
title = "How To Fold Text In Ox-Hugo Quick and Easy"
author = ["santi"]
date = 2020-08-07
tags = ["hugo", "web-design"]
draft = false
weight = 1005
+++

Recently I learned how to write HTML code inside of ox-hugo thanks to this amazing [short blog-post](~/Zotero/storage/289Z3CW7/hugo-raw-html-shortcode.html).

This feature seems to work natively inside of ox-hugo without the need to put it in an HTML block.

This should work just as well for regular HTML, as well as regular Hugo, this is not a special feature of ox-hugo, but it works great in it and that's where I'm using it.


## What It Looks Like {#what-it-looks-like}

<details>
<summary>Click Here To Expand</summary>

This is really useful for times when you want to write about something optional for your audience to read, without interrupting the flow of the blog-post.

It can also be used for adding long code.

Or in any other creative way you can think of.
 </details>


## How to Do it. {#how-to-do-it-dot}

Create an opening "details" tag like so:

```nil
<details>
```

Define the text you want it to show with "summary" tag like so:

```nil
<summary>
```

write what you want to display as a folding title and then close the "summary" tag.

```nil
</summary>
```

Insert all the text you want to insert.

And then close the "details" tag.

```nil
</details>
```


## This Is How The Code Would Look Like {#this-is-how-the-code-would-look-like}

```nil
 <details>
 <summary>Write What You Want To Display Here</summary>
The content you want to unfold goes in here.
 </details>
```


## And This Is What It Would Look Like For The User {#and-this-is-what-it-would-look-like-for-the-user}

<details>
<summary>Write What You Want To Display Here</summary>

The content you want to unfold goes in here.
 </details>

Of course you get the benefits of using this feature when the content inside of it is longer and worth unfolding.

The following is [Hipster Ipsum](https://hipsum.co) it's like Lorem Ipsum but hipster, unfold at your own risk!
<details>
<summary>Hipster Ipsum</summary>

Fanny pack squid ramps, hammock blog 90's portland shaman poutine shabby chic craft beer.

Activated charcoal taxidermy pork belly chia godard pickled franzen unicorn bushwick adaptogen flannel sriracha.

Copper mug pop-up chicharrones umami, woke godard shaman four dollar toast art party twee PBR&B knausgaard yuccie post-ironic.

Truffaut chambray vape, sriracha cred man braid sartorial live-edge direct trade. Squid woke hoodie letterpress normcore biodiesel.
   </details>

That's all folks, hope you found this helpful.
