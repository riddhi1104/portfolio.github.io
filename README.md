<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:version='2' class='v2' expr:dir='data:blog.languageDirection' expr:lang='data:blog.locale' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
  <head>
    <meta expr:content='data:blog.isMobile         ? &quot;width=device-width,initial-scale=1.0,minimum-scale=1.0,maximum-scale=1.0&quot;         : &quot;width=1100&quot;' name='viewport'/>
    <b:include data='blog' name='all-head-content'/>
    <title><data:blog.pageTitle/></title>

    <b:skin><![CDATA[/*
-----------------------------------------------
Blogger Template Style
Name:     Ethereal
Designer: Jason Morrow
URL:      jasonmorrow.etsy.com
----------------------------------------------- */

/* Variable definitions
   ====================
   <Variable name="keycolor" description="Main Color" type="color" default="#000000" value="#000000"/>

   <Group description="Body Text" selector="body">
     <Variable name="body.font" description="Font" type="font"
         default="normal normal 13px Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal normal 13px Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
     <Variable name="body.text.color" description="Text Color" type="color" default="#666666" value="#666666"/>
   </Group>

   <Group description="Background" selector=".body-fauxcolumns-outer">
     <Variable name="body.background.color" description="Outer Background" type="color" default="#fb5e53" value="#fb5e53"/>
     <Variable name="content.background.color" description="Main Background" type="color" default="#ffffff" value="#ffffff"/>
     <Variable name="body.border.color" description="Border Color" type="color" default="#fb5e53" value="#fb5e53"/>
   </Group>

   <Group description="Links" selector=".main-inner">
     <Variable name="link.color" description="Link Color" type="color" default="#2198a6" value="#2198a6"/>
     <Variable name="link.visited.color" description="Visited Color" type="color" default="#4d469c" value="#4d469c"/>
     <Variable name="link.hover.color" description="Hover Color" type="color" default="$(link.color)" value="#2198a6"/>
   </Group>

   <Group description="Blog Title" selector=".header h1">
     <Variable name="header.font" description="Font" type="font"
         default="normal normal 60px Times, 'Times New Roman', FreeSerif, serif" value="normal normal 60px Times, &#39;Times New Roman&#39;, FreeSerif, serif"/>
     <Variable name="header.text.color" description="Text Color" type="color" default="#ff8b8b" value="#ff8b8b"/>
   </Group>

   <Group description="Blog Description" selector=".header .description">
     <Variable name="description.text.color" description="Description Color" type="color"
         default="#666666" value="#666666"/>
   </Group>

   <Group description="Tabs Text" selector=".tabs-inner .widget li a">
     <Variable name="tabs.font" description="Font" type="font"
         default="normal normal 12px Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal normal 12px Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
     <Variable name="tabs.selected.text.color" description="Selected Color" type="color" default="#ffffff" value="#ffffff"/>
     <Variable name="tabs.text.color" description="Text Color" type="color" default="$(body.text.color)" value="#666666"/>
   </Group>

   <Group description="Tabs Background" selector=".tabs-outer .PageList">
     <Variable name="tabs.selected.background.color" description="Selected Color" type="color" default="#ffa183" value="#ffa183"/>
     <Variable name="tabs.background.color" description="Background Color" type="color" default="#ffdfc7" value="#ffdfc7"/>
     <Variable name="tabs.border.bevel.color" description="Bevel Color" type="color" default="#fb5e53" value="#fb5e53"/>
   </Group>

   <Group description="Post Title" selector="h3.post-title, h4, h3.post-title a">
     <Variable name="post.title.font" description="Font" type="font"
         default="normal normal 24px Times, Times New Roman, serif" value="normal normal 24px Times, Times New Roman, serif"/>
     <Variable name="post.title.text.color" description="Text Color" type="color" default="#2198a6" value="#2198a6"/>
   </Group>

   <Group description="Gadget Title" selector="h2">
     <Variable name="widget.title.font" description="Title Font" type="font"
        default="normal bold 12px Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal bold 12px Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
     <Variable name="widget.title.text.color" description="Text Color" type="color" default="$(body.text.color)" value="#666666"/>
     <Variable name="widget.title.border.bevel.color" description="Bevel Color" type="color" default="#dbdbdb" value="#dbdbdb"/>
   </Group>

   <Group description="Accents" selector=".main-inner .widget">
     <Variable name="widget.alternate.text.color" description="Alternate Color" type="color" default="#cccccc" value="#cccccc"/>
     <Variable name="widget.border.bevel.color" description="Bevel Color" type="color" default="#dbdbdb" value="#dbdbdb"/>
   </Group>

   <Variable name="body.background" description="Body Background" type="background"
       color="$(body.background.color)" default="$(color) none repeat-x scroll top left" value="#fb5e53 url(https://resources.blogblog.com/blogblog/data/1kt/ethereal/birds-2toned-bg.png) repeat-x scroll top center"/>
   <Variable name="body.background.gradient" description="Body Gradient Cap" type="url"
       default="none" value="none"/>
   <Variable name="body.background.imageBorder" description="Body Image Border" type="url"
       default="none" value="url(//themes.googleusercontent.com/image?id=0BwVBOzw_-hbMNjViMzQ0ZDEtMWU1NS00ZTBkLWFjY2EtZjM5YmU4OTA2MjBm)"/>
   <Variable name="body.background.imageBorder.position.left" description="Body Image Border Left" type="length"
       default="0" min="0" max="400px" value="300px"/>
   <Variable name="body.background.imageBorder.position.right" description="Body Image Border Right" type="length"
       default="0" min="0" max="400px" value="299px"/>
   <Variable name="header.background.gradient" description="Header Background Gradient" type="url" default="none" value="none"/>
   <Variable name="content.background.gradient" description="Content Gradient" type="url" default="none" value="url(https://resources.blogblog.com/blogblog/data/1kt/ethereal/bird-2toned-blue-fade.png)"/>

   <Variable name="link.decoration" description="Link Decoration" type="string" default="none" value="none"/>
   <Variable name="link.visited.decoration" description="Link Visited Decoration" type="string" default="$(link.decoration)" value="none"/>
   <Variable name="link.hover.decoration" description="Link Hover Decoration" type="string" default="underline" value="underline"/>

   <Variable name="widget.padding.top" description="Widget Padding Top" type="length" default="15px" min="0" max="100px" value="15px"/>

   <Variable name="date.space" description="Date Space" type="length" default="15px" min="0" max="100px" value="15px"/>

   <Variable name="post.first.padding.top" description="First Post Padding Top" type="length" default="0" min="0" max="100px" value="0"/>

   <Variable name="mobile.background.overlay" description="Mobile Background Overlay" type="string" default="" value=""/>
   <Variable name="mobile.background.size" description="Mobile Background Size" type="string" default="auto" value="auto"/>

   <Variable name="startSide" description="Side where text starts in blog language" type="automatic" default="left"/>
   <Variable name="endSide" description="Side where text ends in blog language" type="automatic" default="right"/>
*/

/* Content
----------------------------------------------- */
body {
  font: $(body.font);
  color: $(body.text.color);
  background: $(body.background);
}

html body .content-outer {
  min-width: 0;
  max-width: 100%;
  width: 100%;
}

a:link {
  text-decoration: $(link.decoration);
  color: $(link.color);
}

a:visited {
  text-decoration: $(link.visited.decoration);
  color: $(link.visited.color);
}

a:hover {
  text-decoration: $(link.hover.decoration);
  color: $(link.hover.color);
}

.main-inner {
  padding-top: $(date.space);
}

.body-fauxcolumn-outer {
  background: transparent $(body.background.gradient) repeat-x scroll top center;
}

.content-fauxcolumns .fauxcolumn-inner {
  background: $(content.background.color) $(content.background.gradient) repeat-x scroll top left;
  border-left: 1px solid $(body.border.color);
  border-right: 1px solid $(body.border.color);
}

/* Flexible Background
----------------------------------------------- */
.content-fauxcolumn-outer .fauxborder-left {
  width: 100%;
  padding-left: $(body.background.imageBorder.position.left);
  margin-left: -$(body.background.imageBorder.position.left);
  background-color: transparent;
  background-image: $(body.background.imageBorder);
  background-repeat: no-repeat;
  background-position: left top;
}


.content-fauxcolumn-outer .fauxborder-right {
  margin-right: -$(body.background.imageBorder.position.right);
  width: $(body.background.imageBorder.position.right);
  background-color: transparent;
  background-image: $(body.background.imageBorder);
  background-repeat: no-repeat;
  background-position: right top;
}


/* Columns
----------------------------------------------- */

.content-inner {
  padding: 0;
}

/* Header
----------------------------------------------- */
.header-inner {
  padding: 27px 0 3px;
}

.header-inner .section {
  margin: 0 35px;
}

.Header h1 {
  font: $(header.font);
  color: $(header.text.color);
}

.Header h1 a {
  color: $(header.text.color);
}

.Header .description {
  font-size: 115%;
  color: $(description.text.color);
}

.header-inner .Header .titlewrapper,
.header-inner .Header .descriptionwrapper {
  padding-left: 0;
  padding-right: 0;
  margin-bottom: 0;
}

/* Tabs
----------------------------------------------- */
.tabs-outer {
  position: relative;
  background: transparent;
}

.tabs-cap-top, .tabs-cap-bottom {
  position: absolute;
  width: 100%;
}

.tabs-cap-bottom {
  bottom: 0;
}

.tabs-inner {
  padding: 0;
}

.tabs-inner .section {
  margin: 0 35px;
}

*+html body .tabs-inner .widget li {
  padding: 1px;
}

.PageList {
  border-bottom: 1px solid $(tabs.border.bevel.color);
}

.tabs-inner .widget li.selected a,
.tabs-inner .widget li a:hover {
  position: relative;
  -moz-border-radius-topleft: 5px;
  -moz-border-radius-topright: 5px;
  -webkit-border-top-left-radius: 5px;
  -webkit-border-top-right-radius: 5px;
  -goog-ms-border-top-left-radius: 5px;
  -goog-ms-border-top-right-radius: 5px;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;

  background: $(tabs.selected.background.color) none ;
  color: $(tabs.selected.text.color);
}

.tabs-inner .widget li a {
  display: inline-block;
  margin: 0;
  margin-right: 1px;
  padding: .65em 1.5em;
  font: $(tabs.font);
  color: $(tabs.text.color);
  background-color: $(tabs.background.color);

  -moz-border-radius-topleft: 5px;
  -moz-border-radius-topright: 5px;
  -webkit-border-top-left-radius: 5px;
  -webkit-border-top-right-radius: 5px;
  -goog-ms-border-top-left-radius: 5px;
  -goog-ms-border-top-right-radius: 5px;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}

/* Headings
----------------------------------------------- */
h2 {
  font: $(widget.title.font);
  color: $(widget.title.text.color);
}

/* Widgets
----------------------------------------------- */
.main-inner .column-left-inner {
  padding: 0 0 0 20px;
}

.main-inner .column-left-inner .section {
  margin-right: 0;
}

.main-inner .column-right-inner {
  padding: 0 20px 0 0;
}

.main-inner .column-right-inner .section {
  margin-left: 0;
}

.main-inner .section {
  padding: 0;
}

.main-inner .widget {
  padding: 0 0 15px;
  margin: 20px 0;
  border-bottom: 1px solid $(widget.border.bevel.color);
}

.main-inner .widget h2 {
  margin: 0;
  padding: .6em 0 .5em;
}

.footer-inner .widget h2 {
  padding: 0 0 .4em;
}

.main-inner .widget h2 + div, .footer-inner .widget h2 + div {
  padding-top: $(widget.padding.top);
}

.main-inner .widget .widget-content {
  margin: 0;
  padding: 15px 0 0;
}

.main-inner .widget ul, .main-inner .widget #ArchiveList ul.flat {
  margin: -$(widget.padding.top) -15px -15px;
  padding: 0;

  list-style: none;
}

.main-inner .sidebar .widget h2 {
  border-bottom: 1px solid $(widget.title.border.bevel.color);
}

.main-inner .widget #ArchiveList {
  margin: -$(widget.padding.top) 0 0;
}

