---
layout: post
title: How I Build This Site
author: Rangsiman Ketkaew
date: "2019-07-26 01:29:00 +0700"
category:
  - HTML
  - web-development
summary: Example of style code I use to write this site
thumbnail: posts/html.png
permalink: content/6
comments: true
---

<br>

<h1 class="card-title">How I Build This Site</h1>
  <br>
  <h3><a id="Platform_and_Service_12"></a>Platform and Service</h3>
  <ul>
    <li>Github</li>
    <li>Jekyll</li>
    <li>Disqus</li>
    <li>MailChimp</li>
    <li>MakerWidget</li>
  </ul>
  <h3><a id="Programming_language_20"></a>Programming language</h3>
  <ul>
    <li>Markdown</li>
    <li>Ruby/Gem</li>
    <li>HTML/CSS</li>
    <li>Python</li>
    <li>IPython notebook</li>
  </ul>
  <h3><a id="IDE_and_extensions_28"></a>IDE and extensions</h3>
  <ul>
    <li>
      Visual Studio Code
      <ul>
        <li>Markdown All in one</li>
        <li>Markdown Shortcuts</li>
        <li>markdownlint</li>
        <li>Live Server</li>
        <li>Live Server Preview</li>
        <li>File Utils</li>
        <li>Auto Close Tag</li>
        <li>Auto Rename Tag</li>
        <li>Bracket Pair Colorizer</li>
      </ul>
    </li>
    <li>
      Vi/Vim
      <ul>
        <li>NERDTree</li>
      </ul>
    </li>
  </ul>
  <h3><a id="Other_tools_43"></a>Other tools</h3>
  <ul>
    <li>Jupyter Notebook</li>
    <li>Jupyter Book</li>
    <li><a href="https://nbviewer.jupyter.org/">nbviewer</a></li>
  </ul>
  <h3><a id="Jupyter_commandline_49"></a>Jupyter command-line</h3>
  <ul>
    <li>Merge multiple .ipynb files into one file</li>
  </ul>
  <pre><code>pip install nbmerge
</code></pre>
  <ul>
    <li>Convert .ipynb to .html (by default)</li>
  </ul>
  <pre><code>jupyter nbconvert NOTEBOOK.ipynb
</code></pre>
  <ul>
    <li>Convert .ipynb to .html (by default)</li>
  </ul>
  <pre><code>jupyter nbconvert NOTEBOOK.ipynb --to html
</code></pre>
  <ul>
    <li>Execute notebook and replace file</li>
  </ul>
  <pre><code>jupyter nbconvert NOTEBOOK.ipynb --execute
</code></pre>
  <ul>
    <li>Execute notebook and save as .html file</li>
  </ul>
  <pre><code>jupyter nbconvert NOTEBOOK.ipynb --execute --to html
</code></pre>
  <h3><a id="Convert_md_to_html_81"></a>Convert .md to .html</h3>
  <ul>
    <li>Use markdown2</li>
  </ul>
  <pre><code>pip install markdown2
