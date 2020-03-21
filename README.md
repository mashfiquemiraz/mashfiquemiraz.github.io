Skip to content
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 
@mashfiquemiraz 
mashfiquemiraz
/
mashfiquemiraz.github.io
Template
0
00
 Code Issues 0 Pull requests 0 Actions Projects 0 Wiki Security Insights Settings
Add files via upload

 master
@mashfiquemiraz
mashfiquemiraz committed 3 minutes ago 
1 parent 01f41e9 commit a8e3a0f9d5f1c2736bc2828a019c50700d2c9375
Showing  with 2,835 additions and 0 deletions.
 2,835  Mashfique's Modded Blogspot.xml 
@@ -0,0 +1,2835 @@
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
  <head>
    <b:include data='blog' name='all-head-content'/>

    <title>
      <b:if cond='data:blog.pageType == &quot;index&quot;'>
        <data:blog.pageTitle/>
        <b:else/>
        <b:if cond='data:blog.pageType != &quot;error_page&quot;'>
          <data:blog.pageName/> | <data:blog.title/>
          <b:else/>
          Page Not Found | <data:blog.title/> 
        </b:if>
      </b:if>
    </title>


    <b:if cond='data:blog.pageType == &quot;archive&quot;'>
      <meta content='noindex,noarchive' name='robots'/>
    </b:if>
    <meta charset='UTF-8'/>
    <meta content='width=device-width, initial-scale=1, maximum-scale=1' name='viewport'/>
<link href='//maxcdn.bootstrapcdn.com/bootstrap/3.3.1/css/bootstrap.min.css' rel='stylesheet' type='text/css'/>
<link href='//maxcdn.bootstrapcdn.com/font-awesome/4.1.0/css/font-awesome.min.css' id='fontawesome' rel='stylesheet' type='text/css'/>
<link href='http://fonts.googleapis.com/css?family=PT+Serif:400,700|Open+Sans:400,600|Rock+Salt|Montserrat:400,700&amp;subset=cyrillic' rel='stylesheet' type='text/css'/>