.main-inner .widget ul li, .main-inner .widget #ArchiveList ul.flat li {
  padding: .5em 15px;
  text-indent: 0;
}

.main-inner .widget #ArchiveList ul li {
  padding-top: .25em;
  padding-bottom: .25em;
}

.main-inner .widget ul li:first-child, .main-inner .widget #ArchiveList ul.flat li:first-child {
  border-top: none;
}

.main-inner .widget ul li:last-child, .main-inner .widget #ArchiveList ul.flat li:last-child {
  border-bottom: none;
}

.main-inner .widget .post-body ul {
  padding: 0 2.5em;
  margin: .5em 0;

  list-style: disc;
}

.main-inner .widget .post-body ul li {
  padding: 0.25em 0;
  margin-bottom: .25em;
  color: $(body.text.color);
  border: none;
}

.footer-inner .widget ul {
  padding: 0;

  list-style: none;
}

.widget .zippy {
  color: $(widget.alternate.text.color);
}

/* Posts
----------------------------------------------- */
.main.section {
  margin: 0 20px;
}

body .main-inner .Blog {
  padding: 0;
  background-color: transparent;
  border: none;
}

.main-inner .widget h2.date-header {
  border-bottom: 1px solid $(widget.title.border.bevel.color);
}

.date-outer {
  position: relative;
  margin: $(date.space) 0 20px;
}

