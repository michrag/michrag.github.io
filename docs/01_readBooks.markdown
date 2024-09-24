---
layout: page
title: Read Books
permalink: /readbooks/
---

<a id="top"></a>
# A selection of books I have read / studied about software / computer science and related topics

I use the app <a href="https://www.bookshelfapp.info/" target="_blank">Bookshelf</a> (Android version) to keep a database of my books, and the tables below have been generated with the "export to html" feature of Bookshelf: it's a very well crafted software, I highly recommend it (I have no affiliation with it).

* TOC
{:toc}

## Programming Languages

<iframe id="programmingIframe" src="/html/Programming.html" width="100%" frameborder="0"></iframe>

[Back to Top](#top)

[//]: # (This may be the most platform independent comment: <br> is a vertical space)
<br>

## Software Development

<iframe id="softwareIframe" src="/html/Software.html" width="100%" frameborder="0"></iframe>

[Back to Top](#top)

[//]: # (This may be the most platform independent comment: <br> is a vertical space)
<br>

## Unix & Linux

<iframe id="unixIframe" src="/html/UnixLinux.html" width="100%" frameborder="0"></iframe>

[Back to Top](#top)

[//]: # (This may be the most platform independent comment: <br> is a vertical space)
<br>

## University Textbooks

<iframe id="universityIframe" src="/html/University.html" width="100%" frameborder="0"></iframe>

[Back to Top](#top)


<script>
  function resizeIframes() {
    var iframes = document.querySelectorAll('iframe');
    iframes.forEach(function(iframe) {
      var documentElement = iframe.contentWindow.document.documentElement;
      var body = iframe.contentWindow.document.body;
      
      var newHeight = Math.max(body.scrollHeight, documentElement.scrollHeight);
      iframe.style.height = newHeight + 'px';
    });
  }

  window.addEventListener('resize', resizeIframes);

  document.querySelectorAll('iframe').forEach(function(iframe) {
    iframe.onload = resizeIframes;
  });
</script>