<b:skin><![CDATA[
*, *:after, *:before {box-sizing: border-box;-webkit-box-sizing: border-box;-moz-box-sizing: border-box;-webkit-font-smoothing: antialiased;font-smoothing: antialiased;text-rendering: optimizeLegibility;}
/*------------------------------------------------------
Variable @ Template Designer
--------------------------------------------------------
------------------------------------------------------*/
/* ------------------------- */
/*		RESET.CSS			 */
/* ------------------------- */
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, font, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td, figure {    margin: 0;    padding: 0;}
article,aside,details,figcaption,figure,
footer,header,hgroup,menu,nav,section {     display:block;}
table {    border-collapse: separate;    border-spacing: 0;}
caption, th, td {    text-align: left;    font-weight: normal;}
blockquote:before, blockquote:after,
q:before, q:after {    content: "";}
blockquote, q {    quotes: "" "";}
sup{    vertical-align: super;    font-size:smaller;}
code{    font-family: 'Courier New', Courier, monospace;    font-size:12px;    color:#272727;}
::selection {  background: #333;  color: #fff;  }
::-moz-selection {  background: #333;  color: #fff;  }
a img{	border: none;vertical-align: middle;}
img{vertical-align: middle;max-width:100%;}
ol, ul { padding: 10px 0 20px;  margin: 0 0 0 35px;  text-align: left;  }
ol li { list-style-type: decimal;  padding:0 0 5px;  }
ul li { list-style-type: square;  padding: 0 0 5px;  }
ul ul, ol ol { padding: 0; }
h1, h2, h3, h4, h5, h6 {  color: #222222 ;font:normal normal 16px Playfair Display, serif; font-weight: normal; }
.post-body h1 { line-height: 48px; font-size: 42px; margin: 10px 0; }
.post-body h2 { font-size: 36px; line-height: 44px; padding-bottom: 5px; margin: 10px 0; }
.post-body h3 { font-size: 32px; line-height: 40px; padding-bottom: 5px; margin: 10px 0; }
.post-body h4 { font-size: 28px; line-height: 36px; margin: 10px 0;  }
.post-body h5 { font-size: 24px; line-height: 30px; margin: 10px 0;  }
.post-body h6 { font-size: 18px; line-height: 24px; margin: 10px 0;  }
/* ------------------------- */
/*		GENERAL				 */
/* ------------------------- */
body{ 
	background: #f3f3f3; 
	color: #555555; 
	padding: 0;
	font : normal normal 14px Open Sans;
	font-size: 15px; 
	line-height: 1.85; 
}
a{ color: #333333; outline:none; text-decoration: none; }
a:hover,a:focus { color: #333; text-decoration:none; }
.clr { clear:both; float:none; }
.clearfix{position:relative;}
.clearfix:after,.clearfix:before{display:table;content:"";line-height:0}
/* ------------------------- */
/*		WRAPPERS			 */
/* ------------------------- */
.ct-wrapper {
    padding: 0px 20px;
    position: relative;
    max-width: 1080px;
    margin: 0 auto;
}
.content-wrapper{ 
    position: relative;
    margin-right: 25px;
	padding-top: 50px;
}
.main-wrapper {
  width: 80%;
  display: table;
  margin: 0 auto;
}
#content { position: relative;margin-right:25px; }
.sidebar-wrapper { display:none;width:30%; float: right; }
.stretched{margin-top:60px;}
/*----------------------------- */
/*	>> BLOG LAYOUT STYLING		*/
/* ---------------------------- */
body#layout .header-wrapper { margin-top: 0px; }
body#layout .outer-wrapper, body#layout .sidebar-wrapper, body#layout .ct-wrapper { margin: 0; padding: 0; }
body#layout #About { width: 100%; }
#layout .blog_share {
display: none;
}
#layout .bg-opacity {
  opacity: 0;
  position: static;
  height: 0;
}
#layout .about_author,#layout .blog_author,#layout .bottom_share,#layout .contact_us,#layout p.attribution{margin:0;margin-top:0;  padding: 0;}
#layout #site-header{height:auto!important;}
#layout .footer_bottom {margin: 0;padding: 0;}
#layout .widget.Header { display: block; }
/*----------------------------- */
/*	>> SITE HEADER				*/
/* ---------------------------- */
#site-header {
	position: relative; 
	overflow: hidden; 
	width: 100%; 
	height: 400px;
}
#site-header:before {
	content: "";
  	width: 100%;
  	height: 100%;
  	background: rgba(0,0,0,.7);
  	position: absolute;
  	top: 0;
  	z-index: 100;
}
/*----------------------------- */
/*	>> HEADER WIDGET			*/
/* ---------------------------- */
#header {
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    z-index: 100;
}
.widget.Header {
    display: table;
    vertical-align: middle;
    height: 100%;
    margin: auto;
}
#header-inner {
    display: table-cell;
    vertical-align: middle;
}
#header h1 { 
  	font: normal normal 70px Rock Salt;
  	font-weight: normal;
  	line-height: 1.5;
  	letter-spacing: 5px;
}
#header h1 a, 
#header h1 a:hover {  color: #eeeeee;  }
#header p.description{ color: #333; font-size: 12px; font-style: italic; text-shadow: 1px 1px #FFFFFF; margin: 0; padding: 0; text-transform:capitalize; }
#header img{   border:0 none; background:none; width:auto; height:auto; margin:0 auto;  max-height:190px;}
a.logo {
  padding: 20px 0;
}
/*----------------------------- */
/*	>> ABOUT AUTHOR				*/
/* ---------------------------- */
.about_author {
    margin-top: -80px;
    z-index: 200;
    position: relative;
}
.blog_author {
    text-align: center;
    margin-bottom: 25px;
}
.author_thumbnail {
    width: 150px;
    margin: 0 auto 10px;
}
.blog_author img {
    border-radius: 50%;
    border: 5px solid transparent;
    background: $(body.background.color);
}
.about_author .detail {
    margin: 0 auto;
    display: inline-block;
    color: #666;
}
.blog_author .detail .name {
  	font-size: 22px;
	margin-bottom: 5px;
}
.blog_author .detail .term {
  	font-size: 14px;
	font-weight:300;
}
/*----------------------------- */
/*	>> NAVIGATION MENU			*/
/* ---------------------------- */
.nav-menu {
    position: absolute;
    top: 40px;
    right: 0;
    left: 0;
	z-index: 100;
}
.nav-menu ul {
    list-style: none;
    margin: 0 auto;
    padding: 0;
    z-index: 999;
    display: table;
}
.nav-menu ul li {
    display: inline-block;
    float: left;
    line-height: 1;
    list-style: none;
    padding: 0;
    margin-right: 15px;
}
.nav-menu li a {
  	color: #eee;
  	display: block;
  	font-size: 12px;
  	font-weight: 300;
  	padding: 5px 15px;
  	position: relative;
  	text-decoration: none;
  	text-transform: uppercase;
  	letter-spacing: 1px;
  	font-family: montserrat,sans-serif;
}
.nav-menu li a:hover { 
	color: #ffffff; 
}
.nav-menu li:first-child a, .nav-menu li a:hover {
  	background: #edc037;
	color: #f3f3f3;
}
/*----------------------------- */
/*	>> BLOG FEATURED POST		*/
/* ---------------------------- */
.featured-slider {
	position: absolute;
	top: 0;
	z-index: -1;
}
.blog_featured_post {
    display: inline-block;
    width: 100%;
    height: 550px;
    display: block;
    position: relative;
    float: left;
    overflow: hidden;
}
.blog_featured_post .feat-img {
    width: 100%!important;
    height: 100%;
    background-size: cover;
    background-position-y: 20%;
    background-repeat: no-repeat;
}
/*----------------------------- */
/*	>> POST & PAGES				*/
/* ---------------------------- */
/* index gallery style */
.blog-posts.hfeed {
width: 100%;
}
.post-outer{
	margin-bottom:30px;
	padding-bottom:30px;
}
.post.hentry {
	height:100%;
	margin: 0;
	overflow: hidden;
}
.post.hentry {
    border-bottom: 2px solid #cccccc;
    padding-bottom: 50px;
}
h2.entry-title, .post-title {
    color: #333333;
	font: normal bold 36px PT Serif;
  	margin: 0 0 15px;
  	padding: 0;
  	text-transform: capitalize;
  	text-align: center;
}
h2.entry-title a, .post-title a{ color: #333333; }
.post-body { 
	font: normal normal 15px Open Sans; 
	color: #666666;
	line-height: 1.75;
	text-transform: auto; 
	word-wrap:break-word;  
}
/* >> POST IMAGE 
/* _____ _____ _____ _____ */
.post-image { 
	margin: 0 0 30px;
}
/* >> POST HEADER 
/* ________ _____ _____ */
.post-header {
    margin: 0 0 20px;
    padding: 0;
    text-align: center;
}
/* >> POST CATEGORY 
/* ____ ____ _____ _____ ____ */
.post-category {
    margin: 0 0 25px;
}
.post-category a:nth-child(n+2) {
    display: none;
}
.post-category a {
    display: inline-block;
    color: #333;
    font-family: Montserrat, sans-serif;
    font-size: 12px;
    font-weight: bold;
    letter-spacing: 0.55px;
    line-height: 20px;
    padding: 0 7px;
    position: relative;
    text-transform: uppercase;
}
/* >> POST META
/* ____ ____ ____ ____ */
.post-meta {
	margin: 0 0 25px;	
}
.post-meta .post-date,
.post-meta .post-author, 
.post-meta .post-comment {
	color: #777;
    display: inline-block;
    font-family: montserrat,sans-serif;
    font-size: 11px;
	letter-spacing: 0.25px;
	margin-left: 10px;
    padding: 0 5px;
    position: relative;
    text-transform: uppercase;
}
.post-meta .post-date {
    padding-right: 15px;
}
.post-meta .post-date:after {
    content: "|";
    position: absolute;
    top: 0;
    right: 0;
}
.post-meta .post-comment { padding-left: 15px; }
.post-meta .post-comment:before {
    content: "|";
    position: absolute;
    top: 0;
    left: 0;
}
/* >> POST CONTENT 
/* ____ ____ ____ ____ */
.post-content {
    letter-spacing: -0.45px;
    line-height: 1.9;
    margin: 0 0 25px;
    padding: 0 15px;
    text-align: center;
}
/* >> POSTE READ MORE
/* _____ ______ _____ _____ */
.post-read-more {
    text-align: center;
}
.post-read-more a {
    color: #777;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 50px;
    font: normal normal 12px Montserrat;
    letter-spacing: .5px;
    line-height: 44px;
    padding: 0 24px;
    text-transform: uppercase;
}
/***** Page Nav CSS *****/
.status-msg-wrap {
  margin-bottom: 30px;
}
#blog-pager {
display: inline-block;
margin: 20px 0 0;
overflow: visible;
padding: 25px 3%;
width: 100%;
}
.showpageOf, .home-link {  display:none;  }
.showpagePoint {  background: #101010;  color: #FFFFFF;  margin: 0 10px 0 0;  padding: 5px 10px;  text-decoration: none;  border-radius: 3px; -moz-border-radius: 3px; -o-border-radius: 3px; -webkit-border-radius: 3px;  }
.showpage a, .showpageNum a { background: transparent; color: #333;border:1px solid #333; margin: 0 10px 0 0; padding: 5px 10px; text-decoration: none; border-radius: 3px; -moz-border-radius: 3px; -o-border-radius: 3px; -webkit-border-radius: 3px; }
.showpage a:hover, .showpageNum a:hover {  background: #101010;  color: #fff;  border-radius: 3px;  -moz-border-radius: 3px;  -o-border-radius: 3px;  -webkit-border-radius: 3px;  text-decoration: none;  }
#blog-pager-newer-link { padding: 20px 0 0; position: relative; text-align: left; width: 40%; }
#blog-pager-newer-link:before {
    content: "\00AB";
    font-size: 22px;
    margin-right: 10px;
    float: left;
    margin-top: 10px;
    color: #fff;
    width: 35px;
    height: 35px;
    line-height: 28px;
    padding: 0 12px;
    border-radius: 50%;
    background-color: #333;
}
#blog-pager-older-link { padding: 20px 0 0; position: relative; text-align: right; width: 40%; }
#blog-pager-older-link:before {
    content: "\00BB";
    font-size: 22px;
    float: right;
    margin-left: 15px;
    margin-top: 9px;
    background-color: #333;
    color: #fff;
    width: 35px;
    height: 35px;
    line-height: 28px;
    padding: 0 12px;
    border-radius: 50%;
}
#blog-pager-newer-link .newer-text, #blog-pager-older-link .older-text { display: block; color: #999; }
/*****************************************
Post Highlighter CSS
******************************************/
blockquote { border-color: #F1F4F9; border-style: solid; border-width: 1px 0; color: #888888; margin: 10px 0 20px; padding: 15px 40px; }
div#blog-banner {
  width: 100%;
  height: 400px;
  background-position: 50%;
  background-repeat: no-repeat;
  background-size: cover;
}
/*****************************************
Sidebar CSS
******************************************/
.sidebar { margin: 0; padding: 0; display: block; }
.sidebar h2 {
  position: relative;
  font-size: 16px;
  margin-bottom: 25px;
  padding-bottom: 5px;
  text-transform: uppercase;
  line-height: 1.7;
}
.sidebar h2:after {
  top: 40px;
  color: #333;
  left: 2px;
}
.sidebar .widget { padding: 25px 20px; clear: both; font-size: 13px; line-height: 23px; margin-bottom: 30px;  }
.sidebar ul { margin: 0; padding: 0; list-style: none; }
.sidebar li {
border-bottom: 1px solid #F1f4f9;
line-height: normal;
list-style: none !important;
margin: 8px 0;
overflow: hidden;
padding: 0 0 10px;
}
/* --------------------------- */
/* 	>> FOOTER				   */
/* --------------------------- */
.footer_bottom {
    position: relative;
    background-color: #222;
    padding: 20px 0 0;
    margin-top: 80px;
}
.footerLogo {
    padding-top: 60px;
}
#Footer-header {
    display: table;
    margin: 0 auto;
    margin-bottom: 35px;
}
div#Header2 h1 a {
  color: #eeeeee;
}
div#Header2 h1 {
  font: normal normal 70px Rock Salt;
  font-size: 44px;
  line-height: 1.5;
  letter-spacing: 2px;
}
.contact_us {
  text-align: center;
  display: table;
  margin: 0 auto;
  margin-bottom: 55px;
}
.contact_us a {
  background-color: #edc037;
  color: #fff;
  padding: 8px 30px;
  display: block;
  border-radius: 20px;
  font-size: 12px;
  font-family: montserrat,sans-serif;
  text-transform: uppercase;
}
.bottom_share {
  display: table;
  margin: 0 auto;
  margin-bottom: 55px;
  border-top: 2px solid #444;
  padding-top: 25px;
}
.bottom_share a {
  font-size: 22px;
  color: #999;
  display: inline-block;
  margin: 0 15px;
}
p.attribution {
  	background-color: #101010;
  	padding: 20px 0;
  	margin: 0 auto;
  	text-align: center;
  	color: #777;
  	font-size: 14px;
	font-weight: 300;
}
p.attribution, p.attribution a {
	color: #777;
}
.toTop {
  position: relative;
  display: table;
  margin: 0 auto;
  text-align: center;
}
.toTop a {
  position: absolute;
  top: -45px;
  left: -25px;
  display: block;
  background-color: #222222;
  padding: 7px 14px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  border: 4px solid #F3F3F3;
  color: #fff;
}
/*****************************************
Custom Widget CSS
******************************************/
/***** Search Form *****/
#searchform fieldset { background: #F1F4F9; border: 1px solid #F1F4F9; color: #888888; width: 98%; }
#searchform fieldset:hover { background: #fff; }
#s { background: url("http://3.bp.blogspot.com/-Mu6D1ld_3TE/U35bF1XXIVI/AAAAAAAADBM/VaHEtkyX3MA/s1600/sprites.png") no-repeat scroll right -60px rgba(0, 0, 0, 0); border: 0 none; color: #888888; float: left; margin: 8px 5%; padding: 0 10% 0 0; width: 80%; }
/***** Custom Labels *****/
.cloud-label-widget-content { display: inline-block; text-align: left; }
.cloud-label-widget-content .label-size { display: inline-block; float: left; font-size: 10px; font-family: Verdana,Arial,Tahoma,sans-serif; font-weight: bold; line-height: normal; margin: 5px 5px 0 0; opacity: 1; text-transform: uppercase; }
.cloud-label-widget-content .label-size a { color: #000 !important; float: left; padding: 5px; }
.cloud-label-widget-content .label-size:hover a { color: #333 !important; }
.cloud-label-widget-content .label-size .label-count { color: #333; padding: 5px 0; float: left; }
.Label li {
border: 0;
display: inline-block;
padding: 0;
margin: 0;
margin-right: 5px;
margin-bottom: 5px;
}
.Label li a {
display: block;
border: 1px solid #333;
border-radius: 20px;
padding: 7px 15px;
line-height: 1;
}
/***** Popular Post *****/
.PopularPosts .item-thumbnail img {
display: block;
float: left;
height: 73px;
width: 73px;
padding: 0;
border-radius: 80px;
}
.item-snippet {
display: none;
}
/***** Blogger Contact Form Widget *****/
.contact-form-email, .contact-form-name, .contact-form-email-message, .contact-form-email:hover, .contact-form-name:hover, .contact-form-email-message:hover, .contact-form-email:focus, .contact-form-name:focus, .contact-form-email-message:focus { background: #F8F8F8; border: 1px solid #D2DADD; box-shadow: 0 1px 1px #F3F4F6 inset; max-width: 300px; color: #999; }
.contact-form-button-submit { background: #000; border: medium none; float: right; height: auto; margin: 10px 0 0; max-width: 300px; padding: 5px 10px; width: 100%; cursor: pointer; }
.contact-form-button-submit:hover { background: #2980B9; border: none; }
/***** Profile Widget CSS *****/
.Profile img { border:1px solid #cecece; background:#fff; float:left; margin:5px 10px 5px 0; padding: 5px; -webkit-border-radius: 50%;	-moz-border-radius: 50%; border-radius: 50%; }
.profile-data { color:#999999; font:bold 20px/1.6em Arial,Helvetica,Tahoma,sans-serif; font-variant:small-caps; margin:0; text-transform:capitalize;}
.profile-datablock { margin:0.5em 0;}
.profile-textblock { line-height:1.6em; margin:0.5em 0;}
a.profile-link { clear:both; display:block; font:80% monospace; padding:10px 0; text-align:center; text-transform:capitalize;}
/***** Meet The Author *****/
#About { background: #FFFFFF; display: inline-block; padding: 25px 3%; width: 100%; }
#About .widget-content { position: relative; width: 100%; }
#About .widget-content .main-wrap { width: auto; margin-right: 370px; }
#About .widget-content .main-wrap .info { float: left; position: relative; width: 90%; padding: 10px 5%; }
#About .widget-content .side-wrap { width: 340px; float: right; text-align: center; }
#About .widget-content .main-wrap .info h5 { border-bottom: 1px solid #F1F4F9; color: #000000; font-size: 16px; font-weight: bold; margin: 0 0 10px; padding: 0 0 5px; text-transform: capitalize; } 
#About .widget-content .main-wrap .info p { color: #333; font-style: italic; } 
#About .widget-content .side-wrap .author-img { border: 1px solid #CECECE; height: 150px; vertical-align: bottom; width: 150px; -webkit-border-radius: 50%;	-moz-border-radius: 50%; border-radius: 50%; }
ul.author-social { display: inline-block; margin: 10px 0 0; padding: 0; }
ul.author-social li { background: url("http://3.bp.blogspot.com/-Mu6D1ld_3TE/U35bF1XXIVI/AAAAAAAADBM/VaHEtkyX3MA/s1600/sprites.png") no-repeat; display: inline-block; font-weight: bold; font-size: 12px; line-height: 16px; list-style: none; padding: 0 20px; }
ul.author-social li.facebook { background-position: 0 -80px; }
ul.author-social li.twitter { background-position: 0 -100px; }
ul.author-social li.googleplus { background-position: 0 -120px; }
ul.author-social li.rss { background-position: 0 -176px; }
ul.author-social li a { color: #000; }
ul.author-social li a:hover { color: #666; }
.post-footer{margin-top:30px;}
/* ---------------------------- */
/* 	SHARE WRAPPER				*/
/* ---------------------------- */
.share-wrapper {margin-bottom: 50px;}
.share-wrapper ul {padding: 0;margin: 0;text-align: center;}
.share-wrapper li {list-style: none;display: inline-block;margin-right: 10px;padding: 0;margin-bottom: 30px;}
.share-wrapper li a{display:block;text-align: center;}
.share-wrapper span{display:none;}
.share-wrapper li a i {
display: block;
color: #333;
width: 40px;
height: 40px;
padding: 9px;
font-size: 24px;
}
.share-wrapper{margin-bottom:30px;}
/* ----------------------------- */
/* AUTHOR BOX 					 */
/* ----------------------------- */
.authorboxwrap {
    display: inline-block;
    width: 100%;
    padding-bottom: 40px;
}
.avatar-container {width: 170px;float: left;}
.avatar-container img {width: 125px;height: auto;border: 5px solid transparent;box-shadow: 0px 0px 20px -5px #000;-moz-box-shadow: 0px 0px 20px -5px #000;-webkit-box-shadow: 0px 0px 20px -5px #000;-ms-box-shadow: 0px 0px 20px -5px #000;-o-box-shadow: 0px 0px 20px -5px #000;}
.author_description_container {margin-left: 170px;}
.author_description_container h4 {font-weight:600;font-size: 16px;display: block;margin-bottom: 10px;}
.author_description_container h4 a{color: #333;}
.author_description_container p {font-size: 12px;line-height: 1.7;margin-bottom: 15px;}
.authorsocial a {display: inline-block;margin-right: 5px;text-align: center;float:left;margin-right:2px;}
.authorsocial a i {width: 30px;height: 30px;padding: 8px 9px;display: block;background: #E9E9E9!important;color: #333;}
/* ----------------------- */
/* 	RELATED POSTS		   */
/* ----------------------- */
#related-posts {
    font-size: 16px;
    display: inline-block;
    width: 100%;
}
#related-posts h5 {
    font-size: 16px;
    text-transform: uppercase;
    margin: 0 0 25px;
    padding-bottom: 15px;
    font-weight: 900;
    letter-spacing: 1px;
    text-align: center;
    position: relative;
}
#related-posts h5:after {
    content: "";
    position: absolute;
    width: 4px;
    height: 4px;
    background: #222;
    border-radius: 50%;
    bottom: 0;
    left: 47%;
    box-shadow: 1em 0px 0px 0px #222, 2em 0px 0px 0px #222;
}
#related-posts ul {
    padding: 0;
    margin: 0;
}
#related-posts ul li {
    list-style: none;
    display: block;
    float: left;
    width: 32.75%;
    padding: 0;
    margin: 1px;
    text-align: center;
    position: relative;
}
#related-posts img {
    padding: 0;
    width: 100%;
    height: 145px;
}
a.related-thumbs {
    position: relative;
    display: block;
}
a.related-thumbs:before{opacity:1;}
a.related-title {
    display: block;
    font-family: Pt Serif, serif;
    font-size: 14px;
    font-weight: bold;
    margin: 15px 0 0;
}
/* ---------------------------- */
/* 	SOCIAL WIDGET - FOOTER 		*/
/* ---------------------------- */
.social-widget {
padding: 40px 0;
}
.social-widget a {
margin-left: 15px;
display: inline-block;
}
.social-widget a div {
display: inline-block;
width: 50px;
height: 50px;
font-size: 26px;
line-height:1;
padding: 14px 0;
text-align: center;
color: #333;
}
/*****************************************
Comments CSS
******************************************/
#comments {margin-top: 30px;margin-right: 15px;background: white;padding: 25px;border-bottom: 1px solid #D6D6D6;box-shadow: 0px 2px 10px -7px #000;-webkit-box-shadow: 0px 2px 10px -7px #000;-moz-box-shadow: 0px 2px 10px -7px #000;-o-box-shadow: 0px 2px 10px -7px #000;}
.comments h4 { font-size: 20px; margin: 0 0 18px; text-transform: capitalize; }
.comments .comments-content .comment-thread ol { overflow: hidden; margin: 0; }
.comments .comments-content .comment:first-child { padding-top: 0; }
.comments .comments-content .comment { margin-bottom: 0; padding-bottom: 0; }
.comments .avatar-image-container { max-height: 60px; width: 60px; }
.comments .avatar-image-container img { max-width: 60px; width: 100%; border-radius: 10px;-webkit-border-radius: 10px;-moz-border-radius: 10px;}
.comments .comment-block { background: #fff; margin-left: 72px; padding: 14px 0 0 20px; border-radius: 2px; -moz-border-radius: 2px; -webkit-border-radius: 2px; }
.comments .comments-content .comment-header a { color: #333; text-transform: capitalize; }
.comments .comments-content .user { display: block; font-style: normal; font-weight: bold; }
.comments .comments-content .datetime { margin-left: 0; }
.comments .comments-content .datetime a { font-size: 12px; text-transform: uppercase; }
.comments .comments-content .comment-header, .comments .comments-content .comment-content { margin: 0 20px 0 0; }
.comments .comment-block .comment-actions { display: block; text-align: right; }
.comments .comment .comment-actions a { border-radius: 2px; -moz-border-radius: 2px; -webkit-border-radius:2px; background: #333; color: #FFFFFF; display: inline-block; font-size: 12px; line-height: 1;letter-spacing:1px; margin-left: 1px; padding: 5px 10px 7px; }
.comments .comment .comment-actions a:hover { text-decoration: none; }
.comments .thread-toggle { display: none; }
.comments .comments-content .inline-thread { border-left: 1px solid #F4F4F4; margin: 0 0 20px 35px !important; padding: 0 0 0 20px; }
.comments .continue { display: none; }
.comment-thread ol { counter-reset: countcomments; }
.comment-thread li:before { color:#ddd; content: counter(countcomments, decimal); counter-increment: countcomments; float: right; font-size: 22px; padding: 15px 20px 10px; position: relative; z-index: 10; }
.comment-thread ol ol { counter-reset: contrebasse; }
.comment-thread li li:before { content: counter(countcomments,decimal) "." counter(contrebasse,lower-latin); counter-increment: contrebasse; float: right; font-size: 18px; }
.comments .comments-content .icon.blog-author{dipslya:none!important;}
.vt_menu_toggle {  font-size: 21px;display: none;position: absolute;color: #fff;top: 0;background: transparent;width: 40px;height: 40px;left: 0px;padding: 7px 5px;text-align: center;z-index:1000}
/*****************************************
Responsive styles
******************************************/
@media screen and (max-width: 960px) {
.ct-wrapper{ padding:0 15px; }
.main-wrapper { margin-right:0; width:100%; }
.sidebar-wrapper{ float: left; width: auto; margin-top: 30px; }
#About .widget-content .main-wrap { margin-right: 0; }
#About .widget-content .main-wrap .info { float: none; text-align: center; width: 90%; padding: 10px 5%; }
#About .widget-content .side-wrap { width: 100%; float: none; text-align: center; }
.sticky { position: static; }
}
@media screen and (max-width: 860px){
#comment-editor { margin:10px; }
#content{margin-right:0;}
#header h1 {font-size: 60px;}
.blog_featured_post a .blog_contents h3 {font-size: 26px;}
div#Blog1{margin:0;}
.post_title {font-size: 30px;}
.vt_menu_toggle{display:block}
ul.blog_menus {display:none;width: 240px;position: absolute;top: 45px;left: 12px;background: #333;color);padding: 0;margin: 0;}
ul.blog_menus li {display: block;text-align: left;width:100%;}
.main-wrapper {width: 100%;}
#content{margin:0!important;}
.nav-menu li a{padding:10px 20px;}
.article_excerpt h2 {
  font-size: 28px;
  line-height: 1.3;
}
}
@media screen and (max-width: 520px){
.blog_featured_post a .blog_contents h3 {font-size: 20px;}
.blog_featured_post a .blog_contents{bottom:15px;}
.post_title {font-size: 26px;}
#content{padding-right:0!important;}
}
@media screen and (max-width: 420px){
.comments .comments-content .datetime{    display:block;    float:none;    }
.comments .comments-content .comment-header {    height:70px;    }
}
@media screen and (max-width: 320px){
.ct-wrapper{ padding:0; }
.post-body img{  max-width: 230px; }
.comments .comments-content .comment-replies {    margin-left: 0;    }
}
/*****************************************
Hiding Header Date and Feed Links
******************************************/
h2.date-header,span.blog-admin{display:none!important}
.playbutton {position: relative;padding-bottom: 56.25%; /* 16:9 */padding-top: 25px;height: 0;}
.playbutton iframe {position: absolute;top: 0;left: 0;width: 100%;height: 100%;}
]]></b:skin>




<b:if cond='data:blog.pageType == &quot;index&quot;'>
<style type='text/css'>
.sidebar-wrapper{display:none;}

	.post-body {
    	margin: 0 0 40px;
	}
	.share-wrapper {
   	 	margin-bottom: 0;
	}
	.share-wrapper li:first-child {
	    display: none; 
	}
	.share-wrapper li { margin-bottom: 0; }
	.share-wrapper li a i {
    	display: block;
    	color: #333;
    	width: 24px;
    	height: 24px;
    	font-size: 16px;
	}

</style>
</b:if>

<b:if cond='data:blog.pageType == &quot;item&quot;'>
<style type='text/css'>

.post-body {
    margin: 0 0 30px; 
}

.post-body img{width:100%; height: auto; max-width: 100%; }
.post-outer{width:100%;}
.post.hentry {margin: 0;}
#content {}

</style>
</b:if>

<b:if cond='data:blog.pageType == &quot;static_page&quot;'>
<style type='text/css'>
#blog-pager { display: none; }
.post-outer {width: 100%;float: none;}
.post.hentry {margin: 0;margin-right: 15px;padding: 25px;}
h2.post_title.entry-title {margin-bottom: 25px;}
</style>
</b:if>



<style type='text/css'>

/*
    Mobile Menu Core Style
*/

#slick_nav {
    position: absolute;
    top: 2%;
    left: 45%;
    z-index: 1000;
}

@media screen and (min-width: 786px){
	#slick_nav {
    	display: none;
	}
}

.slicknav_btn { position: relative; display: block; vertical-align: middle; float: left;  line-height: 27px; cursor: pointer;  height:27px;}
.slicknav_menu  .slicknav_menutxt { display: block; line-height: 1.188em; float: left; }
.slicknav_menu .slicknav_icon { float: left; margin: 0.188em 0 0 0.438em; }
.slicknav_menu .slicknav_no-text { margin: 0 }
.slicknav_menu .slicknav_icon-bar { background: #eee; display: block; width: 1.125em; height: 0.125em; }
.slicknav_btn .slicknav_icon-bar + .slicknav_icon-bar { margin-top: 0.188em }

.slicknav_btn {
    display: block;
    width: 80px;
    height: 50px;
    margin: 0;
    padding: 11px 0;
    text-decoration: none;
}

.slicknav_nav { clear: both }
.slicknav_nav ul,
.slicknav_nav li { display: block }
.slicknav_nav .slicknav_arrow { font-size: 0.8em; margin: 0 0 0 0.4em; }
.slicknav_nav .slicknav_item { cursor: pointer; }
.slicknav_nav .slicknav_row { display: block; }
.slicknav_nav a { display: block }
.slicknav_nav .slicknav_item a,
.slicknav_nav .slicknav_parent-link a { display: inline }
.slicknav_menu:before,
.slicknav_menu:after { content: &quot; &quot;; display: table; }
.slicknav_menu:after { clear: both }
/* IE6/7 support */
.slicknav_menu { *zoom: 1 }

/* 
    User Default Style
    Change the following styles to modify the appearance of the menu.
*/

.slicknav_menu {
    font-size:16px;
}
/* Button */
.slicknav_btn {
    margin: 0;
    text-decoration:none;
    text-shadow: 0 1px 1px rgba(255, 255, 255, 0.75);
    -webkit-border-radius: 4px;
    -moz-border-radius: 4px;
    border-radius: 4px;  

}
a.slicknav_btn:after {
    color: #fff;
    content: &quot;MENU&quot;;
    font-size: 12px;
    top: -2px;
    padding-left: 10px;
    position: relative;
}
/* Button Text */
.slicknav_menu  .slicknav_menutxt {
    color: #FFF;
    font-weight: bold;
    text-shadow: 0 1px 3px #000;
}
/* Button Lines */


.slicknav_nav {
    color:#fff;
    margin:0;
    padding:0;
    font-size:0.875em;
}
.slicknav_nav, .slicknav_nav ul {
    list-style: none;
    overflow:hidden;
}
.slicknav_nav ul {
    padding:0;
    margin:8px 0 0 20px;
}
.slicknav_nav .slicknav_row {
    padding:5px 10px;
    margin:2px 5px;
}

.slicknav_nav .slicknav_item a,
.slicknav_nav .slicknav_parent-link a {
    padding:0;
    margin:0;
}
.slicknav_nav .slicknav_row:hover {

}
.slicknav_nav a:hover{

    background:#333;
    color:#fff;
}
.slicknav_nav .slicknav_txtnode {
     margin-left:15px;   
}

.slicknav_menu .slicknav_no-text {
	margin-top:7px;
}


/* Mobile Menu */
ul.slicknav_nav {
    background: #333;
    padding: 5px 20px;
    position: absolute;
    top: 55px;
    left: -10px;
    width: 200px;
    z-index: 100;
}
ul.slicknav_nav li {
    padding: 7px 0;
}
ul.slicknav_nav li a {
    color: #fff;
    font-family: Montserrat, sans-serif;
    font-size: 11px;
    letter-spacing: .5px;
    text-transform: uppercase;
}


@media screen and (max-width: 420px){
	.nav-col {
    	float: none;
	}

	.slicknav_btn {
		float: none;
    	margin: 0 auto;
	}
	ul.slicknav_nav {
		left: 90px;
    }

}
</style>

<style id='owl-carousel' type='text/css'>
/**
 * Owl Carousel v2.2.1
 * Copyright 2013-2017 David Deutsch
 * Licensed under  ()
 */
.owl-carousel,.owl-carousel .owl-item{-webkit-tap-highlight-color:transparent;position:relative}.owl-carousel{display:none;width:100%;z-index:1}.owl-carousel .owl-stage{position:relative;-ms-touch-action:pan-Y;-moz-backface-visibility:hidden}.owl-carousel .owl-stage:after{content:&quot;.&quot;;display:block;clear:both;visibility:hidden;line-height:0;height:0}.owl-carousel .owl-stage-outer{position:relative;overflow:hidden;-webkit-transform:translate3d(0,0,0)}.owl-carousel .owl-item,.owl-carousel .owl-wrapper{-webkit-backface-visibility:hidden;-moz-backface-visibility:hidden;-ms-backface-visibility:hidden;-webkit-transform:translate3d(0,0,0);-moz-transform:translate3d(0,0,0);-ms-transform:translate3d(0,0,0)}.owl-carousel .owl-item{min-height:1px;float:left;-webkit-backface-visibility:hidden;-webkit-touch-callout:none}.owl-carousel .owl-item img{display:block;width:100%}.owl-carousel .owl-dots.disabled,.owl-carousel .owl-nav.disabled{display:none}.no-js .owl-carousel,.owl-carousel.owl-loaded{display:block}.owl-carousel .owl-dot,.owl-carousel .owl-nav .owl-next,.owl-carousel .owl-nav .owl-prev{cursor:pointer;cursor:hand;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.owl-carousel.owl-loading{opacity:0;display:block}.owl-carousel.owl-hidden{opacity:0}.owl-carousel.owl-refresh .owl-item{visibility:hidden}.owl-carousel.owl-drag .owl-item{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.owl-carousel.owl-grab{cursor:move;cursor:grab}.owl-carousel.owl-rtl{direction:rtl}.owl-carousel.owl-rtl .owl-item{float:right}.owl-carousel .animated{animation-duration:1s;animation-fill-mode:both}.owl-carousel .owl-animated-in{z-index:0}.owl-carousel .owl-animated-out{z-index:1}.owl-carousel .fadeOut{animation-name:fadeOut}@keyframes fadeOut{0%{opacity:1}100%{opacity:0}}.owl-height{transition:height .5s ease-in-out}.owl-carousel .owl-item .owl-lazy{opacity:0;transition:opacity .4s ease}.owl-carousel .owl-item img.owl-lazy{transform-style:preserve-3d}.owl-carousel .owl-video-wrapper{position:relative;height:100%;background:#000}.owl-carousel .owl-video-play-icon{position:absolute;height:80px;width:80px;left:50%;top:50%;margin-left:-40px;margin-top:-40px;background:url(owl.video.play.png) no-repeat;cursor:pointer;z-index:1;-webkit-backface-visibility:hidden;transition:transform .1s ease}.owl-carousel .owl-video-play-icon:hover{-ms-transform:scale(1.3,1.3);transform:scale(1.3,1.3)}.owl-carousel .owl-video-playing .owl-video-play-icon,.owl-carousel .owl-video-playing .owl-video-tn{display:none}.owl-carousel .owl-video-tn{opacity:0;height:100%;background-position:center center;background-repeat:no-repeat;background-size:contain;transition:opacity .4s ease}.owl-carousel .owl-video-frame{position:relative;z-index:1;height:100%;width:100%}

.owl-theme .owl-dots,.owl-theme .owl-nav{text-align:center;-webkit-tap-highlight-color:transparent}.owl-theme .owl-nav{margin-top:10px}.owl-theme .owl-nav [class*=owl-]{color:#FFF;font-size:14px;margin:5px;padding:4px 7px;background:#D6D6D6;display:inline-block;cursor:pointer;border-radius:3px}.owl-theme .owl-nav [class*=owl-]:hover{background:#869791;color:#FFF;text-decoration:none}.owl-theme .owl-nav .disabled{opacity:.5;cursor:default}.owl-theme .owl-nav.disabled+.owl-dots{margin-top:10px}.owl-theme .owl-dots .owl-dot{display:inline-block;zoom:1}.owl-theme .owl-dots .owl-dot span{width:10px;height:10px;margin:5px 7px;background:#D6D6D6;display:block;-webkit-backface-visibility:visible;transition:opacity .2s ease;border-radius:30px}.owl-theme .owl-dots .owl-dot.active span,.owl-theme .owl-dots .owl-dot:hover span{background:#869791}

.owl-prev { left: 0; }
.owl-next { right: 0; }
.owl-prev, .owl-next {
    background: #fff;
    height: 65px;
    line-height: 65px;
    padding: 0 14px;
	position: absolute;
    top: 42%;
	visibility: hidden;
	opacity: 0;
	-webkit-transition: all .3s ease-in-out;
	-moz-transition: all .3s ease-in-out;
	-o-transition: all .3s ease-in-out;
	transition: all .3s ease-in-out;
}
.owl-carousel:hover .owl-prev, .owl-carousel:hover .owl-next { opacity: 1; visibility: visible; }

</style>


<script src='http://ajax.googleapis.com/ajax/libs/jquery/1.12.1/jquery.min.js' type='text/javascript'/>



<script type='text/javascript'>
//<![CDATA[
 // Enter the posts labels here 
cat1 = 'Featured'; 
  
imgr = new Array();
imgr[0] = "http://3.bp.blogspot.com/-Viba2SFqY9E/VKfHjrChMXI/AAAAAAAAASQ/ayYZUtgFkBE/s580-c/zEk8RJdmQrqja2XwbjgJ_DSC_2368-1024x682.jpg";
showRandomImg = true;
aBold = true;
summaryPost = 150; 
summaryTitle = 50; 
numposts1 = 9;
readMoreText = 'Continue Reading';
function showrecentposts1(json) {
    j = showRandomImg ? Math.floor((imgr.length + 1) * Math.random()) : 0;
    img = new Array;
    if (numposts1 <= json.feed.entry.length) maxpost = numposts1;
    else maxpost = json.feed.entry.length;
  document.write('<div class="owl_carouselle owl-carousel">');
    for (var i = 0; i < maxpost; i++) {
        var entry = json.feed.entry[i];
        var posttitle = entry.title.$t;
        var pcm;
        var tag_name = entry.category[0].term;
        var posturl;
        if (i == json.feed.entry.length) break;
        for (var k = 0; k < entry.link.length; k++)
            if (entry.link[k].rel == "alternate") {
                posturl = entry.link[k].href;
                break
            }
        
        if ("content" in entry) var postcontent = entry.content.$t;
        else if ("summary" in entry) var postcontent = entry.summary.$t;
        else var postcontent = "";
        if (j > imgr.length - 1) j = 0;
        img[i] = imgr[j];
        s = postcontent;
        a = s.indexOf("<img");
        b = s.indexOf('src="', a);
        c = s.indexOf('"', b + 5);
        d = s.substr(b + 5, c - b - 5);
        if (a != -1 && (b != -1 && (c != -1 && d != ""))) img[i] = d;
       
        var trtd = '<div class="blog_featured_post"><div class="feat-img" style="background-image:url('+img[i]+');"></div></div>';
        document.write(trtd);
        j++
    }
    document.write('</div>')
};
  //]]>
</script>

<script type='text/javascript'>
/*<![CDATA[*/
// JavaScript Document
function removeHtmlTag(e, t) {
    if (e.indexOf("<") != -1) {
        var n = e.split("<");
        for (var r = 0; r < n.length; r++) {
            if (n[r].indexOf(">") != -1) {
                n[r] = n[r].substring(n[r].indexOf(">") + 1, n[r].length)
            }
        }
        e = n.join("")
    }
    t = t < e.length - 1 ? t : e.length - 2;
    while (e.charAt(t - 1) != " " && e.indexOf(" ", t) != -1) t++;
    e = e.substring(0, t - 1);
    return e + " ..."
}
function rm(e, t, n,date,author,tag) {
    var r = document.getElementById(e);
    var i = document.getElementById(n);
 	var tag = tag;
    var s = "";
    var o = r.getElementsByTagName("img");
    var a = summary_noimg;
    var p = "";
     if (o.length >= 1) {
        s = '<div class="post-image"><a title="" href="' + t + '"><img src="' + o[0].src.replace(/s\B\d{2,4}/, 's' + 1600) + '" class="img-responsive"/></a></div>';
        a = summaryi
    }
	if (r.innerHTML.indexOf("thumbvideo") != -1) {
        s = '<div class="playbutton"><a title="" href="' + t + '"><img alt="" class="imgcon" src="' + o[0].src + '" width="' + thw + 'px" height="' + thh + 'px"/></a></div>';
        a = summaryv
    }
    if (r.innerHTML.indexOf("http://www.youtube.com/v/") != -1) {
        var v = u[0].src;
        var m = v.substring(v.indexOf("http://www.youtube.com/v/") + 25);
        s = '<div class="playbutton"><a href="' + t + '"><iframe class="imgcon" src="http://www.youtube.com/embed/' + m + '" width="' + thw + 'px" height="' + thh + 'px"></iframe></div>';
        a = summaryi
    }
    if (r.innerHTML.indexOf("http://www.youtube.com/embed/") != -1) {
        var v = u[0].src;
        var m = v.substring(v.indexOf("http://www.youtube.com/embed/") + 29);
        s = '<div class="playbutton youtube"><iframe class="imgcon" src="http://www.youtube.com/embed/' + m + '" width="' + thw + 'px" height="' + thh + 'px"></iframe></div>';
        a = summaryi
    }
    if (r.innerHTML.indexOf("//www.youtube.com/embed/") != -1) {
        var v = u[0].src;
        var m = v.substring(v.indexOf("//www.youtube.com/embed/") + 24);
        s = '<div class="playbutton youtube"><iframe class="imgcon" src="http://www.youtube.com/embed/' + m + '" width="' + thw + 'px" height="' + thh + 'px"></iframe></div>';
        a = summaryi
    }
    if (r.innerHTML.indexOf("http://www.youtube-nocookie.com/embed/") != -1) {
        var v = u[0].src;
        var m = v.substring(v.indexOf("http://www.youtube-nocookie.com/embed/") + 38);
        s = '<div class="playbutton youtube" ><iframe class="imgcon" src="http://www.youtube.com/embed/' + m + '" width="' + thw + 'px" height="' + thh + 'px"></iframe></div>';
        a = summaryv
    }
    if (r.innerHTML.indexOf("//www.youtube-nocookie.com/embed/") != -1) {
        var v = u[0].src;
        var m = v.substring(v.indexOf("//www.youtube-nocookie.com/embed/") + 33);
        s = '<div class="playbutton youtube"><iframe class="imgcon" src="http://www.youtube.com/embed/' + m + '" width="' + thw + 'px" height="' + thh + 'px"></iframe></div>';
        a = summaryi
    }
    if (r.innerHTML.indexOf("http://player.vimeo.com/video/") != -1) {
        var v = u[0].src;
        var m = v.substring(v.indexOf("http://player.vimeo.com/video/") + 30);
        s = '<div class="playbutton vimeo"><iframe class="imgcon" src="//player.vimeo.com/video/' + m + '" width="' + thw + 'px" height="' + thh + 'px" ></iframe></div>';
        a = summaryi
    }
    if (r.innerHTML.indexOf("//player.vimeo.com/video/") != -1) {
        var v = u[0].src;
        var m = v.substring(v.indexOf("//player.vimeo.com/video/") + 25);
        s = '<div class="playbutton vimeo"><iframe class="imgcon" src="//player.vimeo.com/video/' + m + '" width="' + thw + 'px" height="' + thh + 'px" ></iframe></div>';
        a = summaryi
    }
var g = s + '<div class="post-header"><div class="post-category">'+tag+'</div><h2 class="entry-title"><a href="'+ t +'">'+ n +'</a></h2><div class="post-meta"><div class="post-date">posted on '+ date +'</div><div class="post-author">by '+ author +'</div></div></div><div class="post-content">'+removeHtmlTag(r.innerHTML, a)+'</div><div class="post-read-more"><a href="'+ t +'">'+ Readmore_word +'</a></div>';
r.innerHTML = g;
};
var Readmore_word = "Continue Reading"; // Append  " Read More " String after post break 
var summary_noimg = 420;
summaryi = 320;
summaryv = 320;
thh = 420;
thw = 674;
$(document).ready(function() {
 $('.gallery-wrapper').hover(function() {
      $(this).find('.overlay').fadeToggle(250);
  });
});
/* 
imgCentering.js jQuery Plugin
* A jQuery plugin to centering your pictures and images
*
* Name:			imgCentering.js
* Author:		Kenny Ooi - http://www.inwebson.com
* Date:			September 28, 2012		
* Version:		1.1
* Example:		http://www.inwebson.com/demo/imgcentering/
*
*/
(function($){var blank="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///ywAAAAAAQABAAACAUwAOw==";var imgCentering=function(obj,options){var defaults={'forceWidth':false,'forceHeight':false,'forceSmart':false,'bgColor':"inherit"};function forceWidth(obj){obj.css('width','100%');}
function forceHeight(obj){obj.css('height','100%');}
var img=$(obj);var settings=$.extend(defaults,options);img.load(function(){var _conwidth=img.parent().width();var _conheight=img.parent().height();var _parentpos=img.parent().css('position');if(settings.bgColor=='inherit')
var _parentbg=img.parent().css('backgroundColor');else
var _parentbg=settings.bgColor;img.css('width','auto');img.css('height','auto');if(settings.forceSmart){var _fullratio=img.width()/ img.height();var _conratio=_conwidth / _conheight;if(_fullratio<_conratio)
forceWidth(img);else
forceHeight(img);}else{if(settings.forceWidth)
forceWidth(img);if(settings.forceHeight)
forceHeight(img);}
var _finalwidth=img.width();var _finalheight=img.height();img.css({'position':'relative','left':-(_finalwidth-_conwidth)/2+'px','top':-(_finalheight-_conheight)/2+'px'}).parent().css({'position':_parentpos,'overflow':'hidden','backgroundColor':_parentbg});});if(obj.complete||obj.complete===undefined){var src=obj.src;obj.src=blank;obj.src=src;}}
$.fn.imgCentering=function(options){return this.each(function(e){var img=$(this);if(img.data('imgCentering'))return;var imgcenter=new imgCentering(this,options);img.data('imgCentering',imgcenter);});}})(jQuery);$(document).ready(function(){$('.gallry_img').imgCentering({'forceWidth':true});});
/*]]>*/</script>


<b:if cond='data:blog.pageType == &quot;item&quot;'>
<script type='text/javascript'>
//<![CDATA[
$(document).ready(function() {
$('.post-body img:eq(0)').each(function() {
var image = $(this);
var src = image.attr("src");
var href= image.parent().attr("href");
var banner = $('#blog-banner');
var imgtag = $('<a rel="prettyPhoto" href="' + href + '"><img src="' + src + '" /></a>');
imgtag.appendTo(".bckpic");
banner.css({'background-image': 'url(' + src + ')'});  
}); 
});
//]]></script>

</b:if>

</head>
<!--<body>-->
<body>


<!-- __ HEADER __ -->

<header class='header' id='site-header'>
	<b:section class='header' id='header' maxwidgets='1' showaddelement='yes'>
<b:widget id='Header1' locked='true' title='Storyteller (Header)' type='Header' version='1'>
  <b:widget-settings>
    <b:widget-setting name='displayUrl'/>
    <b:widget-setting name='displayHeight'>0</b:widget-setting>
    <b:widget-setting name='sectionWidth'>150</b:widget-setting>
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
          <div expr:style='&quot;background-image: url(\&quot;&quot; + data:sourceUrl + &quot;\&quot;); &quot;                        + &quot;background-position: &quot;                        + data:backgroundPositionStyleStr + &quot;; &quot;                        + data:widthStyleStr                        + &quot;min-height: &quot; + data:height                        + &quot;_height: &quot; + data:height                        + &quot;background-repeat: no-repeat; &quot;' id='header-inner'>
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
        <a class='logo' expr:href='data:blog.homepageUrl' style='display: inline-block'>
          <img expr:alt='data:title' expr:id='data:widget.instanceId + &quot;_headerimg&quot;' expr:src='data:sourceUrl' style='display: block'/>
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
    <a expr:href='data:blog.homepageUrl'><data:title/></a>
</b:includable>
</b:widget>
</b:section>


	<!-- __ FEATURED SLIDER __ -->

	<div class='featured_slider'>
	<b:if cond='data:blog.pageType == &quot;index&quot;'>
		<!-- Slider Container -->
		<div class='carousel-1 slider' id='main-slider'>

			<script>document.write(&quot;&lt;script src=\&quot;/feeds/posts/default/-/&quot;+cat1+&quot;?max-results=&quot;+numposts1+&quot;&amp;orderby=published&amp;alt=json-in-script&amp;callback=showrecentposts1\&quot;&gt;&lt;\/script&gt;&quot;);</script>

		</div>
	</b:if>

		<b:if cond='data:blog.pageType == &quot;item&quot;'>
			<div id='blog-banner'/>
		</b:if>
  	</div>


</header>


<!-- __ NAVIGATION __ -->

<div class='nav-menu'>
	<div id='slick_nav'/>

	<div class='ct-wrapper'>
		<ul class='blog_menus'>
  			<li><a expr:href='data:blog.homepageUrl'>My Story</a></li>
  			<li><a href='#'>Gallery</a></li>
  			<li><a href='#'>Archive</a></li>
  			<li><a href='#'>Blog</a></li>
  			<li><a href='/p/blog-page.html'>About</a></li>
			<li><a href='#'>Contact</a></li>
		</ul>
   </div>
</div>



<!-- __ ABOUT AUTHOR __ -->

<div class='about_author'>
	<div class='blog_author'>
		<div class='author_thumbnail'>
			<img src='http://1.bp.blogspot.com/-UzkSBiqI288/VN8s5gboKdI/AAAAAAAABAo/iFSuwrrBWOk/s1600/groom.jpg'/>
		</div>
		<div class='detail'>
			<h2 class='name'>James Derulo&#39;s</h2>
			<span class='term'>Portfolio</span>
		</div>
	</div>
</div>



<!-- __ SITE CONTENT  __ -->

<div class='content-wrapper' id='site-content'>
	<div class='ct-wrapper'>
    	<div class='main-wrapper'>
        	<b:section class='content' id='content' maxwidgets='1' showaddelement='no'>
<b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog' version='1'>
  <b:widget-settings>
    <b:widget-setting name='showDateHeader'>true</b:widget-setting>
    <b:widget-setting name='style.textcolor'>#000000</b:widget-setting>
    <b:widget-setting name='showShareButtons'>true</b:widget-setting>
    <b:widget-setting name='showCommentLink'>true</b:widget-setting>
    <b:widget-setting name='style.urlcolor'>#008000</b:widget-setting>
    <b:widget-setting name='showAuthor'>true</b:widget-setting>
    <b:widget-setting name='style.linkcolor'>#0000ff</b:widget-setting>
    <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
    <b:widget-setting name='style.bgcolor'>#ffffff</b:widget-setting>
    <b:widget-setting name='showAuthorProfile'>true</b:widget-setting>
    <b:widget-setting name='style.layout'>1x1</b:widget-setting>
    <b:widget-setting name='showLabels'>true</b:widget-setting>
    <b:widget-setting name='showLocation'>true</b:widget-setting>
    <b:widget-setting name='showTimestamp'>true</b:widget-setting>
    <b:widget-setting name='postsPerAd'>1</b:widget-setting>
    <b:widget-setting name='showBacklinks'>false</b:widget-setting>
    <b:widget-setting name='style.bordercolor'>#ffffff</b:widget-setting>
    <b:widget-setting name='showInlineAds'>false</b:widget-setting>
    <b:widget-setting name='showReactions'>false</b:widget-setting>
  </b:widget-settings>
  <b:includable id='main' var='top'>
  <b:if cond='data:mobile == &quot;false&quot;'>

    <!-- posts -->
    <div class='blog-posts hfeed'>

      <b:include data='top' name='status-message'/>

      <data:defaultAdStart/>
      <b:loop values='data:posts' var='post'>
        <div class='post-outer'>
        <b:include data='post' name='post'/>
        <b:if cond='data:blog.pageType == &quot;item&quot;'>
          <!-- navigation -->
          <b:include name='nextprev'/>
        </b:if>
        <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
          <b:include data='post' name='comment_picker'/>
        </b:if>
        <b:if cond='data:blog.pageType == &quot;item&quot;'>
          <b:include data='post' name='comment_picker'/>
        </b:if>
        </div>
        <b:if cond='data:post.includeAd'>
          <b:if cond='data:post.isFirstPost'>
            <data:defaultAdEnd/>
          <b:else/>
            <data:adEnd/>
          </b:if>
          <div class='inline-ad'>
            <data:adCode/>
          </div>
          <data:adStart/>
        </b:if>
      </b:loop>
      <data:adEnd/>
    </div>

    <b:if cond='data:blog.pageType != &quot;item&quot;'>
    <!-- navigation -->
    <b:include name='nextprev'/>
    </b:if>


    <b:if cond='data:top.showStars'>
      <script src='//www.google.com/jsapi' type='text/javascript'/>
      <script type='text/javascript'>
        google.load(&quot;annotations&quot;, &quot;1&quot;, {&quot;locale&quot;: &quot;<data:top.languageCode/>&quot;});
        function initialize() {
          google.annotations.setApplicationId(<data:top.blogspotReviews/>);
          google.annotations.createAll();
          google.annotations.fetch();
        }
        google.setOnLoadCallback(initialize);
      </script>
    </b:if>

  <b:else/>
    <b:include name='mobile-main'/>
  </b:if>

  <b:if cond='data:top.showDummy'>
    <data:top.dummyBootstrap/>
  </b:if>

</b:includable>
  <b:includable id='backlinkDeleteIcon' var='backlink'>
  <span expr:class='&quot;item-control &quot; + data:backlink.adminClass'>
    <a expr:href='data:backlink.deleteUrl' expr:title='data:top.deleteBacklinkMsg'>
      <img src='//www.blogger.com/img/icon_delete13.gif'/>
    </a>
  </span>
</b:includable>
  <b:includable id='backlinks' var='post'>
  <a name='links'/><h4><data:post.backlinksLabel/></h4>
  <b:if cond='data:post.numBacklinks != 0'>
    <dl class='comments-block' id='comments-block'>
      <b:loop values='data:post.backlinks' var='backlink'>
        <div class='collapsed-backlink backlink-control'>
          <dt class='comment-title'>
            <span class='backlink-toggle-zippy'>&#160;</span>
            <a expr:href='data:backlink.url' rel='nofollow'><data:backlink.title/></a>
            <b:include data='backlink' name='backlinkDeleteIcon'/>
          </dt>
          <dd class='comment-body collapseable'>
            <data:backlink.snippet/>
          </dd>
          <dd class='comment-footer collapseable'>
            <span class='comment-author'><data:post.authorLabel/> <data:backlink.author/></span>
            <span class='comment-timestamp'><data:post.timestampLabel/> <data:backlink.timestamp/></span>
          </dd>
        </div>
      </b:loop>
    </dl>
  </b:if>
  <p class='comment-footer'>
    <a class='comment-link' expr:href='data:post.createLinkUrl' expr:id='data:widget.instanceId + &quot;_backlinks-create-link&quot;' target='_blank'><data:post.createLinkLabel/></a>
  </p>
</b:includable>
  <b:includable id='comment-form' var='post'>
  <div class='comment-form'>
    <a name='comment-form'/>
    <b:if cond='data:mobile'>
      <h4 id='comment-post-message'>
        <a expr:id='data:widget.instanceId + &quot;_comment-editor-toggle-link&quot;' href='javascript:void(0)'><data:postCommentMsg/></a></h4>
      <p><data:blogCommentMessage/></p>
      <data:blogTeamBlogMessage/>
      <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
      <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='410' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
    <b:else/>
      <h4 id='comment-post-message'><data:postCommentMsg/></h4>
      <p><data:blogCommentMessage/></p>
      <data:blogTeamBlogMessage/>
      <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
      <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='410' id='comment-editor' name='comment-editor' src='' width='100%'/>
    </b:if>
    <data:post.friendConnectJs/>
    <data:post.cmtfpIframe/>
    <script type='text/javascript'>
      BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;, &#39;<data:post.communityId/>&#39;);
    </script>
  </div>
</b:includable>
  <b:includable id='commentDeleteIcon' var='comment'>
  <span expr:class='&quot;item-control &quot; + data:comment.adminClass'>
    <b:if cond='data:showCmtPopup'>
      <div class='goog-toggle-button'>
        <div class='goog-inline-block comment-action-icon'/>
      </div>
    <b:else/>
      <a class='comment-delete' expr:href='data:comment.deleteUrl' expr:title='data:top.deleteCommentMsg'>
        <img src='//www.blogger.com/img/icon_delete13.gif'/>
      </a>
    </b:if>
  </span>
</b:includable>
  <b:includable id='comment_count_picker' var='post'>
  <b:if cond='data:post.commentSource == 1'>
    <span class='cmt_count_iframe_holder' expr:data-count='data:post.numComments' expr:data-onclick='data:post.addCommentOnclick' expr:data-post-url='data:post.url' expr:data-url='data:post.canonicalUrl'>
    </span>
  <b:else/>
    <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'>
      <data:post.commentLabelFull/>:
    </a>
  </b:if>
</b:includable>
  <b:includable id='comment_picker' var='post'>
  <b:if cond='data:post.commentSource == 1'>
    <b:include data='post' name='iframe_comments'/>
  <b:elseif cond='data:post.showThreadedComments'/>
    <b:include data='post' name='threaded_comments'/>
  <b:else/>
    <b:include data='post' name='comments'/>
  </b:if>
</b:includable>
  <b:includable id='comments' var='post'>
  <div class='comments' id='comments'>
    <a name='comments'/>
    <b:if cond='data:post.allowComments'>
      <h4>
        <b:if cond='data:post.numComments == 1'>
          1 <data:commentLabel/>:
        <b:else/>
          <data:post.numComments/> <data:commentLabelPlural/>:
        </b:if>
      </h4>

      <b:if cond='data:post.commentPagingRequired'>
        <span class='paging-control-container'>
          <a expr:class='data:post.oldLinkClass' expr:href='data:post.oldestLinkUrl'><data:post.oldestLinkText/></a>
          &#160;
          <a expr:class='data:post.oldLinkClass' expr:href='data:post.olderLinkUrl'><data:post.olderLinkText/></a>
          &#160;
          <data:post.commentRangeText/>
          &#160;
          <a expr:class='data:post.newLinkClass' expr:href='data:post.newerLinkUrl'><data:post.newerLinkText/></a>
          &#160;
          <a expr:class='data:post.newLinkClass' expr:href='data:post.newestLinkUrl'><data:post.newestLinkText/></a>
        </span>
      </b:if>

      <div expr:id='data:widget.instanceId + &quot;_comments-block-wrapper&quot;'>
        <dl expr:class='data:post.avatarIndentClass' id='comments-block'>
          <b:loop values='data:post.comments' var='comment'>
            <dt expr:class='&quot;comment-author &quot; + data:comment.authorClass' expr:id='data:comment.anchorName'>
              <b:if cond='data:comment.favicon'>
                <img expr:src='data:comment.favicon' height='16px' style='margin-bottom:-2px;' width='16px'/>
              </b:if>
              <a expr:name='data:comment.anchorName'/>
              <b:if cond='data:blog.enabledCommentProfileImages'>
                <data:comment.authorAvatarImage/>
              </b:if>
              <b:if cond='data:comment.authorUrl'>
                <a expr:href='data:comment.authorUrl' rel='nofollow'><data:comment.author/></a>
              <b:else/>
                <data:comment.author/>
              </b:if>
              <data:commentPostedByMsg/>
            </dt>
            <dd class='comment-body' expr:id='data:widget.instanceId + data:comment.cmtBodyIdPostfix'>
              <b:if cond='data:comment.isDeleted'>
                <span class='deleted-comment'><data:comment.body/></span>
              <b:else/>
                <p>
                  <data:comment.body/>
                </p>
              </b:if>
            </dd>
            <dd class='comment-footer'>
              <span class='comment-timestamp'>
                <a expr:href='data:comment.url' title='comment permalink'>
                  <data:comment.timestamp/>
                </a>
                <b:include data='comment' name='commentDeleteIcon'/>
              </span>
            </dd>
          </b:loop>
        </dl>
      </div>

      <b:if cond='data:post.commentPagingRequired'>
        <span class='paging-control-container'>
          <a expr:class='data:post.oldLinkClass' expr:href='data:post.oldestLinkUrl'>
            <data:post.oldestLinkText/>
          </a>
          <a expr:class='data:post.oldLinkClass' expr:href='data:post.olderLinkUrl'>
            <data:post.olderLinkText/>
          </a>
          &#160;
          <data:post.commentRangeText/>
          &#160;
          <a expr:class='data:post.newLinkClass' expr:href='data:post.newerLinkUrl'>
            <data:post.newerLinkText/>
          </a>
          <a expr:class='data:post.newLinkClass' expr:href='data:post.newestLinkUrl'>
            <data:post.newestLinkText/>
          </a>
        </span>
      </b:if>

      <p class='comment-footer'>
        <b:if cond='data:post.embedCommentForm'>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='comment-form'/>
          <b:else/>
            <data:post.noNewCommentsText/>
          </b:if>
        <b:else/>
          <b:if cond='data:post.allowComments'>
            <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:postCommentMsg/></a>
          </b:if>
        </b:if>

      </p>
    </b:if>
    <b:if cond='data:showCmtPopup'>
      <div id='comment-popup'>
        <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'>
        </iframe>
      </div>
    </b:if>

    <div id='backlinks-container'>
    <div expr:id='data:widget.instanceId + &quot;_backlinks-container&quot;'>
       <b:if cond='data:post.showBacklinks'>
         <b:include data='post' name='backlinks'/>
       </b:if>
    </div>
    </div>
  </div>
</b:includable>
  <b:includable id='feedLinks'>
  <b:if cond='data:blog.pageType != &quot;item&quot;'> <!-- Blog feed links -->
    <b:if cond='data:feedLinks'>
      <div class='blog-feeds'>
        <b:include data='feedLinks' name='feedLinksBody'/>
      </div>
    </b:if>

  <b:else/> <!--Post feed links -->
    <div class='post-feeds'>
      <b:loop values='data:posts' var='post'>
        <b:include cond='data:post.allowComments and data:post.feedLinks' data='post.feedLinks' name='feedLinksBody'/>
      </b:loop>
    </div>
  </b:if>
</b:includable>
  <b:includable id='feedLinksBody' var='links'>
  <div class='feed-links'>
  <data:feedLinksMsg/>
  <b:loop values='data:links' var='f'>
     <a class='feed-link' expr:href='data:f.url' expr:type='data:f.mimeType' target='_blank'><data:f.name/> (<data:f.feedType/>)</a>
  </b:loop>
  </div>
</b:includable>
  <b:includable id='iframe_comments' var='post'>

  <b:if cond='data:post.allowIframeComments'>
    <script expr:src='data:post.iframeCommentSrc' type='text/javascript'/>
    <div class='cmt_iframe_holder' expr:data-href='data:post.canonicalUrl' expr:data-viewtype='data:post.viewType'/>

    <b:if cond='data:post.embedCommentForm == &quot;false&quot;'>
      <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:postCommentMsg/></a>
    </b:if>
  </b:if>
</b:includable>
  <b:includable id='mobile-index-post' var='post'>
  <div class='mobile-date-outer date-outer'>
    <b:if cond='data:post.dateHeader'>
      <div class='date-header'>
        <span><data:post.dateHeader/></span>
      </div>
    </b:if>

    <div class='mobile-post-outer'>
      <a expr:href='data:post.url'>
        <h3 class='mobile-index-title entry-title' itemprop='name'>
          <data:post.title/>
        </h3>

        <div class='mobile-index-arrow'>&amp;rsaquo;</div>

        <div class='mobile-index-contents'>
          <b:if cond='data:post.thumbnailUrl'>
            <div class='mobile-index-thumbnail'>
              <div class='Image'>
                <img expr:src='data:post.thumbnailUrl'/>
              </div>
            </div>
          </b:if>

          <div class='post-body'>
            <b:if cond='data:post.snippet'><data:post.snippet/></b:if>
          </div>
        </div>

        <div style='clear: both;'/>
      </a>

      <div class='mobile-index-comment'>
        <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
          <b:if cond='data:post.allowComments'>
            <b:if cond='data:post.numComments != 0'>
              <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><b:if cond='data:post.numComments == 1'>1 <data:top.commentLabel/><b:else/><data:post.numComments/> <data:top.commentLabelPlural/></b:if></a>
            </b:if>
          </b:if>
        </b:if>
      </div>
    </div>
  </div>
</b:includable>
  <b:includable id='mobile-main' var='top'>
    <!-- posts -->
    <div class='blog-posts hfeed'>

      <b:include data='top' name='status-message'/>

      <b:if cond='data:blog.pageType == &quot;index&quot;'>
        <b:loop values='data:posts' var='post'>
          <b:include data='post' name='mobile-index-post'/>
        </b:loop>
      <b:else/>
        <b:loop values='data:posts' var='post'>
          <b:include data='post' name='mobile-post'/>
        </b:loop>
      </b:if>
    </div>

   <b:include name='mobile-nextprev'/>
</b:includable>
  <b:includable id='mobile-nextprev'>
  <div class='blog-pager' id='blog-pager'>
    <b:if cond='data:newerPageUrl'>
      <div class='mobile-link-button' id='blog-pager-newer-link'>
      <a class='blog-pager-newer-link' expr:href='data:newerPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-newer-link&quot;' expr:title='data:newerPageTitle'>&amp;lsaquo;</a>
      </div>
    </b:if>

    <b:if cond='data:olderPageUrl'>
      <div class='mobile-link-button' id='blog-pager-older-link'>
      <a class='blog-pager-older-link' expr:href='data:olderPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-older-link&quot;' expr:title='data:olderPageTitle'>&amp;rsaquo;</a>
      </div>
    </b:if>

    <div class='mobile-link-button' id='blog-pager-home-link'>
    <a class='home-link' expr:href='data:blog.homepageUrl'><data:homeMsg/></a>
    </div>

    <div class='mobile-desktop-link'>
      <a class='home-link' expr:href='data:desktopLinkUrl'><data:desktopLinkMsg/></a>
    </div>

  </div>
  <div class='clear'/>
</b:includable>
  <b:includable id='mobile-post' var='post'>
  <div class='date-outer'>
    <b:if cond='data:post.dateHeader'>
      <h2 class='date-header'><span><data:post.dateHeader/></span></h2>
    </b:if>
    <div class='date-posts'>
      <div class='post-outer'>

        <div class='post hentry uncustomized-post-template'>
          <a expr:name='data:post.id'/>
          <b:if cond='data:post.title'>
            <h1 class='post-title entry-title'>
              <b:if cond='data:post.link'>
                <a expr:href='data:post.link'><data:post.title/></a>
              <b:else/>
                <b:if cond='data:post.url'>
                  <b:if cond='data:blog.url != data:post.url'>
                    <a expr:href='data:post.url'><data:post.title/></a>
                  <b:else/>
                    <data:post.title/>
                  </b:if>
                <b:else/>
                  <data:post.title/>
                </b:if>
              </b:if>
            </h1>
          </b:if>

          <div class='post-header'>
            <div class='post-header-line-1'/>
          </div>

          <div class='post-body entry-content' expr:id='&quot;post-body-&quot; + data:post.id'>
            <data:post.body/>
            <div style='clear: both;'/> <!-- clear for photos floats -->
          </div>

          <div class='post-footer'>
            <div class='post-footer-line post-footer-line-1'>
              <span class='post-author vcard'>
                <b:if cond='data:top.showAuthor'>
                  <b:if cond='data:post.authorProfileUrl'>
                    <span class='fn'>
                      <a expr:href='data:post.authorProfileUrl' rel='author' title='author profile'>
                        <data:post.author/>
                      </a>
                    </span>
                  <b:else/>
                    <span class='fn'><data:post.author/></span>
                  </b:if>
                </b:if>
              </span>

              <span class='post-timestamp'>
                <b:if cond='data:top.showTimestamp'>
                  <data:top.timestampLabel/>
                  <b:if cond='data:post.url'>
                    <a class='timestamp-link' expr:href='data:post.url' rel='bookmark' title='permanent link'><abbr class='published' expr:title='data:post.timestampISO8601'><data:post.timestamp/></abbr></a>
                  </b:if>
                </b:if>
              </span>

              <span class='post-comment-link'>
                <b:if cond='data:blog.pageType != &quot;item&quot;'>
                  <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
                    <b:if cond='data:post.allowComments'>
                      <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><b:if cond='data:post.numComments == 1'>1 <data:top.commentLabel/><b:else/><data:post.numComments/> <data:top.commentLabelPlural/></b:if></a>
                    </b:if>
                  </b:if>
                </b:if>
              </span>
            </div>

            <div class='post-footer-line post-footer-line-2'>
              <b:if cond='data:top.showMobileShare'>
                <div class='mobile-link-button goog-inline-block' id='mobile-share-button'>
                  <a href='javascript:void(0);'><data:shareMsg/></a>
                </div>
              </b:if>
              <b:if cond='data:top.showDummy'>
                <div class='goog-inline-block dummy-container'><data:post.dummyTag/></div>
              </b:if>
            </div>

          </div>
        </div>
        <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
          <b:include data='post' name='comment_picker'/>
        </b:if>
        <b:if cond='data:blog.pageType == &quot;item&quot;'>
          <b:include data='post' name='comment_picker'/>
        </b:if>
      </div>
    </div>
  </div>
</b:includable>
  <b:includable id='nextprev'>
  <div class='blog-pager' id='blog-pager'>
    <b:if cond='data:newerPageUrl'>
      <span id='blog-pager-newer-link'>
        <span class='newer-text'>Next Post</span><a class='blog-pager-newer-link' expr:href='data:newerPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-newer-link&quot;' expr:title='data:newerPageTitle'><data:newerPageTitle/></a>
      </span>
    </b:if>

    <b:if cond='data:olderPageUrl'>
      <span id='blog-pager-older-link'>
        <span class='older-text'>Previous Post</span><a class='blog-pager-older-link' expr:href='data:olderPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-older-link&quot;' expr:title='data:olderPageTitle'><data:olderPageTitle/></a>
      </span>
    </b:if>

    <a class='home-link' expr:href='data:blog.homepageUrl'><data:homeMsg/></a>

    <b:if cond='data:mobileLinkUrl'>
      <div class='blog-mobile-link'>
        <a expr:href='data:mobileLinkUrl'><data:mobileLinkMsg/></a>
      </div>
    </b:if>

  </div>
  <div class='clear'/>
</b:includable>
  <b:includable id='post' var='post'>
  <div class='post hentry'>
	<b:if cond='data:post.firstImageUrl'>
      <meta expr:content='data:post.firstImageUrl' itemprop='image_url'/>
    </b:if>
    <meta expr:content='data:blog.blogId' itemprop='blogId'/>
    <meta expr:content='data:post.id' itemprop='postId'/>

<b:if cond='data:blog.pageType == &quot;item&quot;'>
<div class='post-header'>
	<div class='post-category'>
       <b:if cond='data:post.labels'>
          <b:loop values='data:post.labels' var='label'>
            <a expr:href='data:label.url' rel='tag'><data:label.name/></a><b:if cond='not data:label.isLast'/>
          </b:loop>
        </b:if>
    </div>

	<b:if cond='data:post.title'>
	<h1 class='post-title entry-title'>
	<b:if cond='data:post.link'>       
	<a expr:href='data:post.link'><data:post.title/></a>    
	<b:else/>
	<b:if cond='data:post.url'>
 	<b:if cond='data:blog.url != data:post.url'>
	<a expr:href='data:post.url'><data:post.title/></a>
	<b:else/>
	<data:post.title/>
	</b:if>
	<b:else/>
	<data:post.title/>
	</b:if>
	</b:if>
	</h1>
 	</b:if>


	<div class='post-meta'>
		<div class='post-date'>
        <b:if cond='data:top.showTimestamp'>
          <b:if cond='data:post.url'>
            <meta expr:content='data:post.canonicalUrl' itemprop='url'/>
            <span>posted on </span><time class='published' expr:title='data:post.timestampISO8601' itemprop='datePublished'><data:post.timestamp/></time>
          </b:if>
        </b:if>
    	</div><!-- post-date -->
  		<div class='post-author vcard'>
      	 	<b:if cond='data:top.showAuthor'>
            	<span>by</span>
            		<b:if cond='data:post.authorProfileUrl'>
             	 	<span class='fn' itemprop='author' itemscope='itemscope' itemtype='http://schema.org/Person'>
               	 		<meta expr:content='data:post.authorProfileUrl' itemprop='url'/>
               	 			<a class='g-profile' expr:href='data:post.authorProfileUrl' rel='author' title='author profile'>
                  				<span itemprop='name'><data:post.author/></span>
                			</a>
             	 	</span>
              <b:else/>
               	 <span class='fn' itemprop='author' itemscope='itemscope' itemtype='http://schema.org/Person'>
                	<span itemprop='name'><data:post.author/></span>
              	</span>
            </b:if>
        </b:if>
    	</div><!-- post-author -->

		<b:if cond='data:post.allowComments'>
			<div class='post-comment'>
              <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><b:if cond='data:post.numComments == 0'>Leave a Comment</b:if><b:if cond='data:post.numComments == 1'>1 comment</b:if><b:if cond='data:post.numComments &gt;= 2'><data:post.numComments/> comments</b:if></a>
      		</div>
        </b:if>

	</div>
  </div>
</b:if>

<b:if cond='data:blog.pageType == &quot;static_page&quot;'>
<b:if cond='data:post.title'>
<h2 class='post-title entry-title'>
<b:if cond='data:post.link'>
<a expr:href='data:post.link'><data:post.title/></a>  
<b:else/>
<b:if cond='data:post.url'>
<b:if cond='data:blog.url != data:post.url'>
<a expr:href='data:post.url'><data:post.title/></a>
<b:else/>
<data:post.title/>
</b:if>
<b:else/>
<data:post.title/>
</b:if>
</b:if>
</h2>
</b:if>
</b:if>


    <div class='post-body entry-content' expr:id='&quot;post-body-&quot; + data:post.id'>
      <b:if cond='data:blog.pageType == &quot;item&quot;'>
<data:post.body/>
<b:else/>
<b:if cond='data:blog.pageType == &quot;static_page&quot;'>
<data:post.body/>
<b:else/>
<div expr:id='&quot;p&quot; + data:post.id'>
<data:post.body/>
</div>
<script type='text/javascript'>
rm(&quot;p<data:post.id/>&quot;,&quot;<data:post.url/>&quot;,&quot;<data:post.title/>&quot;,&quot;<data:post.timestamp/>&quot;,&quot;<data:post.author/>&quot;,&quot;<b:loop values='data:post.labels' var='label'><a expr:class='data:label.name' expr:href='data:label.url + &quot;?max-results=6&quot;' rel='tag'><data:label.name/></a></b:loop>&quot;);
</script>

</b:if>
</b:if>
      <div style='clear: both;'/> <!-- clear for photos floats -->
    </div>


<!-- @social_share_icons -->
<div class='share-wrapper'>	
<ul class='entry-share-list clearfix'>

<li class='facebook_share'>
<a expr:href='&quot;http://www.facebook.com/sharer.php?u=&quot; + data:post.url + &quot;&amp;title=&quot;+ data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=550, height=600, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-facebook-square'/> <span class='share-text'>Facebook</span></a>
</li>
<li class='twitter_share'>
<a expr:href='&quot;http://twitter.com/share?url=&quot; + data:post.url + &quot;&amp;title=&quot; + data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=550, height=600, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-twitter'/> <span class='share-text'>Twitter</span></a>
</li>
<li class='google_share'>
<a expr:href='&quot;https://plus.google.com/share?url=&quot; + data:post.url + &quot;&amp;title=&quot; + data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=550, height=600, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-google-plus-square'/><span class='share-text'>Google+</span></a>
</li>
<li class='linkedin_share'>
<a expr:href='&quot;http://www.linkedin.com/shareArticle?mini=true&amp;url=&quot; + data:post.url + &quot;&amp;title=&quot;+ data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=550, height=600, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-linkedin'/><span class='share-text'>Linkedin</span></a>
</li>
<li><a expr:href='&quot;http://pinterest.com/pin/create/button/?url=&quot; + data:post.url + &quot;&amp;media=&quot; + data:post.thumbnailUrl + &quot;&amp;description=&quot; + data:post.snippet' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=550, height=600, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow'><i class='fa fa-pinterest-square'/><span class='share-text'>Pin It</span></a></li>


</ul><!-- .entry-share-icons -->
</div>


<b:if cond='data:blog.pageType == &quot;item&quot;'>
<div class='post-footer'>

<!-- blog_post_author_profile -->    
<div class='authorboxwrap'>
<div class='authorboxfull'>
<div class='avatar-container'>
<a href=''>
<img class='author_avatar img-circle' expr:alt='data:post.author' expr:src='data:post.authorPhoto.url' height='96' width='96'/>
</a>
</div>
<div class='author_description_container'>
<h4><a href='#' rel='author'><data:post.author/></a></h4>
<p>
<data:post.authorAboutMe/>       
</p>
</div>
</div>
</div>






<!-- @related-posts -->
<div id='related-posts'>
<script type='text/javascript'>//<![CDATA[
var ry="<h5>Related Posts</h5>";rn="<h5>No related post available</h5>";rcomment="comments";rdisable="disable comments";commentYN="no";var dw="";titles=new Array;titlesNum=0;urls=new Array;timeR=new Array;thumb=new Array;commentsNum=new Array;comments=new Array;
function related_results_labels(c){for(var b=0;b<c.feed.entry.length;b++){var d=c.feed.entry[b];titles[titlesNum]=d.title.$t;for(var a=0;a<d.link.length;a++){if("thr$total"in d)commentsNum[titlesNum]=d.thr$total.$t+" "+rcomment;else commentsNum[titlesNum]=rdisable;if(d.link[a].rel=="alternate"){urls[titlesNum]=d.link[a].href;timeR[titlesNum]=d.published.$t;if("media$thumbnail"in d)thumb[titlesNum]=d.media$thumbnail.url;else thumb[titlesNum]="http://lh3.ggpht.com/--Z8SVBQZ4X8/TdDxPVMl_sI/AAAAAAAAAAA/jhAgjCpZtRQ/no-image.png";
titlesNum++;break}}}}function removeRelatedDuplicates(){var b=new Array(0);c=new Array(0);e=new Array(0);f=new Array(0);g=new Array(0);for(var a=0;a<urls.length;a++)if(!contains(b,urls[a])){b.length+=1;b[b.length-1]=urls[a];c.length+=1;c[c.length-1]=titles[a];e.length+=1;e[e.length-1]=timeR[a];f.length+=1;f[f.length-1]=thumb[a];g.length+=1;g[g.length-1]=commentsNum[a]}urls=b;titles=c;timeR=e;thumb=f;commentsNum=g}
function contains(b,d){for(var c=0;c<b.length;c++)if(b[c]==d)return true;return false}
function printRelatedLabels(a){var y=a.indexOf("?m=0");if(y!=-1)a=a.replace(/\?m=0/g,"");for(var b=0;b<urls.length;b++)if(urls[b]==a){urls.splice(b,1);titles.splice(b,1);timeR.splice(b,1);thumb.splice(b,1);commentsNum.splice(b,1)}var c=Math.floor((titles.length-1)*Math.random());var b=0;if(titles.length==0)dw+=rn;else{dw+=ry;dw+="<ul>";while(b<titles.length&&b<20&&b<maxresults){if(y!=-1)urls[c]=urls[c]+"?m=0";if(commentYN=="yes")comments[c]=" - "+commentsNum[c];else comments[c]="";dw+='<li class="related_gallery"><a href="'+
urls[c]+'" title="'+titles[c]+'" rel="nofollow" class="related-thumbs"><img alt="'+titles[c]+'" src="'+thumb[c].replace(/\/s72\-c/,"/s"+size+"")+'"/></a><a class="related-title" href="'+urls[c]+'">'+titles[c]+"</a></li></div>";if(c<titles.length-1)c++;else c=0;b++}dw+="</ul>"}urls.splice(0,urls.length);titles.splice(0,titles.length);document.getElementById("related-posts").innerHTML=dw};
//]]></script>
<b:loop values='data:post.labels' var='label'>
<script expr:src='&quot;/feeds/posts/default/-/&quot; + data:label.name + &quot;?alt=json-in-script&amp;callback=related_results_labels&quot;' type='text/javascript'/>
</b:loop>
<script type='text/javascript'>
var maxresults=3;
var size = 250;
removeRelatedDuplicates();
printRelatedLabels(&#39;<data:post.url/>&#39;);</script>
</div>

<div class='post-footer-line post-footer-line-2'>

 </div>

      <div class='post-footer-line post-footer-line-3'><span class='post-location'>
        <b:if cond='data:top.showLocation'>
          <b:if cond='data:post.location'>
            <data:postLocationLabel/>
            <a expr:href='data:post.location.mapsUrl' target='_blank'><data:post.location.name/></a>
          </b:if>
        </b:if>
      </span> </div>
    </div>
</b:if>


  </div>
</b:includable>
  <b:includable id='postQuickEdit' var='post'>
  <b:if cond='data:post.editUrl'>
    <span expr:class='&quot;item-control &quot; + data:post.adminClass'>
      <a expr:href='data:post.editUrl' expr:title='data:top.editPostMsg'>
        <img alt='' class='icon-action' height='18' src='http://img2.blogblog.com/img/icon18_edit_allbkg.gif' width='18'/>
      </a>
    </span>
  </b:if>
</b:includable>
  <b:includable id='shareButtons' var='post'>
  <b:if cond='data:top.showEmailButton'><a class='goog-inline-block share-button sb-email' expr:href='data:post.sharePostUrl + &quot;&amp;target=email&quot;' expr:title='data:top.emailThisMsg' target='_blank'><span class='share-button-link-text'><data:top.emailThisMsg/></span></a></b:if><b:if cond='data:top.showBlogThisButton'><a class='goog-inline-block share-button sb-blog' expr:href='data:post.sharePostUrl + &quot;&amp;target=blog&quot;' expr:onclick='&quot;window.open(this.href, \&quot;_blank\&quot;, \&quot;height=270,width=475\&quot;); return false;&quot;' expr:title='data:top.blogThisMsg' target='_blank'><span class='share-button-link-text'><data:top.blogThisMsg/></span></a></b:if><b:if cond='data:top.showTwitterButton'><a class='goog-inline-block share-button sb-twitter' expr:href='data:post.sharePostUrl + &quot;&amp;target=twitter&quot;' expr:title='data:top.shareToTwitterMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToTwitterMsg/></span></a></b:if><b:if cond='data:top.showFacebookButton'><a class='goog-inline-block share-button sb-facebook' expr:href='data:post.sharePostUrl + &quot;&amp;target=facebook&quot;' expr:onclick='&quot;window.open(this.href, \&quot;_blank\&quot;, \&quot;height=430,width=640\&quot;); return false;&quot;' expr:title='data:top.shareToFacebookMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToFacebookMsg/></span></a></b:if><b:if cond='data:top.showOrkutButton'><a class='goog-inline-block share-button sb-orkut' expr:href='data:post.sharePostUrl + &quot;&amp;target=orkut&quot;' expr:title='data:top.shareToOrkutMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToOrkutMsg/></span></a></b:if><b:if cond='data:top.showDummy'><div class='goog-inline-block dummy-container'><data:post.dummyTag/></div></b:if>
</b:includable>
  <b:includable id='status-message'>
  <b:if cond='data:navMessage'>
  <div class='status-msg-wrap'>
    <div class='status-msg-body'>
      <data:navMessage/>
    </div>
    <div class='status-msg-border'>
      <div class='status-msg-bg'>
        <div class='status-msg-hidden'><data:navMessage/></div>
      </div>
    </div>
  </div>
  <div style='clear: both;'/>
  </b:if>
</b:includable>
  <b:includable id='threaded-comment-form' var='post'>
  <div class='comment-form'>
    <a name='comment-form'/>
    <b:if cond='data:mobile'>
      <p><data:blogCommentMessage/></p>
      <data:blogTeamBlogMessage/>
      <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
      <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='410' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
    <b:else/>
      <p><data:blogCommentMessage/></p>
      <data:blogTeamBlogMessage/>
      <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
      <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='410' id='comment-editor' name='comment-editor' src='' width='100%'/>
    </b:if>
    <data:post.friendConnectJs/>
    <data:post.cmtfpIframe/>
    <script type='text/javascript'>
      BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;, &#39;<data:post.communityId/>&#39;);
    </script>
  </div>
</b:includable>
  <b:includable id='threaded_comment_css'>
  <style>

  </style>
</b:includable>
  <b:includable id='threaded_comment_js' var='post'>
  <script async='async' expr:src='data:post.commentSrc' type='text/javascript'/>

  <script type='text/javascript'>
    (function() {
      var items = <data:post.commentJso/>;
      var msgs = <data:post.commentMsgs/>;
      var config = <data:post.commentConfig/>;

// <![CDATA[
      var cursor = null;
      if (items && items.length > 0) {
        cursor = parseInt(items[items.length - 1].timestamp) + 1;
      }
      var bodyFromEntry = function(entry) {
        if (entry.gd$extendedProperty) {
          for (var k in entry.gd$extendedProperty) {
            if (entry.gd$extendedProperty[k].name == 'blogger.contentRemoved') {
              return '<span class="deleted-comment">' + entry.content.$t + '</span>';
            }
          }
        }
        return entry.content.$t;
      }
      var parse = function(data) {
        cursor = null;
        var comments = [];
        if (data && data.feed && data.feed.entry) {
          for (var i = 0, entry; entry = data.feed.entry[i]; i++) {
            var comment = {};
            // comment ID, parsed out of the original id format
            var id = /blog-(\d+).post-(\d+)/.exec(entry.id.$t);
            comment.id = id ? id[2] : null;
            comment.body = bodyFromEntry(entry);
            comment.timestamp = Date.parse(entry.published.$t) + '';
            if (entry.author && entry.author.constructor === Array) {
              var auth = entry.author[0];
              if (auth) {
                comment.author = {
                  name: (auth.name ? auth.name.$t : undefined),
                  profileUrl: (auth.uri ? auth.uri.$t : undefined),
                  avatarUrl: (auth.gd$image ? auth.gd$image.src : undefined)
                };
              }
            }
            if (entry.link) {
              if (entry.link[2]) {
                comment.link = comment.permalink = entry.link[2].href;
              }
              if (entry.link[3]) {
                var pid = /.*comments\/default\/(\d+)\?.*/.exec(entry.link[3].href);
                if (pid && pid[1]) {
                  comment.parentId = pid[1];
                }
              }
            }
            comment.deleteclass = 'item-control blog-admin';
            if (entry.gd$extendedProperty) {
              for (var k in entry.gd$extendedProperty) {
                if (entry.gd$extendedProperty[k].name == 'blogger.itemClass') {
                  comment.deleteclass += ' ' + entry.gd$extendedProperty[k].value;
                } else if (entry.gd$extendedProperty[k].name == 'blogger.displayTime') {
                  comment.displayTime = entry.gd$extendedProperty[k].value;
                }
              }
            }
            comments.push(comment);
          }
        }
        return comments;
      };
      var paginator = function(callback) {
        if (hasMore()) {
          var url = config.feed + '?alt=json&v=2&orderby=published&reverse=false&max-results=50';
          if (cursor) {
            url += '&published-min=' + new Date(cursor).toISOString();
          }
          window.bloggercomments = function(data) {
            var parsed = parse(data);
            cursor = parsed.length < 50 ? null
                : parseInt(parsed[parsed.length - 1].timestamp) + 1
            callback(parsed);
            window.bloggercomments = null;
          }
          url += '&callback=bloggercomments';
          var script = document.createElement('script');
          script.type = 'text/javascript';
          script.src = url;
          document.getElementsByTagName('head')[0].appendChild(script);
        }
      };
      var hasMore = function() {
        return !!cursor;
      };
      var getMeta = function(key, comment) {
        if ('iswriter' == key) {
          var matches = !!comment.author
              && comment.author.name == config.authorName
              && comment.author.profileUrl == config.authorUrl;
          return matches ? 'true' : '';
        } else if ('deletelink' == key) {
          return config.baseUri + '/delete-comment.g?blogID='
               + config.blogId + '&postID=' + comment.id;
        } else if ('deleteclass' == key) {
          return comment.deleteclass;
        }
        return '';
      };
      var replybox = null;
      var replyUrlParts = null;
      var replyParent = undefined;
      var onReply = function(commentId, domId) {
        if (replybox == null) {
          // lazily cache replybox, and adjust to suit this style:
          replybox = document.getElementById('comment-editor');
          if (replybox != null) {
            replybox.height = '250px';
            replybox.style.display = 'block';
            replyUrlParts = replybox.src.split('#');
          }
        }
        if (replybox && (commentId !== replyParent)) {
          document.getElementById(domId).insertBefore(replybox, null);
          replybox.src = replyUrlParts[0]
              + (commentId ? '&parentID=' + commentId : '')
              + '#' + replyUrlParts[1];
          replyParent = commentId;
        }
      };
      var hash = (window.location.hash || '#').substring(1);
      var startThread, targetComment;
      if (/^comment-form_/.test(hash)) {
        startThread = hash.substring('comment-form_'.length);
      } else if (/^c[0-9]+$/.test(hash)) {
        targetComment = hash.substring(1);
      }
      // Configure commenting API:
      var configJso = {
        'maxDepth': config.maxThreadDepth
      };
      var provider = {
        'id': config.postId,
        'data': items,
        'loadNext': paginator,
        'hasMore': hasMore,
        'getMeta': getMeta,
        'onReply': onReply,
        'rendered': true,
        'initComment': targetComment,
        'initReplyThread': startThread,
        'config': configJso,
        'messages': msgs
      };
      var render = function() {
        if (window.goog && window.goog.comments) {
          var holder = document.getElementById('comment-holder');
          window.goog.comments.render(holder, provider);
        }
      };
      // render now, or queue to render when library loads:
      if (window.goog && window.goog.comments) {
        render();
      } else {
        window.goog = window.goog || {};
        window.goog.comments = window.goog.comments || {};
        window.goog.comments.loadQueue = window.goog.comments.loadQueue || [];
        window.goog.comments.loadQueue.push(render);
      }
    })();
// ]]>
  </script>
</b:includable>
  <b:includable id='threaded_comments' var='post'>
  <div class='comments' id='comments'>
    <a name='comments'/>
    <h4><data:post.commentLabelFull/>:</h4>

    <div class='comments-content'>
      <b:include cond='data:post.embedCommentForm' data='post' name='threaded_comment_js'/>
      <div id='comment-holder'>
         <data:post.commentHtml/>
      </div>
    </div>

    <p class='comment-footer'>
      <b:if cond='data:post.allowNewComments'>
        <b:include data='post' name='threaded-comment-form'/>
      <b:else/>
        <data:post.noNewCommentsText/>
      </b:if>
    </p>

    <b:if cond='data:showCmtPopup'>
      <div id='comment-popup'>
        <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'>
        </iframe>
      </div>
    </b:if>

    <div id='backlinks-container'>
    <div expr:id='data:widget.instanceId + &quot;_backlinks-container&quot;'>
      <b:include cond='data:post.showBacklinks' data='post' name='backlinks'/>
    </div>
    </div>
  </div>
</b:includable>
</b:widget>
</b:section>
        </div><!-- /main-wrapper -->

        <div class='sidebar-wrapper'>
        	<b:section class='sidebar' id='sidebar' showaddelement='yes'/>     
        </div><!-- /sidebar-wrapper -->

        <div class='clr'/>
    </div>
</div>


<!-- __ FOOTER __ -->

<div class='footer_bottom'>
<div class='toTop'>
            <a href='#header-inner' id='smooth_scroll'><i class='fa fa-chevron-up'/></a>
        </div>

<div class='ct-wrapper'>

<div class='footerLogo'>

<b:section class='header' id='Footer-header' maxwidgets='1' showaddelement='yes'>
  <b:widget id='Header2' locked='true' title='Storyteller (Header)' type='Header' version='1'>
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
          <div expr:style='&quot;background-image: url(\&quot;&quot; + data:sourceUrl + &quot;\&quot;); &quot;                        + &quot;background-position: &quot;                        + data:backgroundPositionStyleStr + &quot;; &quot;                        + data:widthStyleStr                        + &quot;min-height: &quot; + data:height                        + &quot;_height: &quot; + data:height                        + &quot;background-repeat: no-repeat; &quot;' id='header-inner'>
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
          <img expr:alt='data:title' expr:id='data:widget.instanceId + &quot;_headerimg&quot;' expr:src='data:sourceUrl' style='display: block'/>
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
    <a expr:href='data:blog.homepageUrl'><data:title/></a>
</b:includable>
  </b:widget>
</b:section>

<div vlass='clr'/>

<div class='contact_us'>
<a class='contact_link' href='/p/contact.html'>Contact</a>
</div>

<div class='clr'/>

<!-- footer-social-share -->
  <div class='bottom_share'>
    <a href='#'><i class='fa fa-facebook'/></a>
    <a href='#'><i class='fa fa-twitter'/></a>
    <a href='#'><i class='fa fa-google-plus'/></a>
    <a href='#'><i class='fa fa-dribbble'/></a>
    <a href='#'><i class='fa fa-instagram'/></a>
</div>

</div>

</div>

<p class='attribution'>&#169; Copyright 2015 <a expr:href='data:blog.homepageUrl'><data:blog.title/></a> Designed by <a href='//www.veethemes.co.in'>VeeThemes</a>, Powered by <a href='http://www.blogger.com/'>Blogger</a></p>     

</div>

<script type='text/javascript'>//<![CDATA[
/**
 * Owl Carousel v2.2.1
 * Copyright 2013-2017 David Deutsch
 * Licensed under  ()
 */
/**
 * Owl carousel
 * @version 2.1.6
 * @author Bartosz Wojciechowski
 * @author David Deutsch
 * @license The MIT License (MIT)
 * @todo Lazy Load Icon
 * @todo prevent animationend bubling
 * @todo itemsScaleUp
 * @todo Test Zepto
 * @todo stagePadding calculate wrong active classes
 */
!function(t,e,i,s){function n(e,i){this.settings=null,this.options=t.extend({},n.Defaults,i),this.$element=t(e),this._handlers={},this._plugins={},this._supress={},this._current=null,this._speed=null,this._coordinates=[],this._breakpoint=null,this._width=null,this._items=[],this._clones=[],this._mergers=[],this._widths=[],this._invalidated={},this._pipe=[],this._drag={time:null,target:null,pointer:null,stage:{start:null,current:null},direction:null},this._states={current:{},tags:{initializing:["busy"],animating:["busy"],dragging:["interacting"]}},t.each(["onResize","onThrottledResize"],t.proxy(function(e,i){this._handlers[i]=t.proxy(this[i],this)},this)),t.each(n.Plugins,t.proxy(function(t,e){this._plugins[t.charAt(0).toLowerCase()+t.slice(1)]=new e(this)},this)),t.each(n.Workers,t.proxy(function(e,i){this._pipe.push({filter:i.filter,run:t.proxy(i.run,this)})},this)),this.setup(),this.initialize()}n.Defaults={items:3,loop:!1,center:!1,rewind:!1,mouseDrag:!0,touchDrag:!0,pullDrag:!0,freeDrag:!1,margin:0,stagePadding:0,merge:!1,mergeFit:!0,autoWidth:!1,startPosition:0,rtl:!1,smartSpeed:250,fluidSpeed:!1,dragEndSpeed:!1,responsive:{},responsiveRefreshRate:200,responsiveBaseElement:e,fallbackEasing:"swing",info:!1,nestedItemSelector:!1,itemElement:"div",stageElement:"div",refreshClass:"owl-refresh",loadedClass:"owl-loaded",loadingClass:"owl-loading",rtlClass:"owl-rtl",responsiveClass:"owl-responsive",dragClass:"owl-drag",itemClass:"owl-item",stageClass:"owl-stage",stageOuterClass:"owl-stage-outer",grabClass:"owl-grab"},n.Width={Default:"default",Inner:"inner",Outer:"outer"},n.Type={Event:"event",State:"state"},n.Plugins={},n.Workers=[{filter:["width","settings"],run:function(){this._width=this.$element.width()}},{filter:["width","items","settings"],run:function(t){t.current=this._items&&this._items[this.relative(this._current)]}},{filter:["items","settings"],run:function(){this.$stage.children(".cloned").remove()}},{filter:["width","items","settings"],run:function(t){var e=this.settings.margin||"",i=!this.settings.autoWidth,s=this.settings.rtl,n={width:"auto","margin-left":s?e:"","margin-right":s?"":e};!i&&this.$stage.children().css(n),t.css=n}},{filter:["width","items","settings"],run:function(t){var e=(this.width()/this.settings.items).toFixed(3)-this.settings.margin,i=null,s=this._items.length,n=!this.settings.autoWidth,o=[];for(t.items={merge:!1,width:e};s--;)i=this._mergers[s],i=this.settings.mergeFit&&Math.min(i,this.settings.items)||i,t.items.merge=i>1||t.items.merge,o[s]=n?e*i:this._items[s].width();this._widths=o}},{filter:["items","settings"],run:function(){var e=[],i=this._items,s=this.settings,n=Math.max(2*s.items,4),o=2*Math.ceil(i.length/2),r=s.loop&&i.length?s.rewind?n:Math.max(n,o):0,a="",h="";for(r/=2;r--;)e.push(this.normalize(e.length/2,!0)),a+=i[e[e.length-1]][0].outerHTML,e.push(this.normalize(i.length-1-(e.length-1)/2,!0)),h=i[e[e.length-1]][0].outerHTML+h;this._clones=e,t(a).addClass("cloned").appendTo(this.$stage),t(h).addClass("cloned").prependTo(this.$stage)}},{filter:["width","items","settings"],run:function(){for(var t=this.settings.rtl?1:-1,e=this._clones.length+this._items.length,i=-1,s=0,n=0,o=[];++i<e;)s=o[i-1]||0,n=this._widths[this.relative(i)]+this.settings.margin,o.push(s+n*t);this._coordinates=o}},{filter:["width","items","settings"],run:function(){var t=this.settings.stagePadding,e=this._coordinates,i={width:Math.ceil(Math.abs(e[e.length-1]))+2*t,"padding-left":t||"","padding-right":t||""};this.$stage.css(i)}},{filter:["width","items","settings"],run:function(t){var e=this._coordinates.length,i=!this.settings.autoWidth,s=this.$stage.children();if(i&&t.items.merge)for(;e--;)t.css.width=this._widths[this.relative(e)],s.eq(e).css(t.css);else i&&(t.css.width=t.items.width,s.css(t.css))}},{filter:["items"],run:function(){this._coordinates.length<1&&this.$stage.removeAttr("style")}},{filter:["width","items","settings"],run:function(t){t.current=t.current?this.$stage.children().index(t.current):0,t.current=Math.max(this.minimum(),Math.min(this.maximum(),t.current)),this.reset(t.current)}},{filter:["position"],run:function(){this.animate(this.coordinates(this._current))}},{filter:["width","position","items","settings"],run:function(){var t,e,i,s,n=this.settings.rtl?1:-1,o=2*this.settings.stagePadding,r=this.coordinates(this.current())+o,a=r+this.width()*n,h=[];for(i=0,s=this._coordinates.length;s>i;i++)t=this._coordinates[i-1]||0,e=Math.abs(this._coordinates[i])+o*n,(this.op(t,"<=",r)&&this.op(t,">",a)||this.op(e,"<",r)&&this.op(e,">",a))&&h.push(i);this.$stage.children(".active").removeClass("active"),this.$stage.children(":eq("+h.join("), :eq(")+")").addClass("active"),this.settings.center&&(this.$stage.children(".center").removeClass("center"),this.$stage.children().eq(this.current()).addClass("center"))}}],n.prototype.initialize=function(){if(this.enter("initializing"),this.trigger("initialize"),this.$element.toggleClass(this.settings.rtlClass,this.settings.rtl),this.settings.autoWidth&&!this.is("pre-loading")){var e,i,n;e=this.$element.find("img"),i=this.settings.nestedItemSelector?"."+this.settings.nestedItemSelector:s,n=this.$element.children(i).width(),e.length&&0>=n&&this.preloadAutoWidthImages(e)}this.$element.addClass(this.options.loadingClass),this.$stage=t("<"+this.settings.stageElement+' class="'+this.settings.stageClass+'"/>').wrap('<div class="'+this.settings.stageOuterClass+'"/>'),this.$element.append(this.$stage.parent()),this.replace(this.$element.children().not(this.$stage.parent())),this.$element.is(":visible")?this.refresh():this.invalidate("width"),this.$element.removeClass(this.options.loadingClass).addClass(this.options.loadedClass),this.registerEventHandlers(),this.leave("initializing"),this.trigger("initialized")},n.prototype.setup=function(){var e=this.viewport(),i=this.options.responsive,s=-1,n=null;i?(t.each(i,function(t){e>=t&&t>s&&(s=Number(t))}),n=t.extend({},this.options,i[s]),"function"==typeof n.stagePadding&&(n.stagePadding=n.stagePadding()),delete n.responsive,n.responsiveClass&&this.$element.attr("class",this.$element.attr("class").replace(new RegExp("("+this.options.responsiveClass+"-)\\S+\\s","g"),"$1"+s))):n=t.extend({},this.options),this.trigger("change",{property:{name:"settings",value:n}}),this._breakpoint=s,this.settings=n,this.invalidate("settings"),this.trigger("changed",{property:{name:"settings",value:this.settings}})},n.prototype.optionsLogic=function(){this.settings.autoWidth&&(this.settings.stagePadding=!1,this.settings.merge=!1)},n.prototype.prepare=function(e){var i=this.trigger("prepare",{content:e});return i.data||(i.data=t("<"+this.settings.itemElement+"/>").addClass(this.options.itemClass).append(e)),this.trigger("prepared",{content:i.data}),i.data},n.prototype.update=function(){for(var e=0,i=this._pipe.length,s=t.proxy(function(t){return this[t]},this._invalidated),n={};i>e;)(this._invalidated.all||t.grep(this._pipe[e].filter,s).length>0)&&this._pipe[e].run(n),e++;this._invalidated={},!this.is("valid")&&this.enter("valid")},n.prototype.width=function(t){switch(t=t||n.Width.Default){case n.Width.Inner:case n.Width.Outer:return this._width;default:return this._width-2*this.settings.stagePadding+this.settings.margin}},n.prototype.refresh=function(){this.enter("refreshing"),this.trigger("refresh"),this.setup(),this.optionsLogic(),this.$element.addClass(this.options.refreshClass),this.update(),this.$element.removeClass(this.options.refreshClass),this.leave("refreshing"),this.trigger("refreshed")},n.prototype.onThrottledResize=function(){e.clearTimeout(this.resizeTimer),this.resizeTimer=e.setTimeout(this._handlers.onResize,this.settings.responsiveRefreshRate)},n.prototype.onResize=function(){return this._items.length?this._width===this.$element.width()?!1:this.$element.is(":visible")?(this.enter("resizing"),this.trigger("resize").isDefaultPrevented()?(this.leave("resizing"),!1):(this.invalidate("width"),this.refresh(),this.leave("resizing"),void this.trigger("resized"))):!1:!1},n.prototype.registerEventHandlers=function(){t.support.transition&&this.$stage.on(t.support.transition.end+".owl.core",t.proxy(this.onTransitionEnd,this)),this.settings.responsive!==!1&&this.on(e,"resize",this._handlers.onThrottledResize),this.settings.mouseDrag&&(this.$element.addClass(this.options.dragClass),this.$stage.on("mousedown.owl.core",t.proxy(this.onDragStart,this)),this.$stage.on("dragstart.owl.core selectstart.owl.core",function(){return!1})),this.settings.touchDrag&&(this.$stage.on("touchstart.owl.core",t.proxy(this.onDragStart,this)),this.$stage.on("touchcancel.owl.core",t.proxy(this.onDragEnd,this)))},n.prototype.onDragStart=function(e){var s=null;3!==e.which&&(t.support.transform?(s=this.$stage.css("transform").replace(/.*\(|\)| /g,"").split(","),s={x:s[16===s.length?12:4],y:s[16===s.length?13:5]}):(s=this.$stage.position(),s={x:this.settings.rtl?s.left+this.$stage.width()-this.width()+this.settings.margin:s.left,y:s.top}),this.is("animating")&&(t.support.transform?this.animate(s.x):this.$stage.stop(),this.invalidate("position")),this.$element.toggleClass(this.options.grabClass,"mousedown"===e.type),this.speed(0),this._drag.time=(new Date).getTime(),this._drag.target=t(e.target),this._drag.stage.start=s,this._drag.stage.current=s,this._drag.pointer=this.pointer(e),t(i).on("mouseup.owl.core touchend.owl.core",t.proxy(this.onDragEnd,this)),t(i).one("mousemove.owl.core touchmove.owl.core",t.proxy(function(e){var s=this.difference(this._drag.pointer,this.pointer(e));t(i).on("mousemove.owl.core touchmove.owl.core",t.proxy(this.onDragMove,this)),Math.abs(s.x)<Math.abs(s.y)&&this.is("valid")||(e.preventDefault(),this.enter("dragging"),this.trigger("drag"))},this)))},n.prototype.onDragMove=function(t){var e=null,i=null,s=null,n=this.difference(this._drag.pointer,this.pointer(t)),o=this.difference(this._drag.stage.start,n);this.is("dragging")&&(t.preventDefault(),this.settings.loop?(e=this.coordinates(this.minimum()),i=this.coordinates(this.maximum()+1)-e,o.x=((o.x-e)%i+i)%i+e):(e=this.settings.rtl?this.coordinates(this.maximum()):this.coordinates(this.minimum()),i=this.settings.rtl?this.coordinates(this.minimum()):this.coordinates(this.maximum()),s=this.settings.pullDrag?-1*n.x/5:0,o.x=Math.max(Math.min(o.x,e+s),i+s)),this._drag.stage.current=o,this.animate(o.x))},n.prototype.onDragEnd=function(e){var s=this.difference(this._drag.pointer,this.pointer(e)),n=this._drag.stage.current,o=s.x>0^this.settings.rtl?"left":"right";t(i).off(".owl.core"),this.$element.removeClass(this.options.grabClass),(0!==s.x&&this.is("dragging")||!this.is("valid"))&&(this.speed(this.settings.dragEndSpeed||this.settings.smartSpeed),this.current(this.closest(n.x,0!==s.x?o:this._drag.direction)),this.invalidate("position"),this.update(),this._drag.direction=o,(Math.abs(s.x)>3||(new Date).getTime()-this._drag.time>300)&&this._drag.target.one("click.owl.core",function(){return!1})),this.is("dragging")&&(this.leave("dragging"),this.trigger("dragged"))},n.prototype.closest=function(e,i){var s=-1,n=30,o=this.width(),r=this.coordinates();return this.settings.freeDrag||t.each(r,t.proxy(function(t,a){return"left"===i&&e>a-n&&a+n>e?s=t:"right"===i&&e>a-o-n&&a-o+n>e?s=t+1:this.op(e,"<",a)&&this.op(e,">",r[t+1]||a-o)&&(s="left"===i?t+1:t),-1===s},this)),this.settings.loop||(this.op(e,">",r[this.minimum()])?s=e=this.minimum():this.op(e,"<",r[this.maximum()])&&(s=e=this.maximum())),s},n.prototype.animate=function(e){var i=this.speed()>0;this.is("animating")&&this.onTransitionEnd(),i&&(this.enter("animating"),this.trigger("translate")),t.support.transform3d&&t.support.transition?this.$stage.css({transform:"translate3d("+e+"px,0px,0px)",transition:this.speed()/1e3+"s"}):i?this.$stage.animate({left:e+"px"},this.speed(),this.settings.fallbackEasing,t.proxy(this.onTransitionEnd,this)):this.$stage.css({left:e+"px"})},n.prototype.is=function(t){return this._states.current[t]&&this._states.current[t]>0},n.prototype.current=function(t){if(t===s)return this._current;if(0===this._items.length)return s;if(t=this.normalize(t),this._current!==t){var e=this.trigger("change",{property:{name:"position",value:t}});e.data!==s&&(t=this.normalize(e.data)),this._current=t,this.invalidate("position"),this.trigger("changed",{property:{name:"position",value:this._current}})}return this._current},n.prototype.invalidate=function(e){return"string"===t.type(e)&&(this._invalidated[e]=!0,this.is("valid")&&this.leave("valid")),t.map(this._invalidated,function(t,e){return e})},n.prototype.reset=function(t){t=this.normalize(t),t!==s&&(this._speed=0,this._current=t,this.suppress(["translate","translated"]),this.animate(this.coordinates(t)),this.release(["translate","translated"]))},n.prototype.normalize=function(t,e){var i=this._items.length,n=e?0:this._clones.length;return!this.isNumeric(t)||1>i?t=s:(0>t||t>=i+n)&&(t=((t-n/2)%i+i)%i+n/2),t},n.prototype.relative=function(t){return t-=this._clones.length/2,this.normalize(t,!0)},n.prototype.maximum=function(t){var e,i,s,n=this.settings,o=this._coordinates.length;if(n.loop)o=this._clones.length/2+this._items.length-1;else if(n.autoWidth||n.merge){for(e=this._items.length,i=this._items[--e].width(),s=this.$element.width();e--&&(i+=this._items[e].width()+this.settings.margin,!(i>s)););o=e+1}else o=n.center?this._items.length-1:this._items.length-n.items;return t&&(o-=this._clones.length/2),Math.max(o,0)},n.prototype.minimum=function(t){return t?0:this._clones.length/2},n.prototype.items=function(t){return t===s?this._items.slice():(t=this.normalize(t,!0),this._items[t])},n.prototype.mergers=function(t){return t===s?this._mergers.slice():(t=this.normalize(t,!0),this._mergers[t])},n.prototype.clones=function(e){var i=this._clones.length/2,n=i+this._items.length,o=function(t){return t%2===0?n+t/2:i-(t+1)/2};return e===s?t.map(this._clones,function(t,e){return o(e)}):t.map(this._clones,function(t,i){return t===e?o(i):null})},n.prototype.speed=function(t){return t!==s&&(this._speed=t),this._speed},n.prototype.coordinates=function(e){var i,n=1,o=e-1;return e===s?t.map(this._coordinates,t.proxy(function(t,e){return this.coordinates(e)},this)):(this.settings.center?(this.settings.rtl&&(n=-1,o=e+1),i=this._coordinates[e],i+=(this.width()-i+(this._coordinates[o]||0))/2*n):i=this._coordinates[o]||0,i=Math.ceil(i))},n.prototype.duration=function(t,e,i){return 0===i?0:Math.min(Math.max(Math.abs(e-t),1),6)*Math.abs(i||this.settings.smartSpeed)},n.prototype.to=function(t,e){var i=this.current(),s=null,n=t-this.relative(i),o=(n>0)-(0>n),r=this._items.length,a=this.minimum(),h=this.maximum();this.settings.loop?(!this.settings.rewind&&Math.abs(n)>r/2&&(n+=-1*o*r),t=i+n,s=((t-a)%r+r)%r+a,s!==t&&h>=s-n&&s-n>0&&(i=s-n,t=s,this.reset(i))):this.settings.rewind?(h+=1,t=(t%h+h)%h):t=Math.max(a,Math.min(h,t)),this.speed(this.duration(i,t,e)),this.current(t),this.$element.is(":visible")&&this.update()},n.prototype.next=function(t){t=t||!1,this.to(this.relative(this.current())+1,t)},n.prototype.prev=function(t){t=t||!1,this.to(this.relative(this.current())-1,t)},n.prototype.onTransitionEnd=function(t){return t!==s&&(t.stopPropagation(),(t.target||t.srcElement||t.originalTarget)!==this.$stage.get(0))?!1:(this.leave("animating"),void this.trigger("translated"))},n.prototype.viewport=function(){var s;return this.options.responsiveBaseElement!==e?s=t(this.options.responsiveBaseElement).width():e.innerWidth?s=e.innerWidth:i.documentElement&&i.documentElement.clientWidth?s=i.documentElement.clientWidth:console.warn("Can not detect viewport width."),s},n.prototype.replace=function(e){this.$stage.empty(),this._items=[],e&&(e=e instanceof jQuery?e:t(e)),this.settings.nestedItemSelector&&(e=e.find("."+this.settings.nestedItemSelector)),e.filter(function(){return 1===this.nodeType}).each(t.proxy(function(t,e){e=this.prepare(e),this.$stage.append(e),this._items.push(e),this._mergers.push(1*e.find("[data-merge]").addBack("[data-merge]").attr("data-merge")||1)},this)),this.reset(this.isNumeric(this.settings.startPosition)?this.settings.startPosition:0),this.invalidate("items")},n.prototype.add=function(e,i){var n=this.relative(this._current);i=i===s?this._items.length:this.normalize(i,!0),e=e instanceof jQuery?e:t(e),this.trigger("add",{content:e,position:i}),e=this.prepare(e),0===this._items.length||i===this._items.length?(0===this._items.length&&this.$stage.append(e),0!==this._items.length&&this._items[i-1].after(e),this._items.push(e),this._mergers.push(1*e.find("[data-merge]").addBack("[data-merge]").attr("data-merge")||1)):(this._items[i].before(e),this._items.splice(i,0,e),this._mergers.splice(i,0,1*e.find("[data-merge]").addBack("[data-merge]").attr("data-merge")||1)),this._items[n]&&this.reset(this._items[n].index()),this.invalidate("items"),this.trigger("added",{content:e,position:i})},n.prototype.remove=function(t){t=this.normalize(t,!0),t!==s&&(this.trigger("remove",{content:this._items[t],position:t}),this._items[t].remove(),this._items.splice(t,1),this._mergers.splice(t,1),this.invalidate("items"),this.trigger("removed",{content:null,position:t}))},n.prototype.preloadAutoWidthImages=function(e){e.each(t.proxy(function(e,i){this.enter("pre-loading"),i=t(i),t(new Image).one("load",t.proxy(function(t){i.attr("src",t.target.src),i.css("opacity",1),this.leave("pre-loading"),!this.is("pre-loading")&&!this.is("initializing")&&this.refresh()},this)).attr("src",i.attr("src")||i.attr("data-src")||i.attr("data-src-retina"))},this))},n.prototype.destroy=function(){this.$element.off(".owl.core"),this.$stage.off(".owl.core"),t(i).off(".owl.core"),this.settings.responsive!==!1&&(e.clearTimeout(this.resizeTimer),this.off(e,"resize",this._handlers.onThrottledResize));for(var s in this._plugins)this._plugins[s].destroy();this.$stage.children(".cloned").remove(),this.$stage.unwrap(),this.$stage.children().contents().unwrap(),this.$stage.children().unwrap(),this.$element.removeClass(this.options.refreshClass).removeClass(this.options.loadingClass).removeClass(this.options.loadedClass).removeClass(this.options.rtlClass).removeClass(this.options.dragClass).removeClass(this.options.grabClass).attr("class",this.$element.attr("class").replace(new RegExp(this.options.responsiveClass+"-\\S+\\s","g"),"")).removeData("owl.carousel")},n.prototype.op=function(t,e,i){var s=this.settings.rtl;switch(e){case"<":return s?t>i:i>t;case">":return s?i>t:t>i;case">=":return s?i>=t:t>=i;case"<=":return s?t>=i:i>=t}},n.prototype.on=function(t,e,i,s){t.addEventListener?t.addEventListener(e,i,s):t.attachEvent&&t.attachEvent("on"+e,i)},n.prototype.off=function(t,e,i,s){t.removeEventListener?t.removeEventListener(e,i,s):t.detachEvent&&t.detachEvent("on"+e,i)},n.prototype.trigger=function(e,i,s,o,r){var a={item:{count:this._items.length,index:this.current()}},h=t.camelCase(t.grep(["on",e,s],function(t){return t}).join("-").toLowerCase()),l=t.Event([e,"owl",s||"carousel"].join(".").toLowerCase(),t.extend({relatedTarget:this},a,i));return this._supress[e]||(t.each(this._plugins,function(t,e){e.onTrigger&&e.onTrigger(l)}),this.register({type:n.Type.Event,name:e}),this.$element.trigger(l),this.settings&&"function"==typeof this.settings[h]&&this.settings[h].call(this,l)),l},n.prototype.enter=function(e){t.each([e].concat(this._states.tags[e]||[]),t.proxy(function(t,e){this._states.current[e]===s&&(this._states.current[e]=0),this._states.current[e]++},this))},n.prototype.leave=function(e){t.each([e].concat(this._states.tags[e]||[]),t.proxy(function(t,e){this._states.current[e]--},this))},n.prototype.register=function(e){if(e.type===n.Type.Event){if(t.event.special[e.name]||(t.event.special[e.name]={}),!t.event.special[e.name].owl){var i=t.event.special[e.name]._default;t.event.special[e.name]._default=function(t){return!i||!i.apply||t.namespace&&-1!==t.namespace.indexOf("owl")?t.namespace&&t.namespace.indexOf("owl")>-1:i.apply(this,arguments)},t.event.special[e.name].owl=!0}}else e.type===n.Type.State&&(this._states.tags[e.name]?this._states.tags[e.name]=this._states.tags[e.name].concat(e.tags):this._states.tags[e.name]=e.tags,this._states.tags[e.name]=t.grep(this._states.tags[e.name],t.proxy(function(i,s){return t.inArray(i,this._states.tags[e.name])===s},this)))},n.prototype.suppress=function(e){t.each(e,t.proxy(function(t,e){this._supress[e]=!0},this))},n.prototype.release=function(e){t.each(e,t.proxy(function(t,e){delete this._supress[e]},this))},n.prototype.pointer=function(t){var i={x:null,y:null};return t=t.originalEvent||t||e.event,t=t.touches&&t.touches.length?t.touches[0]:t.changedTouches&&t.changedTouches.length?t.changedTouches[0]:t,t.pageX?(i.x=t.pageX,i.y=t.pageY):(i.x=t.clientX,i.y=t.clientY),i},n.prototype.isNumeric=function(t){return!isNaN(parseFloat(t))},n.prototype.difference=function(t,e){return{x:t.x-e.x,y:t.y-e.y}},t.fn.owlCarousel=function(e){var i=Array.prototype.slice.call(arguments,1);return this.each(function(){var s=t(this),o=s.data("owl.carousel");o||(o=new n(this,"object"==typeof e&&e),s.data("owl.carousel",o),t.each(["next","prev","to","destroy","refresh","replace","add","remove"],function(e,i){o.register({type:n.Type.Event,name:i}),o.$element.on(i+".owl.carousel.core",t.proxy(function(t){t.namespace&&t.relatedTarget!==this&&(this.suppress([i]),o[i].apply(this,[].slice.call(arguments,1)),this.release([i]))},o))})),"string"==typeof e&&"_"!==e.charAt(0)&&o[e].apply(o,i)})},t.fn.owlCarousel.Constructor=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){var n=function(e){this._core=e,this._interval=null,this._visible=null,this._handlers={"initialized.owl.carousel":t.proxy(function(t){t.namespace&&this._core.settings.autoRefresh&&this.watch()},this)},this._core.options=t.extend({},n.Defaults,this._core.options),this._core.$element.on(this._handlers)};n.Defaults={autoRefresh:!0,autoRefreshInterval:500},n.prototype.watch=function(){this._interval||(this._visible=this._core.$element.is(":visible"),this._interval=e.setInterval(t.proxy(this.refresh,this),this._core.settings.autoRefreshInterval))},n.prototype.refresh=function(){this._core.$element.is(":visible")!==this._visible&&(this._visible=!this._visible,this._core.$element.toggleClass("owl-hidden",!this._visible),this._visible&&this._core.invalidate("width")&&this._core.refresh())},n.prototype.destroy=function(){var t,i;e.clearInterval(this._interval);for(t in this._handlers)this._core.$element.off(t,this._handlers[t]);for(i in Object.getOwnPropertyNames(this))"function"!=typeof this[i]&&(this[i]=null)},t.fn.owlCarousel.Constructor.Plugins.AutoRefresh=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){var n=function(e){this._core=e,this._loaded=[],this._handlers={"initialized.owl.carousel change.owl.carousel resized.owl.carousel":t.proxy(function(e){if(e.namespace&&this._core.settings&&this._core.settings.lazyLoad&&(e.property&&"position"==e.property.name||"initialized"==e.type))for(var i=this._core.settings,n=i.center&&Math.ceil(i.items/2)||i.items,o=i.center&&-1*n||0,r=(e.property&&e.property.value!==s?e.property.value:this._core.current())+o,a=this._core.clones().length,h=t.proxy(function(t,e){this.load(e)},this);o++<n;)this.load(a/2+this._core.relative(r)),a&&t.each(this._core.clones(this._core.relative(r)),h),r++},this)},this._core.options=t.extend({},n.Defaults,this._core.options),this._core.$element.on(this._handlers)};n.Defaults={lazyLoad:!1},n.prototype.load=function(i){var s=this._core.$stage.children().eq(i),n=s&&s.find(".owl-lazy");!n||t.inArray(s.get(0),this._loaded)>-1||(n.each(t.proxy(function(i,s){var n,o=t(s),r=e.devicePixelRatio>1&&o.attr("data-src-retina")||o.attr("data-src");this._core.trigger("load",{element:o,url:r},"lazy"),o.is("img")?o.one("load.owl.lazy",t.proxy(function(){o.css("opacity",1),this._core.trigger("loaded",{element:o,url:r},"lazy")},this)).attr("src",r):(n=new Image,n.onload=t.proxy(function(){o.css({"background-image":'url("'+r+'")',opacity:"1"}),this._core.trigger("loaded",{element:o,url:r},"lazy")},this),n.src=r)},this)),this._loaded.push(s.get(0)))},n.prototype.destroy=function(){var t,e;for(t in this.handlers)this._core.$element.off(t,this.handlers[t]);for(e in Object.getOwnPropertyNames(this))"function"!=typeof this[e]&&(this[e]=null)},t.fn.owlCarousel.Constructor.Plugins.Lazy=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){var n=function(e){this._core=e,this._handlers={"initialized.owl.carousel refreshed.owl.carousel":t.proxy(function(t){t.namespace&&this._core.settings.autoHeight&&this.update()},this),"changed.owl.carousel":t.proxy(function(t){t.namespace&&this._core.settings.autoHeight&&"position"==t.property.name&&this.update()},this),"loaded.owl.lazy":t.proxy(function(t){t.namespace&&this._core.settings.autoHeight&&t.element.closest("."+this._core.settings.itemClass).index()===this._core.current()&&this.update()},this)},this._core.options=t.extend({},n.Defaults,this._core.options),this._core.$element.on(this._handlers)};n.Defaults={autoHeight:!1,autoHeightClass:"owl-height"},n.prototype.update=function(){var e=this._core._current,i=e+this._core.settings.items,s=this._core.$stage.children().toArray().slice(e,i),n=[],o=0;t.each(s,function(e,i){n.push(t(i).height())}),o=Math.max.apply(null,n),this._core.$stage.parent().height(o).addClass(this._core.settings.autoHeightClass)},n.prototype.destroy=function(){var t,e;for(t in this._handlers)this._core.$element.off(t,this._handlers[t]);for(e in Object.getOwnPropertyNames(this))"function"!=typeof this[e]&&(this[e]=null)},t.fn.owlCarousel.Constructor.Plugins.AutoHeight=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){var n=function(e){this._core=e,this._videos={},this._playing=null,this._handlers={"initialized.owl.carousel":t.proxy(function(t){t.namespace&&this._core.register({type:"state",name:"playing",tags:["interacting"]})},this),"resize.owl.carousel":t.proxy(function(t){t.namespace&&this._core.settings.video&&this.isInFullScreen()&&t.preventDefault()},this),"refreshed.owl.carousel":t.proxy(function(t){t.namespace&&this._core.is("resizing")&&this._core.$stage.find(".cloned .owl-video-frame").remove()},this),"changed.owl.carousel":t.proxy(function(t){t.namespace&&"position"===t.property.name&&this._playing&&this.stop()},this),"prepared.owl.carousel":t.proxy(function(e){if(e.namespace){var i=t(e.content).find(".owl-video");i.length&&(i.css("display","none"),this.fetch(i,t(e.content)))}},this)},this._core.options=t.extend({},n.Defaults,this._core.options),this._core.$element.on(this._handlers),this._core.$element.on("click.owl.video",".owl-video-play-icon",t.proxy(function(t){this.play(t)},this))};n.Defaults={video:!1,videoHeight:!1,videoWidth:!1},n.prototype.fetch=function(t,e){var i=function(){return t.attr("data-vimeo-id")?"vimeo":t.attr("data-vzaar-id")?"vzaar":"youtube"}(),s=t.attr("data-vimeo-id")||t.attr("data-youtube-id")||t.attr("data-vzaar-id"),n=t.attr("data-width")||this._core.settings.videoWidth,o=t.attr("data-height")||this._core.settings.videoHeight,r=t.attr("href");if(!r)throw new Error("Missing video URL.");if(s=r.match(/(http:|https:|)\/\/(player.|www.|app.)?(vimeo\.com|youtu(be\.com|\.be|be\.googleapis\.com)|vzaar\.com)\/(video\/|videos\/|embed\/|channels\/.+\/|groups\/.+\/|watch\?v=|v\/)?([A-Za-z0-9._%-]*)(\&\S+)?/),s[3].indexOf("youtu")>-1)i="youtube";else if(s[3].indexOf("vimeo")>-1)i="vimeo";else{if(!(s[3].indexOf("vzaar")>-1))throw new Error("Video URL not supported.");i="vzaar"}s=s[6],this._videos[r]={type:i,id:s,width:n,height:o},e.attr("data-video",r),this.thumbnail(t,this._videos[r])},n.prototype.thumbnail=function(e,i){var s,n,o,r=i.width&&i.height?'style="width:'+i.width+"px;height:"+i.height+'px;"':"",a=e.find("img"),h="src",l="",c=this._core.settings,p=function(t){n='<div class="owl-video-play-icon"></div>',s=c.lazyLoad?'<div class="owl-video-tn '+l+'" '+h+'="'+t+'"></div>':'<div class="owl-video-tn" style="opacity:1;background-image:url('+t+')"></div>',e.after(s),e.after(n)};return e.wrap('<div class="owl-video-wrapper"'+r+"></div>"),this._core.settings.lazyLoad&&(h="data-src",l="owl-lazy"),a.length?(p(a.attr(h)),a.remove(),!1):void("youtube"===i.type?(o="//img.youtube.com/vi/"+i.id+"/hqdefault.jpg",p(o)):"vimeo"===i.type?t.ajax({type:"GET",url:"//vimeo.com/api/v2/video/"+i.id+".json",jsonp:"callback",dataType:"jsonp",success:function(t){o=t[0].thumbnail_large,p(o)}}):"vzaar"===i.type&&t.ajax({type:"GET",url:"//vzaar.com/api/videos/"+i.id+".json",jsonp:"callback",dataType:"jsonp",success:function(t){o=t.framegrab_url,p(o)}}))},n.prototype.stop=function(){this._core.trigger("stop",null,"video"),this._playing.find(".owl-video-frame").remove(),this._playing.removeClass("owl-video-playing"),this._playing=null,this._core.leave("playing"),this._core.trigger("stopped",null,"video")},n.prototype.play=function(e){var i,s=t(e.target),n=s.closest("."+this._core.settings.itemClass),o=this._videos[n.attr("data-video")],r=o.width||"100%",a=o.height||this._core.$stage.height();this._playing||(this._core.enter("playing"),this._core.trigger("play",null,"video"),n=this._core.items(this._core.relative(n.index())),this._core.reset(n.index()),"youtube"===o.type?i='<iframe width="'+r+'" height="'+a+'" src="//www.youtube.com/embed/'+o.id+"?autoplay=1&rel=0&v="+o.id+'" frameborder="0" allowfullscreen></iframe>':"vimeo"===o.type?i='<iframe src="//player.vimeo.com/video/'+o.id+'?autoplay=1" width="'+r+'" height="'+a+'" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>':"vzaar"===o.type&&(i='<iframe frameborder="0"height="'+a+'"width="'+r+'" allowfullscreen mozallowfullscreen webkitAllowFullScreen src="//view.vzaar.com/'+o.id+'/player?autoplay=true"></iframe>'),t('<div class="owl-video-frame">'+i+"</div>").insertAfter(n.find(".owl-video")),this._playing=n.addClass("owl-video-playing"))},n.prototype.isInFullScreen=function(){var e=i.fullscreenElement||i.mozFullScreenElement||i.webkitFullscreenElement;return e&&t(e).parent().hasClass("owl-video-frame")},n.prototype.destroy=function(){var t,e;this._core.$element.off("click.owl.video");for(t in this._handlers)this._core.$element.off(t,this._handlers[t]);for(e in Object.getOwnPropertyNames(this))"function"!=typeof this[e]&&(this[e]=null)},t.fn.owlCarousel.Constructor.Plugins.Video=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){var n=function(e){this.core=e,this.core.options=t.extend({},n.Defaults,this.core.options),this.swapping=!0,this.previous=s,this.next=s,this.handlers={"change.owl.carousel":t.proxy(function(t){t.namespace&&"position"==t.property.name&&(this.previous=this.core.current(),this.next=t.property.value)},this),"drag.owl.carousel dragged.owl.carousel translated.owl.carousel":t.proxy(function(t){t.namespace&&(this.swapping="translated"==t.type)},this),"translate.owl.carousel":t.proxy(function(t){t.namespace&&this.swapping&&(this.core.options.animateOut||this.core.options.animateIn)&&this.swap()},this)},this.core.$element.on(this.handlers)};n.Defaults={animateOut:!1,animateIn:!1},n.prototype.swap=function(){if(1===this.core.settings.items&&t.support.animation&&t.support.transition){this.core.speed(0);var e,i=t.proxy(this.clear,this),s=this.core.$stage.children().eq(this.previous),n=this.core.$stage.children().eq(this.next),o=this.core.settings.animateIn,r=this.core.settings.animateOut;this.core.current()!==this.previous&&(r&&(e=this.core.coordinates(this.previous)-this.core.coordinates(this.next),s.one(t.support.animation.end,i).css({left:e+"px"}).addClass("animated owl-animated-out").addClass(r)),o&&n.one(t.support.animation.end,i).addClass("animated owl-animated-in").addClass(o))}},n.prototype.clear=function(e){t(e.target).css({left:""}).removeClass("animated owl-animated-out owl-animated-in").removeClass(this.core.settings.animateIn).removeClass(this.core.settings.animateOut),this.core.onTransitionEnd()},n.prototype.destroy=function(){var t,e;for(t in this.handlers)this.core.$element.off(t,this.handlers[t]);for(e in Object.getOwnPropertyNames(this))"function"!=typeof this[e]&&(this[e]=null);
},t.fn.owlCarousel.Constructor.Plugins.Animate=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){var n=function(e){this._core=e,this._timeout=null,this._paused=!1,this._handlers={"changed.owl.carousel":t.proxy(function(t){t.namespace&&"settings"===t.property.name?this._core.settings.autoplay?this.play():this.stop():t.namespace&&"position"===t.property.name&&this._core.settings.autoplay&&this._setAutoPlayInterval()},this),"initialized.owl.carousel":t.proxy(function(t){t.namespace&&this._core.settings.autoplay&&this.play()},this),"play.owl.autoplay":t.proxy(function(t,e,i){t.namespace&&this.play(e,i)},this),"stop.owl.autoplay":t.proxy(function(t){t.namespace&&this.stop()},this),"mouseover.owl.autoplay":t.proxy(function(){this._core.settings.autoplayHoverPause&&this._core.is("rotating")&&this.pause()},this),"mouseleave.owl.autoplay":t.proxy(function(){this._core.settings.autoplayHoverPause&&this._core.is("rotating")&&this.play()},this),"touchstart.owl.core":t.proxy(function(){this._core.settings.autoplayHoverPause&&this._core.is("rotating")&&this.pause()},this),"touchend.owl.core":t.proxy(function(){this._core.settings.autoplayHoverPause&&this.play()},this)},this._core.$element.on(this._handlers),this._core.options=t.extend({},n.Defaults,this._core.options)};n.Defaults={autoplay:!1,autoplayTimeout:5e3,autoplayHoverPause:!1,autoplaySpeed:!1},n.prototype.play=function(t,e){this._paused=!1,this._core.is("rotating")||(this._core.enter("rotating"),this._setAutoPlayInterval())},n.prototype._getNextTimeout=function(s,n){return this._timeout&&e.clearTimeout(this._timeout),e.setTimeout(t.proxy(function(){this._paused||this._core.is("busy")||this._core.is("interacting")||i.hidden||this._core.next(n||this._core.settings.autoplaySpeed)},this),s||this._core.settings.autoplayTimeout)},n.prototype._setAutoPlayInterval=function(){this._timeout=this._getNextTimeout()},n.prototype.stop=function(){this._core.is("rotating")&&(e.clearTimeout(this._timeout),this._core.leave("rotating"))},n.prototype.pause=function(){this._core.is("rotating")&&(this._paused=!0)},n.prototype.destroy=function(){var t,e;this.stop();for(t in this._handlers)this._core.$element.off(t,this._handlers[t]);for(e in Object.getOwnPropertyNames(this))"function"!=typeof this[e]&&(this[e]=null)},t.fn.owlCarousel.Constructor.Plugins.autoplay=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){"use strict";var n=function(e){this._core=e,this._initialized=!1,this._pages=[],this._controls={},this._templates=[],this.$element=this._core.$element,this._overrides={next:this._core.next,prev:this._core.prev,to:this._core.to},this._handlers={"prepared.owl.carousel":t.proxy(function(e){e.namespace&&this._core.settings.dotsData&&this._templates.push('<div class="'+this._core.settings.dotClass+'">'+t(e.content).find("[data-dot]").addBack("[data-dot]").attr("data-dot")+"</div>")},this),"added.owl.carousel":t.proxy(function(t){t.namespace&&this._core.settings.dotsData&&this._templates.splice(t.position,0,this._templates.pop())},this),"remove.owl.carousel":t.proxy(function(t){t.namespace&&this._core.settings.dotsData&&this._templates.splice(t.position,1)},this),"changed.owl.carousel":t.proxy(function(t){t.namespace&&"position"==t.property.name&&this.draw()},this),"initialized.owl.carousel":t.proxy(function(t){t.namespace&&!this._initialized&&(this._core.trigger("initialize",null,"navigation"),this.initialize(),this.update(),this.draw(),this._initialized=!0,this._core.trigger("initialized",null,"navigation"))},this),"refreshed.owl.carousel":t.proxy(function(t){t.namespace&&this._initialized&&(this._core.trigger("refresh",null,"navigation"),this.update(),this.draw(),this._core.trigger("refreshed",null,"navigation"))},this)},this._core.options=t.extend({},n.Defaults,this._core.options),this.$element.on(this._handlers)};n.Defaults={nav:!1,navText:["prev","next"],navSpeed:!1,navElement:"div",navContainer:!1,navContainerClass:"owl-nav",navClass:["owl-prev","owl-next"],slideBy:1,dotClass:"owl-dot",dotsClass:"owl-dots",dots:!0,dotsEach:!1,dotsData:!1,dotsSpeed:!1,dotsContainer:!1},n.prototype.initialize=function(){var e,i=this._core.settings;this._controls.$relative=(i.navContainer?t(i.navContainer):t("<div>").addClass(i.navContainerClass).appendTo(this.$element)).addClass("disabled"),this._controls.$previous=t("<"+i.navElement+">").addClass(i.navClass[0]).html(i.navText[0]).prependTo(this._controls.$relative).on("click",t.proxy(function(t){this.prev(i.navSpeed)},this)),this._controls.$next=t("<"+i.navElement+">").addClass(i.navClass[1]).html(i.navText[1]).appendTo(this._controls.$relative).on("click",t.proxy(function(t){this.next(i.navSpeed)},this)),i.dotsData||(this._templates=[t("<div>").addClass(i.dotClass).append(t("<span>")).prop("outerHTML")]),this._controls.$absolute=(i.dotsContainer?t(i.dotsContainer):t("<div>").addClass(i.dotsClass).appendTo(this.$element)).addClass("disabled"),this._controls.$absolute.on("click","div",t.proxy(function(e){var s=t(e.target).parent().is(this._controls.$absolute)?t(e.target).index():t(e.target).parent().index();e.preventDefault(),this.to(s,i.dotsSpeed)},this));for(e in this._overrides)this._core[e]=t.proxy(this[e],this)},n.prototype.destroy=function(){var t,e,i,s;for(t in this._handlers)this.$element.off(t,this._handlers[t]);for(e in this._controls)this._controls[e].remove();for(s in this.overides)this._core[s]=this._overrides[s];for(i in Object.getOwnPropertyNames(this))"function"!=typeof this[i]&&(this[i]=null)},n.prototype.update=function(){var t,e,i,s=this._core.clones().length/2,n=s+this._core.items().length,o=this._core.maximum(!0),r=this._core.settings,a=r.center||r.autoWidth||r.dotsData?1:r.dotsEach||r.items;if("page"!==r.slideBy&&(r.slideBy=Math.min(r.slideBy,r.items)),r.dots||"page"==r.slideBy)for(this._pages=[],t=s,e=0,i=0;n>t;t++){if(e>=a||0===e){if(this._pages.push({start:Math.min(o,t-s),end:t-s+a-1}),Math.min(o,t-s)===o)break;e=0,++i}e+=this._core.mergers(this._core.relative(t))}},n.prototype.draw=function(){var e,i=this._core.settings,s=this._core.items().length<=i.items,n=this._core.relative(this._core.current()),o=i.loop||i.rewind;this._controls.$relative.toggleClass("disabled",!i.nav||s),i.nav&&(this._controls.$previous.toggleClass("disabled",!o&&n<=this._core.minimum(!0)),this._controls.$next.toggleClass("disabled",!o&&n>=this._core.maximum(!0))),this._controls.$absolute.toggleClass("disabled",!i.dots||s),i.dots&&(e=this._pages.length-this._controls.$absolute.children().length,i.dotsData&&0!==e?this._controls.$absolute.html(this._templates.join("")):e>0?this._controls.$absolute.append(new Array(e+1).join(this._templates[0])):0>e&&this._controls.$absolute.children().slice(e).remove(),this._controls.$absolute.find(".active").removeClass("active"),this._controls.$absolute.children().eq(t.inArray(this.current(),this._pages)).addClass("active"))},n.prototype.onTrigger=function(e){var i=this._core.settings;e.page={index:t.inArray(this.current(),this._pages),count:this._pages.length,size:i&&(i.center||i.autoWidth||i.dotsData?1:i.dotsEach||i.items)}},n.prototype.current=function(){var e=this._core.relative(this._core.current());return t.grep(this._pages,t.proxy(function(t,i){return t.start<=e&&t.end>=e},this)).pop()},n.prototype.getPosition=function(e){var i,s,n=this._core.settings;return"page"==n.slideBy?(i=t.inArray(this.current(),this._pages),s=this._pages.length,e?++i:--i,i=this._pages[(i%s+s)%s].start):(i=this._core.relative(this._core.current()),s=this._core.items().length,e?i+=n.slideBy:i-=n.slideBy),i},n.prototype.next=function(e){t.proxy(this._overrides.to,this._core)(this.getPosition(!0),e)},n.prototype.prev=function(e){t.proxy(this._overrides.to,this._core)(this.getPosition(!1),e)},n.prototype.to=function(e,i,s){var n;!s&&this._pages.length?(n=this._pages.length,t.proxy(this._overrides.to,this._core)(this._pages[(e%n+n)%n].start,i)):t.proxy(this._overrides.to,this._core)(e,i)},t.fn.owlCarousel.Constructor.Plugins.Navigation=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){"use strict";var n=function(i){this._core=i,this._hashes={},this.$element=this._core.$element,this._handlers={"initialized.owl.carousel":t.proxy(function(i){i.namespace&&"URLHash"===this._core.settings.startPosition&&t(e).trigger("hashchange.owl.navigation")},this),"prepared.owl.carousel":t.proxy(function(e){if(e.namespace){var i=t(e.content).find("[data-hash]").addBack("[data-hash]").attr("data-hash");if(!i)return;this._hashes[i]=e.content}},this),"changed.owl.carousel":t.proxy(function(i){if(i.namespace&&"position"===i.property.name){var s=this._core.items(this._core.relative(this._core.current())),n=t.map(this._hashes,function(t,e){return t===s?e:null}).join();if(!n||e.location.hash.slice(1)===n)return;e.location.hash=n}},this)},this._core.options=t.extend({},n.Defaults,this._core.options),this.$element.on(this._handlers),t(e).on("hashchange.owl.navigation",t.proxy(function(t){var i=e.location.hash.substring(1),n=this._core.$stage.children(),o=this._hashes[i]&&n.index(this._hashes[i]);o!==s&&o!==this._core.current()&&this._core.to(this._core.relative(o),!1,!0)},this))};n.Defaults={URLhashListener:!1},n.prototype.destroy=function(){var i,s;t(e).off("hashchange.owl.navigation");for(i in this._handlers)this._core.$element.off(i,this._handlers[i]);for(s in Object.getOwnPropertyNames(this))"function"!=typeof this[s]&&(this[s]=null)},t.fn.owlCarousel.Constructor.Plugins.Hash=n}(window.Zepto||window.jQuery,window,document),function(t,e,i,s){function n(e,i){var n=!1,o=e.charAt(0).toUpperCase()+e.slice(1);return t.each((e+" "+a.join(o+" ")+o).split(" "),function(t,e){return r[e]!==s?(n=i?e:!0,!1):void 0}),n}function o(t){return n(t,!0)}var r=t("<support>").get(0).style,a="Webkit Moz O ms".split(" "),h={transition:{end:{WebkitTransition:"webkitTransitionEnd",MozTransition:"transitionend",OTransition:"oTransitionEnd",transition:"transitionend"}},animation:{end:{WebkitAnimation:"webkitAnimationEnd",MozAnimation:"animationend",OAnimation:"oAnimationEnd",animation:"animationend"}}},l={csstransforms:function(){return!!n("transform")},csstransforms3d:function(){return!!n("perspective")},csstransitions:function(){return!!n("transition")},cssanimations:function(){return!!n("animation")}};l.csstransitions()&&(t.support.transition=new String(o("transition")),t.support.transition.end=h.transition.end[t.support.transition]),l.cssanimations()&&(t.support.animation=new String(o("animation")),t.support.animation.end=h.animation.end[t.support.animation]),l.csstransforms()&&(t.support.transform=new String(o("transform")),t.support.transform3d=l.csstransforms3d())}(window.Zepto||window.jQuery,window,document);
/*!
    SlickNav Responsive Mobile Menu
    (c) 2014 Josh Cope
    licensed under MIT
*/
;(function(e,t,n){function o(t,n){this.element=t;this.settings=e.extend({},r,n);this._defaults=r;this._name=i;this.init()}var r={label:"MENU",duplicate:true,duration:200,easingOpen:"swing",easingClose:"swing",closedSymbol:"&#9658;",openedSymbol:"&#9660;",prependTo:"body",parentTag:"a",closeOnClick:false,allowParentLinks:false,nestedParentLinks:true,showChildren:false,init:function(){},open:function(){},close:function(){}},i="slicknav",s="slicknav";o.prototype.init=function(){var n=this;var r=e(this.element);var i=this.settings;if(i.duplicate){n.mobileNav=r.clone();n.mobileNav.removeAttr("id");n.mobileNav.find("*").each(function(t,n){e(n).removeAttr("id")})}else n.mobileNav=r;var o=s+"_icon";if(i.label===""){o+=" "+s+"_no-text"}if(i.parentTag=="a"){i.parentTag='a href="#"'}n.mobileNav.attr("class",s+"_nav");var u=e('<div class="'+s+'_menu"></div>');n.btn=e("<"+i.parentTag+' aria-haspopup="true" tabindex="0" class="'+s+"_btn "+s+'_collapsed"><span class="'+s+'_menutxt">'+i.label+'</span><span class="'+o+'"><span class="'+s+'_icon-bar"></span><span class="'+s+'_icon-bar"></span><span class="'+s+'_icon-bar"></span></span></a>');e(u).append(n.btn);e(i.prependTo).prepend(u);u.append(n.mobileNav);var a=n.mobileNav.find("li");e(a).each(function(){var t=e(this);var r={};r.children=t.children("ul").attr("role","menu");t.data("menu",r);if(r.children.length>0){var o=t.contents();var u=false;var a=[];e(o).each(function(){if(!e(this).is("ul")){a.push(this)}else{return false}if(e(this).is("a")){u=true}});var f=e("<"+i.parentTag+' role="menuitem" aria-haspopup="true" tabindex="-1" class="'+s+'_item"/>');if(!i.allowParentLinks||i.nestedParentLinks||!u){var l=e(a).wrapAll(f).parent();l.addClass(s+"_row")}else e(a).wrapAll('<span class="'+s+"_parent-link "+s+'_row"/>').parent();t.addClass(s+"_collapsed");t.addClass(s+"_parent");var c=e('<span class="'+s+'_arrow">'+i.closedSymbol+"</span>");if(i.allowParentLinks&&!i.nestedParentLinks&&u)c=c.wrap(f).parent();e(a).last().after(c)}else if(t.children().length===0){t.addClass(s+"_txtnode")}t.children("a").attr("role","menuitem").click(function(t){if(i.closeOnClick&&!e(t.target).parent().closest("li").hasClass(s+"_parent"))e(n.btn).click()});if(i.closeOnClick&&i.allowParentLinks){t.children("a").children("a").click(function(t){e(n.btn).click()});t.find("."+s+"_parent-link a:not(."+s+"_item)").click(function(t){e(n.btn).click()})}});e(a).each(function(){var t=e(this).data("menu");if(!i.showChildren){n._visibilityToggle(t.children,null,false,null,true)}});n._visibilityToggle(n.mobileNav,null,false,"init",true);n.mobileNav.attr("role","menu");e(t).mousedown(function(){n._outlines(false)});e(t).keyup(function(){n._outlines(true)});e(n.btn).click(function(e){e.preventDefault();n._menuToggle()});n.mobileNav.on("click","."+s+"_item",function(t){t.preventDefault();n._itemClick(e(this))});e(n.btn).keydown(function(e){var t=e||event;if(t.keyCode==13){e.preventDefault();n._menuToggle()}});n.mobileNav.on("keydown","."+s+"_item",function(t){var r=t||event;if(r.keyCode==13){t.preventDefault();n._itemClick(e(t.target))}});if(i.allowParentLinks&&i.nestedParentLinks){e("."+s+"_item a").click(function(e){e.stopImmediatePropagation()})}};o.prototype._menuToggle=function(e){var t=this;var n=t.btn;var r=t.mobileNav;if(n.hasClass(s+"_collapsed")){n.removeClass(s+"_collapsed");n.addClass(s+"_open")}else{n.removeClass(s+"_open");n.addClass(s+"_collapsed")}n.addClass(s+"_animating");t._visibilityToggle(r,n.parent(),true,n)};o.prototype._itemClick=function(e){var t=this;var n=t.settings;var r=e.data("menu");if(!r){r={};r.arrow=e.children("."+s+"_arrow");r.ul=e.next("ul");r.parent=e.parent();if(r.parent.hasClass(s+"_parent-link")){r.parent=e.parent().parent();r.ul=e.parent().next("ul")}e.data("menu",r)}if(r.parent.hasClass(s+"_collapsed")){r.arrow.html(n.openedSymbol);r.parent.removeClass(s+"_collapsed");r.parent.addClass(s+"_open");r.parent.addClass(s+"_animating");t._visibilityToggle(r.ul,r.parent,true,e)}else{r.arrow.html(n.closedSymbol);r.parent.addClass(s+"_collapsed");r.parent.removeClass(s+"_open");r.parent.addClass(s+"_animating");t._visibilityToggle(r.ul,r.parent,true,e)}};o.prototype._visibilityToggle=function(t,n,r,i,o){var u=this;var a=u.settings;var f=u._getActionItems(t);var l=0;if(r)l=a.duration;if(t.hasClass(s+"_hidden")){t.removeClass(s+"_hidden");t.slideDown(l,a.easingOpen,function(){e(i).removeClass(s+"_animating");e(n).removeClass(s+"_animating");if(!o){a.open(i)}});t.attr("aria-hidden","false");f.attr("tabindex","0");u._setVisAttr(t,false)}else{t.addClass(s+"_hidden");t.slideUp(l,this.settings.easingClose,function(){t.attr("aria-hidden","true");f.attr("tabindex","-1");u._setVisAttr(t,true);t.hide();e(i).removeClass(s+"_animating");e(n).removeClass(s+"_animating");if(!o)a.close(i);else if(i=="init")a.init()})}};o.prototype._setVisAttr=function(t,n){var r=this;var i=t.children("li").children("ul").not("."+s+"_hidden");if(!n){i.each(function(){var t=e(this);t.attr("aria-hidden","false");var i=r._getActionItems(t);i.attr("tabindex","0");r._setVisAttr(t,n)})}else{i.each(function(){var t=e(this);t.attr("aria-hidden","true");var i=r._getActionItems(t);i.attr("tabindex","-1");r._setVisAttr(t,n)})}};o.prototype._getActionItems=function(e){var t=e.data("menu");if(!t){t={};var n=e.children("li");var r=n.find("a");t.links=r.add(n.find("."+s+"_item"));e.data("menu",t)}return t.links};o.prototype._outlines=function(t){if(!t){e("."+s+"_item, ."+s+"_btn").css("outline","none")}else{e("."+s+"_item, ."+s+"_btn").css("outline","")}};o.prototype.toggle=function(){var e=this;e._menuToggle()};o.prototype.open=function(){var e=this;if(e.btn.hasClass(s+"_collapsed")){e._menuToggle()}};o.prototype.close=function(){var e=this;if(e.btn.hasClass(s+"_open")){e._menuToggle()}};e.fn[i]=function(t){var n=arguments;if(t===undefined||typeof t==="object"){return this.each(function(){if(!e.data(this,"plugin_"+i)){e.data(this,"plugin_"+i,new o(this,t))}})}else if(typeof t==="string"&&t[0]!=="_"&&t!=="init"){var r;this.each(function(){var s=e.data(this,"plugin_"+i);if(s instanceof o&&typeof s[t]==="function"){r=s[t].apply(s,Array.prototype.slice.call(n,1))}});return r!==undefined?r:this}}})(jQuery,document,window)
//]]></script>


<script type='text/javascript'>//<![CDATA[
$(document).ready(function(){
	$('.owl_carouselle').owlCarousel({
      	autoplay:true,
    	loop:true,
		nav: true,
		navText: ["<i class='fa fa-chevron-left'></i>","<i class='fa fa-chevron-right'></i>"],
		smartSpeed: 900,
    	responsiveClass:true,
    	responsive:{
        	0:{
            	items:1,
            	nav:true
        	},
        	600:{
            	items:1,
            	nav:false
        	},
        	1000:{
            	items:1,
            	nav:true,
        	}
    	}
	});
	$('.blog_menus').slicknav({
		label: '',
		duration: 200,
  		prependTo: '#slick_nav'
	});
	var smooth_scroll = $('#smooth_scroll');
	//Click event to scroll to top
	smooth_scroll.click(function(){
		$('html, body').animate({scrollTop : 0},800);
		return false;
	});
});
//]]></script>


<script src='http://yourjavascript.com/26121239615/fitvids.js' type='text/javascript'/>
<b:include data='blog' name='google-analytics'/>
</body>
</html> 
0 comments on commit a8e3a0f
@mashfiquemiraz
 
 
Leave a comment

Attach files by dragging & dropping, selecting or pasting them.
 You’re not receiving notifications from this thread.
© 2020 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
Pricing
API
Training
Blog
About