</code></pre>
  <ul>
    <li>Use markdown-to-html</li>
  </ul>
  <p>
    <a href="https://www.npmjs.com/package/markdown-to-html"
      >https://www.npmjs.com/package/markdown-to-html</a
    >
  </p>
  <ul>
    <li>Use pandoc</li>
  </ul>
  <p>
    <a href="https://www.npmjs.com/package/markdown-to-html"
      >https://pandoc.org/getting-started.html</a
    >
  </p>

  <hr />

  ### HTML in Markdown

  <img src="/assets/img/test-and-wow.jpg" width="100%" height="auto" />

  <p>
    Lets try the different text styles <b> Bold </b> ,
    <strong> Strong </strong>, <em> Emphasis </em>, <i> Italic </i>
  </p>

  <p>Now, lets try different heading styles :</p>

  <code class="inlinecode"><h1>Hello in h1 !</h1></code>

  <h1>Hello in h1 !</h1>
  <code class="inlinecode"><h2>Hello in h2 !</h2></code>
  <h2>Hello in h2 !</h2>
  <code class="inlinecode"><h3>Hello in h3 !</h3></code>
  <h3>Hello in h3 !</h3>
  <code class="inlinecode"><h4>Hello in h4 !</h4></code>
  <h4>Hello in h4 !</h4>
  <code class="inlinecode"><h5>Hello in h5 !</h5></code>
  <h5>Hello in h5 !</h5>
  <code class="inlinecode"><h6>Hello in h6 !</h6></code>
  <h6>Hello in h6 !</h6>
  <code class="inlinecode"><h6 align="left">Hello in h6 at left !</h6></code>
  <h6 align="left">Hello in h6 at left !</h6>
  <code class="inlinecode"
    ><h6 align="center">Hello in h6 at center !</h6></code
  >
  <h6 align="center">Hello in h6 at center !</h6>
  <code class="inlinecode"><h6 align="right">Hello in h6 at right !</h6></code>
  <h6 align="right">Hello in h6 at right !</h6>

  <hr />

  <blockquote>
    <p>This is a Block Quote, It can Expand Multiple Lines</p>
  </blockquote>

  <p>You can use the mark tag to <mark>highlight</mark> text.</p>

  <p><del> This line of text is meant to be deleted text </del></p>

  <p><u>This line of text will render as underlined</u></p>
  <p><small>This line of text is meant to be treated as fine print.</small></p>
  <p><strong>This line rendered as bold text.</strong></p>
  <p><em>This line rendered as italicized text.</em></p>
  <p><abbr title="attribute">attr</abbr></p>
  <p><abbr title="HyperText Markup Language" class="initialism">HTML</abbr></p>

  <hr />
  >

  <p>Unordered List</p>

  <ul>
    <li>List Item 1</li>
    <li>List Item 2</li>
    <li>List Item 3</li>
    <li>List Item 4</li>
    <li>List Item 5</li>
  </ul>

  <p>Ordered List</p>
  <ol>
    <li>List Item 1</li>
    <li>List Item 2</li>
    <li>List Item 3</li>
    <li>List Item 4</li>
    <li>List Item 5</li>
  </ol>

  <hr />

  <div class="responsive-table">
    <table>
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">1</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
        <tr>
          <th scope="row">2</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
        <tr>
          <th scope="row">3</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
      </tbody>
    </table>
  </div>

  <hr />

  <h3 id="syntax-highlighting">Syntax Highlighting</h3>

  <p>
    You can add inline code just like this using &lt;code&gt;, e.g.
    <code class="inlinecode">i am code</code>
  </p>

  <p>This is block code using &lt;pre&gt;&lt;code&gt;.</p>
  <pre><code>&lt;pre&gt;&lt;code&gt;