.date-outer:first-child {
  margin-top: 0;
}

.date-posts {
  clear: both;
}

.post-outer, .inline-ad {
  border-bottom: 1px solid $(widget.border.bevel.color);
  padding: 30px 0;
}

.post-outer {
  padding-bottom: 10px;
}

.post-outer:first-child {
  padding-top: $(post.first.padding.top);
  border-top: none;
}

.post-outer:last-child, .inline-ad:last-child {
  border-bottom: none;
}

.post-body img {
  padding: 8px;
}

h3.post-title, h4 {
  font: $(post.title.font);
  color: $(post.title.text.color);
}

h3.post-title a {
  font: $(post.title.font);
  color: $(post.title.text.color);
  text-decoration: none;
}

h3.post-title a:hover {
  color: $(link.hover.color);
  text-decoration: underline;
}

.post-header {
  margin: 0 0 1.5em;
}

.post-body {
  line-height: 1.4;
}

.post-footer {
  margin: 1.5em 0 0;
}

#blog-pager {
  padding: 15px;
}

.blog-feeds, .post-feeds {
  margin: 1em 0;
  text-align: center;
}

.post-outer .comments {
  margin-top: 2em;
}

/* Comments
----------------------------------------------- */
.comments .comments-content .icon.blog-author {
  background-repeat: no-repeat;
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAYAAABWzo5XAAAAAXNSR0IArs4c6QAAAAZiS0dEAP8A/wD/oL2nkwAAAAlwSFlzAAALEgAACxIB0t1+/AAAAAd0SU1FB9sLFwMeCjjhcOMAAAD+SURBVDjLtZSvTgNBEIe/WRRnm3U8RC1neQdsm1zSBIU9VVF1FkUguQQsD9ITmD7ECZIJSE4OZo9stoVjC/zc7ky+zH9hXwVwDpTAWWLrgS3QAe8AZgaAJI5zYAmc8r0G4AHYHQKVwII8PZrZFsBFkeRCABYiMh9BRUhnSkPTNCtVXYXURi1FpBDgArj8QU1eVXUzfnjv7yP7kwu1mYrkWlU33vs1QNu2qU8pwN0UpKoqokjWwCztrMuBhEhmh8bD5UDqur75asbcX0BGUB9/HAMB+r32hznJgXy2v0sGLBcyAJ1EK3LFcbo1s91JeLwAbwGYu7TP/3ZGfnXYPgAVNngtqatUNgAAAABJRU5ErkJggg==);
}

