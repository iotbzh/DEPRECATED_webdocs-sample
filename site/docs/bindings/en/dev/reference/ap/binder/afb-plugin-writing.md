---
edit_link: ''
title: afb plugin writing
---

<!-- WARNING: This file is generated by fetch_docs.js using site/_tocs/bindings/fetched_files.yml -->

<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en-US" lang="en-US">
<!-- git web interface version 1.7.1, (C) 2005-2006, Kay Sievers <kay.sievers@vrfy.org>, Christian Gierke -->
<!-- git core binaries version 1.7.1 -->
<head>
<meta http-equiv="content-type" content="text/html; charset=utf-8"/>
<meta name="generator" content="gitweb/1.7.1 git/1.7.1"/>
<meta name="robots" content="index, nofollow"/>
<title>gerrit.automotivelinux Code Review - src/app-framework-binder.git/blob_plain - doc/afb-plugin-writing.md</title>
<link rel="stylesheet" type="text/css" href="gitweb-default.css"/>
<link rel="stylesheet" type="text/css" href="gitweb-site.css"/>
<link rel="alternate" title="src/app-framework-binder.git - history of doc/afb-plugin-writing.md - RSS feed" href="/gerrit/gitweb?p=src/app-framework-binder.git;a=rss;f=doc/afb-plugin-writing.md" type="application/rss+xml" />
<link rel="alternate" title="src/app-framework-binder.git - history of doc/afb-plugin-writing.md - RSS feed (no merges)" href="/gerrit/gitweb?p=src/app-framework-binder.git;a=rss;f=doc/afb-plugin-writing.md;opt=--no-merges" type="application/rss+xml" />
<link rel="alternate" title="src/app-framework-binder.git - history of doc/afb-plugin-writing.md - Atom feed" href="/gerrit/gitweb?p=src/app-framework-binder.git;a=atom;f=doc/afb-plugin-writing.md;opt=--no-merges" type="application/atom+xml" />
<link rel="alternate" title="src/app-framework-binder.git - history of doc/afb-plugin-writing.md - Atom feed (no merges)" href="/gerrit/gitweb?p=src/app-framework-binder.git;a=atom;f=doc/afb-plugin-writing.md;opt=--no-merges" type="application/atom+xml" />
<link rel="shortcut icon" href="favicon.ico" type="image/png" />
</head>
<body>
<div>
  <div style="background:url(/gerrit/static/LF_Collab_header_gray_stripe.png); width:100%; height:30px; background-repeat:repeat; overflow:hidden;"><img src="/gerrit/static/LF_Collab_header_gray.png"/>
  </div>
  <div class="header">
    <table style="width:100%; padding: 0px;">
      <tr>
        <td><a href="http://www.automotivelinux.org"><img src="/gerrit/static/logo_automotivelinux.png"/></a></td>
        <td style="vertical-align:bottom; padding:10px 0px;">
          <div class="horizontal">
            <ul>
              <li><a href="https://dev.automotivelinux.org/">Account signup</a> | </li>
              <li><a href="https://wiki.automotivelinux.org/">Wiki</a> | </li>
              <li><a href="https://jira.automotivelinux.org/">Jira</a> | </li>
              <li><a href="https://doors.automotivelinux.org/">Doors</a> | </li>
              <li><a href="https://gerrit.automotivelinux.org/">Gerrit</a> | </li>
              <li><a href="https://build.automotivelinux.org/">Jenkins</a> | </li>
              <li><a href="https://lists.linuxfoundation.org/">Mailing lists</a> | </li>
              <li><a href="https://ask.automotivelinux.org/">Forums (Askbot)</a> | </li>
              <li><a href="/gerrit/static/signoffrules.txt">Sign-off Rules</a></li>
            </ul>
          </div>
        </td>
      </tr>
    </table>
  </div>
</div>
<div class="page_header">
<a title="git homepage" href="http://git-scm.com/"><img src="gitweb-logo.png" width="72" height="27" alt="git" class="logo"/></a><a href="/gerrit/">Code Review</a> / <a href="/gerrit/gitweb?p=src/app-framework-binder.git;a=summary">src/app-framework-binder.git</a> / blob_plain
</div>
<form method="get" action="/gerrit/gitweb" enctype="application/x-www-form-urlencoded">
<div class="search">
<input name="p" type="hidden" value="src/app-framework-binder.git" />
<input name="a" type="hidden" value="search" />
<input name="h" type="hidden" value="master" />
<select name="st" >
<option selected="selected" value="commit">commit</option>
<option value="grep">grep</option>
<option value="author">author</option>
<option value="committer">committer</option>
<option value="pickaxe">pickaxe</option>
</select><sup><a href="/gerrit/gitweb?p=src/app-framework-binder.git;a=search_help">?</a></sup> search:
<input type="text" name="s"  />
<span title="Extended regular expression"><label><input type="checkbox" name="sr" value="1" />re</label></span></div>
</form>
<div class="page_body">
<br /><br />
404 - Cannot find file
<br />
</div>
<div class="page_footer">
<div class="page_footer_text">Application Framework binder daemon, maintained by iot.bzh team</div>
<a class="rss_logo" title="history of doc/afb-plugin-writing.md RSS feed" href="/gerrit/gitweb?p=src/app-framework-binder.git;a=rss;f=doc/afb-plugin-writing.md">RSS</a>
<a class="rss_logo" title="history of doc/afb-plugin-writing.md Atom feed" href="/gerrit/gitweb?p=src/app-framework-binder.git;a=atom;f=doc/afb-plugin-writing.md">Atom</a>
</div>
<div style="position:relative; overflow:hidden;">
  <div style="background:url(/gerrit/static/LF_Collab_footer_gray_stripe.png); width:100%; height:80px; background-repeat:repeat;"><img src="/gerrit/static/LF_Collab_footer_gray.png"/></div>
  <p style="position:absolute; top: 4px; left: 10px; font-family:helvetica,arial; font-size:11px; color:#393939; line-height: 16px; margin-top:12px;">&#169;2015 Automotive Grade Linux, a Linux Foundation Collaborative Project. All Rights Reserved.
  Linux Foundation is a registered trademark of The Linux Foundation.<br />
  Linux is a registered trademark of Linus Torvalds.
  </p>
</div>
<script type="text/javascript" src="gitweb.js"></script>
</body>
</html>