function Panel(element, canClose, closeHandler) {
  this.element = element;
  this.canClose = canClose;
  this.closeHandler = function () { if (closeHandler) closeHandler() };
&lt;/pre&gt;&lt;/code&gt;
</code></pre>

  <pre><code>&lt;pre&gt;&lt;code&gt;
This line is so longggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggggg.
&lt;/pre&gt;&lt;/code&gt;
</code></pre>

  <hr />

  <h3 id="github-gist-embed">GitHub gist Embed</h3>

  <script src="https://gist.github.com/ahmadajmi/dbb4f713317721668bcbc39420562afc.js"></script>

  <hr />

  <h3>YouTube Responsive Embed</h3>

  <iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/nuwjUZCSB2Y?rel=0&amp;controls=0&amp;showinfo=0"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen=""
  ></iframe>

  <hr />

  <h3>Vimeo Responsive Embed</h3>

  <iframe
    src="https://player.vimeo.com/video/212114694?title=0&amp;byline=0&amp;portrait=0"
    width="640"
    height="360"
    frameborder="0"
    webkitallowfullscreen=""
    mozallowfullscreen=""
    allowfullscreen=""
  ></iframe>

  <hr />

  <h3 id="ted-responsive-embed">TED Responsive Embed</h3>

  <iframe
    src="https://embed.ted.com/talks/ted_halstead_a_climate_solution_where_all_sides_can_win"
    width="640"
    height="360"
    frameborder="0"
    scrolling="no"
    allowfullscreen=""
  ></iframe>

  <hr />

  <h3 id="twitch-responsive-embed">Twitch Responsive Embed</h3>

  <iframe
    src="https://player.twitch.tv/?autoplay=false&amp;video=v248755437"
    frameborder="0"
    allowfullscreen="true"
    scrolling="no"
    height="378"
    width="620"
  ></iframe>

  <hr />

  <h3 id="soundcloud-embed">SoundCloud Embed</h3>

  <iframe
    width="100%"
    height="166"
    scrolling="no"
    frameborder="no"
    src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/29738591&amp;color=ff5500&amp;auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false"
  ></iframe>

  <hr />

  <h3 id="codepen-embed">CodePen Embed</h3>

  <p
    data-height="265"
    data-theme-id="light"
    data-slug-hash="YWvpRo"
    data-default-tab="css,result"
    data-user="kharrop"
    data-embed-version="2"
    data-pen-title="Referral Form"
    class="codepen"
  ></p>
  <script
    async=""
    src="https://production-assets.codepen.io/assets/embed/ei.js"
  ></script>

  <hr />

  <h3 id="input-style">Input Style</h3>

  <p><input type="text" placeholder="I'm an input field!" /></p>

  <hr />

  <h3>Twitter Embed</h3>

  <blockquote class="twitter-tweet" data-lang="en">
    <p lang="en" dir="ltr">
      I just published “Deploying a blog using Jekyll and Github Pages with SSL
      certificate for Free”
      <a href="https://t.co/B3T3IQVU93">https://t.co/B3T3IQVU93</a>
    </p>
    &mdash; Sujay Kundu (@SujayKundu777)
    <a
      href="https://twitter.com/SujayKundu777/status/1012601950469160962?ref_src=twsrc%5Etfw"
      >June 29, 2018</a
    >
  </blockquote>
  <script
    async
    src="https://platform.twitter.com/widgets.js"
    charset="utf-8"
  ></script>

  <hr />

  <h3>Instagram Embed</h3>

  <blockquote
    class="instagram-media"
    data-instgrm-permalink="https://www.instagram.com/p/BhFTg6uhNRi/"
    data-instgrm-version="9"
    style=" background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin: 1px; max-width:658px; min-width:326px; padding:0; width:99.375%; width:-webkit-calc(100% - 2px); width:calc(100% - 2px);"
  >
    <div style="padding:8px;">
      <div
        style=" background:#F8F8F8; line-height:0; margin-top:40px; padding:50.0% 0; text-align:center; width:100%;"
      >
        <div
          style=" background:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAsCAMAAAApWqozAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAAAMUExURczMzPf399fX1+bm5mzY9AMAAADiSURBVDjLvZXbEsMgCES5/P8/t9FuRVCRmU73JWlzosgSIIZURCjo/ad+EQJJB4Hv8BFt+IDpQoCx1wjOSBFhh2XssxEIYn3ulI/6MNReE07UIWJEv8UEOWDS88LY97kqyTliJKKtuYBbruAyVh5wOHiXmpi5we58Ek028czwyuQdLKPG1Bkb4NnM+VeAnfHqn1k4+GPT6uGQcvu2h2OVuIf/gWUFyy8OWEpdyZSa3aVCqpVoVvzZZ2VTnn2wU8qzVjDDetO90GSy9mVLqtgYSy231MxrY6I2gGqjrTY0L8fxCxfCBbhWrsYYAAAAAElFTkSuQmCC); display:block; height:44px; margin:0 auto -44px; position:relative; top:-22px; width:44px;"
        ></div>
      </div>
      <p
        style=" color:#c9c8cd; font-family:Arial,sans-serif; font-size:14px; line-height:17px; margin-bottom:0; margin-top:8px; overflow:hidden; padding:8px 0 7px; text-align:center; text-overflow:ellipsis; white-space:nowrap;"
      >
        <a
          href="https://www.instagram.com/p/BhFTg6uhNRi/"
          style=" color:#c9c8cd; font-family:Arial,sans-serif; font-size:14px; font-style:normal; font-weight:normal; line-height:17px; text-decoration:none;"
          target="_blank"
          >A post shared by Ahmad Ajmi (@ahmadajme)</a
        >
        on
        <time
          style=" font-family:Arial,sans-serif; font-size:14px; line-height:17px;"
          datetime="2018-04-02T21:18:58+00:00"
          >Apr 2, 2018 at 2:18pm PDT</time
        >
      </p>
    </div>
  </blockquote>
  <script async defer src="//www.instagram.com/embed.js"></script>

  <br />

  <h3>Embedding PDF</h3>
  
  <h4>PDFObject</h4>

  <div id="pdf1"></div>

  <script src="/jv/pdfobject.js"></script>
  <script>
    PDFObject.embed("/sample/sample.pdf", "#pdf1");
  </script>

  <style>
    .pdfobject-container {
      height: 30rem;
      border: 1rem solid rgba(0, 0, 0, 0.1);
    }
  </style>

  <br />

  <h4>embed</h4>

  <embed
    src="/sample/sample.pdf"
    type="application/pdf"
    width="100%"
    height="500rem"
  />

  <br />

  <h4>iframe</h4>

  <iframe src="/sample/sample.pdf" width="100%" height="500rem">
    This browser does not support PDFs. Please download the PDF to view it:
    <a href="/sample/sample.pdf">Download PDF</a></iframe
