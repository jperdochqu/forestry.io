---
title: How do I add a CNAME to my site?
authors: []
publishdate: 2017-12-31 00:00:00 -0400
expirydate: 2030-01-01 00:00:00 -0400
layout: single
date: 2018-01-02 15:23:56 +0000
headline: ''
description: ''
textline: ''
images: []
categories: []
tags: []
cta:
  headline: ''
  textline: ''
  calls_to_action: []
private: false
weight: ''
aliases:
- /faq/use-a-cname-for-you-hugo-and-github-pages-site/
menu:
  troubleshooting:
    parent: troubleshooting
---
For some hosting providers (such as GitHub pages) you will need to place a `CNAME` file in the root of your site.

You'll need to ensure that the CNAME file is treated as a [static file](/docs/faqs/static-files), so that it is copied to the root of your site during the build.

{{% tip %}}
Make sure you place your `CNAME` file in your source directory, not your build directory. Otherwise it will be deleted during the next build
{{% /tip %}}

### Examples
- **Jekyll:** any file without [front matter](/docs/faqs/front-matter) is treated as a static file, so place your `CNAME` file in the root of your source folder
- **Hugo**: any file inside of the `static/` directory in your source folder is treated as a static file.