.comments .comments-content .loadmore a {
  background: $(content.background.color) $(content.background.gradient) repeat-x scroll top left;
}

.comments .comments-content .loadmore a {
  border-top: 1px solid $(widget.title.border.bevel.color);
  border-bottom: 1px solid $(widget.title.border.bevel.color);
}

.comments .comment-thread.inline-thread {
  background: $(content.background.color) $(content.background.gradient) repeat-x scroll top left;
}

.comments .continue {
  border-top: 2px solid $(widget.title.border.bevel.color);
}

/* Footer
----------------------------------------------- */
.footer-inner {
  padding: 30px 0;
  overflow: hidden;
}

/* Mobile
----------------------------------------------- */
body.mobile  {
  background-size: $(mobile.background.size)
}

.mobile .body-fauxcolumn-outer {
  background: $(mobile.background.overlay);
}

.mobile .content-fauxcolumns .fauxcolumn-inner {
  opacity: 0.75;
}

.mobile .content-fauxcolumn-outer .fauxborder-right {
  margin-right: 0;
}

.mobile-link-button {
  background-color: $(tabs.selected.background.color);
}

.mobile-link-button a:link, .mobile-link-button a:visited {
  color: $(tabs.selected.text.color);
}

.mobile-index-contents {
  color: #444444;
}

