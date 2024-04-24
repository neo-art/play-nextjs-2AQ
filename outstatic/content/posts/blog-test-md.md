---
title: 'Blog Example with MDX'
excerpt: 'Blog Example with MDX That Comes with Templates'
date:
coverImage: '/images/blog-02-MxND.jpg'
author:
  name: 'Milen'
authorImage: '/images/blog/author-02.jpg'
slug: 'blog-test-md'
status: 'published'
description: ''
publishedAt: '2024-04-24T23:00:18.914Z'
---

## Introduction

This part of the documentation shows you how you can configure a contact form with Tailwind CSS Templates and Bootstrap Templates.

## Using PHP Contact Form:

For Bootstrap templates, we used to provide a PHP script that only can be used for PHP servers,

if `phpmailer` function is up and running smoothly.

Here is how it works: Just **replace the email address with your own** from

```bash
assets->php>contact.php
```

This procedure should work if everything is configured properly on the server side.

## Using FormBold: A universal Form API (Recommended):

[FormBold](https://formbold.com/) is a powerful form API and serverless form backend that works with all hosting, SSG, and frameworks.

We highly recommend, using a serverless end-point ([FormBold](https://formbold.com/)) to make contact form dynamic. Since most users nowadays don't use PHP servers.

Here’s how to connect [FormBold](https://formbold.com/) API with your contact form:

**Step#1**: Create an account on [FormBold](https://formbold.com/) and create a Form.

**Step#2**: Integrate the API into your contact Form using this code. Make sure your Form’s method is set to **POST**

```html
<form action="https://formbold.com/s/unique_form_id" method="POST">
  <input type="email" placeholder="email" name="email" />
  <input type="text" placeholder="subject" name="subject" />
  <textarea name="message" placeholder="message"></textarea>

  <button type="submit">Send Message</button>
</form>
```

You’ll find the `unique_form_id` in the [FormBold](https://formbold.com/) dashboard under \***\*Settings&gt;Integration.\*\***

Copy and paste it to the **action** attribute.

This is just the basic setup, FormBold has a lot of great features like re-captcha for spam protection, and the ability to integrate it with other apps like Webhook, Slack, Notion, and GoogleSheet. Learn more about [FormBold](https://formbold.com/) [here](https://formbold.com/).