.mobile .body-fauxcolumn-outer {
  background-size: 100% auto;
}

.mobile .mobile-date-outer {
  border-bottom: transparent;
}

.mobile .PageList {
  border-bottom: none;
}

.mobile .tabs-inner .section {
  margin: 0;
}

.mobile .tabs-inner .PageList .widget-content {
  background: $(tabs.selected.background.color) none;
  color: $(tabs.selected.text.color);
}

.mobile .tabs-inner .PageList .widget-content .pagelist-arrow {
  border-$startSide: 1px solid $(tabs.selected.text.color);
}

.mobile .footer-inner {
  overflow: visible;
}

body.mobile .AdSense {
  margin: 0 -10px;
}
]]></b:skin>

    <b:template-skin>
      <b:variable default='960px' name='content.width' type='length'/>
      <b:variable default='0' name='main.column.left.width' type='length'/>
      <b:variable default='310px' name='main.column.right.width' type='length'/>

      <![CDATA[
      body {
        min-width: $(content.width);
      }

      .content-outer, .content-fauxcolumn-outer, .region-inner {
        min-width: $(content.width);
        max-width: $(content.width);
        _width: $(content.width);
      }

      .main-inner .columns {
        padding-left: $(main.column.left.width);
        padding-right: $(main.column.right.width);
      }

      .main-inner .fauxcolumn-center-outer {
        left: $(main.column.left.width);
        right: $(main.column.right.width);
        /* IE6 does not respect left and right together */
        _width: expression(this.parentNode.offsetWidth -
            parseInt("$(main.column.left.width)") -
            parseInt("$(main.column.right.width)") + 'px');
      }

      .main-inner .fauxcolumn-left-outer {
        width: $(main.column.left.width);
      }

      .main-inner .fauxcolumn-right-outer {
        width: $(main.column.right.width);
      }

      .main-inner .column-left-outer {
        width: $(main.column.left.width);
        right: 100%;
        margin-left: -$(main.column.left.width);
      }

      .main-inner .column-right-outer {
        width: $(main.column.right.width);
        margin-right: -$(main.column.right.width);
      }

      #layout {
        min-width: 0;
      }

      #layout .content-outer {
        min-width: 0;
        width: 800px;
      }

      #layout .region-inner {
        min-width: 0;
        width: auto;
      }

      body#layout div.add_widget {
        padding: 8px;
      }

      body#layout div.add_widget a {
        margin-left: 32px;
      }
      ]]>
    </b:template-skin>

    <b:if cond='data:skin.vars.body_background.image.isResizable'>
      <b:include cond='not data:view.isPreview' data='{                          image: data:skin.vars.body_background.image,                          selector: &quot;body&quot;                        }' name='responsiveImageStyle'/>
    </b:if>

    <b:include data='blog' name='google-analytics'/>
  </head>

  <body expr:class='&quot;loading&quot; + data:blog.mobileClass'>
  <b:section class='navbar' id='navbar' maxwidgets='1' name='Navbar' showaddelement='no'>
    <b:widget id='Navbar1' locked='true' title='Navbar' type='Navbar'>
      <b:includable id='main'>&lt;script type=&quot;text/javascript&quot;&gt;
    function setAttributeOnload(object, attribute, val) {
      if(window.addEventListener) {
        window.addEventListener(&#39;load&#39;,
          function(){ object[attribute] = val; }, false);
      } else {
        window.attachEvent(&#39;onload&#39;, function(){ object[attribute] = val; });
      }
    }
  &lt;/script&gt;
&lt;div id=&quot;navbar-iframe-container&quot;&gt;&lt;/div&gt;
&lt;script type=&quot;text/javascript&quot; src=&quot;https://apis.google.com/js/plusone.js&quot;&gt;&lt;/script&gt;
&lt;script type=&quot;text/javascript&quot;&gt;
      gapi.load(&quot;gapi.iframes:gapi.iframes.style.bubble&quot;, function() {
        if (gapi.iframes &amp;&amp; gapi.iframes.getContext) {
          gapi.iframes.getContext().openChild({
              url: &#39;https://www.blogger.com/navbar.g?targetBlogID\x3d1916471432126489390\x26blogName\x3dHuman+Habits\x26publishMode\x3dPUBLISH_MODE_BLOGSPOT\x26navbarType\x3dLIGHT\x26layoutType\x3dLAYOUTS\x26searchRoot\x3dhttps://aishwaryarajivale123.blogspot.com/search\x26blogLocale\x3den\x26v\x3d2\x26homepageUrl\x3dhttp://aishwaryarajivale123.blogspot.com/\x26vt\x3d-5338652767600162003&#39;,
              where: document.getElementById(&quot;navbar-iframe-container&quot;),
              id: &quot;navbar-iframe&quot;
          });
        }
      });
    &lt;/script&gt;&lt;script type=&quot;text/javascript&quot;&gt;
(function() {
var script = document.createElement(&#39;script&#39;);
script.type = &#39;text/javascript&#39;;
script.src = &#39;//pagead2.googlesyndication.com/pagead/js/google_top_exp.js&#39;;
var head = document.getElementsByTagName(&#39;head&#39;)[0];
if (head) {
head.appendChild(script);
}})();
&lt;/script&gt;
</b:includable>
    </b:widget>
  </b:section>

  <b:if cond='data:blog.pageType == &quot;index&quot;'>
    <div itemscope='itemscope' itemtype='http://schema.org/Blog' style='display: none;'>
      <meta expr:content='data:blog.title' itemprop='name'/>
      <b:if cond='data:blog.metaDescription'>
        <meta expr:content='data:blog.metaDescription' itemprop='description'/>
      </b:if>
    </div>
  </b:if>

  <div class='body-fauxcolumns'>
    <div class='fauxcolumn-outer body-fauxcolumn-outer'>
    <div class='cap-top'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    <div class='fauxborder-left'>
    <div class='fauxborder-right'/>
    <div class='fauxcolumn-inner'>
    </div>
    </div>
    <div class='cap-bottom'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    </div>
  </div>

  <div class='content'>
  <div class='content-fauxcolumns'>
    <div class='fauxcolumn-outer content-fauxcolumn-outer'>
    <div class='cap-top'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    <div class='fauxborder-left'>
    <div class='fauxborder-right'/>
    <div class='fauxcolumn-inner'>
    </div>
    </div>
    <div class='cap-bottom'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    </div>
  </div>

  <div class='content-outer'>
  <div class='content-cap-top cap-top'>
    <div class='cap-left'/>
    <div class='cap-right'/>
  </div>
  <div class='fauxborder-left content-fauxborder-left'>
  <div class='fauxborder-right content-fauxborder-right'/>
  <div class='content-inner'>

    <header>
    <div class='header-outer'>
    <div class='header-cap-top cap-top'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    <div class='fauxborder-left header-fauxborder-left'>
    <div class='fauxborder-right header-fauxborder-right'/>
    <div class='region-inner header-inner'>
      <b:section class='header' id='header' maxwidgets='1' name='Header' showaddelement='no'>
        <b:widget id='Header1' locked='true' title='Human Habits (Header)' type='Header'>
          <b:widget-settings>
            <b:widget-setting name='displayUrl'/>
            <b:widget-setting name='displayHeight'>0</b:widget-setting>
            <b:widget-setting name='sectionWidth'>-1</b:widget-setting>
            <b:widget-setting name='useImage'>false</b:widget-setting>
            <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
            <b:widget-setting name='imagePlacement'>BEHIND</b:widget-setting>
            <b:widget-setting name='displayWidth'>0</b:widget-setting>
          </b:widget-settings>
          <b:includable id='main'>

  <b:if cond='data:useImage'>
    <b:if cond='data:imagePlacement == &quot;BEHIND&quot;'>
      <!--
      Show image as background to text. You can't really calculate the width
      reliably in JS because margins are not taken into account by any of
      clientWidth, offsetWidth or scrollWidth, so we don't force a minimum
      width if the user is using shrink to fit.
      This results in a margin-width's worth of pixels being cropped. If the
      user is not using shrink to fit then we expand the header.
      -->
      <b:if cond='data:mobile'>
        <div id='header-inner'>
          <div class='titlewrapper' style='background: transparent'>
            <h1 class='title' style='background: transparent; border-width: 0px'>
              <b:include name='title'/>
            </h1>
          </div>
          <b:include name='description'/>
        </div>
      <b:else/>
        <div expr:style='&quot;background-image: url(\&quot;&quot; + data:sourceUrl + &quot;\&quot;); &quot;                      + &quot;background-position: &quot;                      + data:backgroundPositionStyleStr + &quot;; &quot;                      + data:widthStyleStr                      + &quot;min-height: &quot; + data:height                      + &quot;_height: &quot; + data:height                      + &quot;background-repeat: no-repeat; &quot;' id='header-inner'>
          <div class='titlewrapper' style='background: transparent'>
            <h1 class='title' style='background: transparent; border-width: 0px'>
              <b:include name='title'/>
            </h1>
          </div>
          <b:include name='description'/>
        </div>
      </b:if>
    <b:else/>
      <!--Show the image only-->
      <div id='header-inner'>
        <a expr:href='data:blog.homepageUrl' style='display: block'>
          <img expr:alt='data:title' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_headerimg&quot;' expr:src='data:sourceUrl' expr:width='data:width' style='display: block'/>
        </a>
        <!--Show the description-->
        <b:if cond='data:imagePlacement == &quot;BEFORE_DESCRIPTION&quot;'>
          <b:include name='description'/>
        </b:if>
      </div>
    </b:if>
  <b:else/>
    <!--No header image -->
    <div id='header-inner'>
      <div class='titlewrapper'>
        <h1 class='title'>
          <b:include name='title'/>
        </h1>
      </div>
      <b:include name='description'/>
    </div>
  </b:if>
</b:includable>
          <b:includable id='description'>
  <div class='descriptionwrapper'>
    <p class='description'><span><data:description/></span></p>
  </div>
</b:includable>
          <b:includable id='title'>
  <b:tag cond='data:blog.url != data:blog.homepageUrl' expr:href='data:blog.homepageUrl' name='a'>
    <data:title/>
  </b:tag>
</b:includable>
        </b:widget>
      </b:section>
    </div>
    </div>
    <div class='header-cap-bottom cap-bottom'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    </div>
    </header>

    <div class='tabs-outer'>
    <div class='tabs-cap-top cap-top'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    <div class='fauxborder-left tabs-fauxborder-left'>
    <div class='fauxborder-right tabs-fauxborder-right'/>
    <div class='region-inner tabs-inner'>
      <b:section class='tabs' id='crosscol' maxwidgets='1' name='Cross-Column' showaddelement='yes'/>
      <b:section class='tabs' id='crosscol-overflow' name='Cross-Column 2' showaddelement='no'/>
    </div>
    </div>
    <div class='tabs-cap-bottom cap-bottom'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    </div>

    <div class='main-outer'>
    <div class='main-cap-top cap-top'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>

    <div class='fauxborder-left main-fauxborder-left'>
    <div class='fauxborder-right main-fauxborder-right'/>
    <div class='region-inner main-inner'>

      <div class='columns fauxcolumns'>

        <div class='fauxcolumn-outer fauxcolumn-center-outer'>
        <div class='cap-top'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
        <div class='fauxborder-left'>
        <div class='fauxborder-right'/>
        <div class='fauxcolumn-inner'>
        </div>
        </div>
        <div class='cap-bottom'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
        </div>

        <div class='fauxcolumn-outer fauxcolumn-left-outer'>
        <div class='cap-top'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
        <div class='fauxborder-left'>
        <div class='fauxborder-right'/>
        <div class='fauxcolumn-inner'>
        </div>
        </div>
        <div class='cap-bottom'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
        </div>

        <div class='fauxcolumn-outer fauxcolumn-right-outer'>
        <div class='cap-top'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
        <div class='fauxborder-left'>
        <div class='fauxborder-right'/>
        <div class='fauxcolumn-inner'>
        </div>
        </div>
        <div class='cap-bottom'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
        </div>

        <!-- corrects IE6 width calculation -->
        <div class='columns-inner'>
