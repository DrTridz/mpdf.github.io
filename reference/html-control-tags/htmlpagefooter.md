---
layout: page
title: htmlpagefooter
parent_title: HTML control tags
permalink: /reference/html-control-tags/htmlpagefooter.html
modification_time: 2015-08-05T12:01:23+00:00
---

<p>(mPDF &gt;= 2.0)</p>
<p>htmlpagefooter – Define an HTML page footer with a given name</p>

# Description

<p class="manual_block">&lt;<b>htmlpagefooter</b>&nbsp; <span class="parameter">name</span>&nbsp; &gt; <span class="parameter">html</span> &lt;/htmlpagefooter&gt;</p>
<p>Define an HTML page footer with a given name. Named footer can be referenced and set later in the document e.g. &lt;<a href="{{ "/reference/html-control-tags/setpageheader.html" | prepend: site.baseurl }}">sethtmlpagefooter</a>&gt;</p>

<div class="alert alert-info" role="alert"><strong>Note:</strong> Do not name any header or footer starting with html_&nbsp;&nbsp; This prefix is reserved to identify an <span class="smallblock">HTML</span> header/footer when passing its name in a reference.</div>

<div class="alert alert-info" role="alert"><strong>Note:</strong> Remember that, unlike most mPDF custom tags which are self-closing with /&gt;, htmlpageheader and htmlpagefooter require end tags. If you wish to make the HTML code compatible with browsers, see <a href="{{ "/html-support/custom-html-tags.html" | prepend: site.baseurl }}">Custom tags</a></div>

# Attributes

<p class="manual_param_dt"><span class="parameter">name</span></p>
<p class="manual_param_dd">This attribute is a text string to use as the name for this footer.

If name is <span class="smallblock">BLANK</span> or omitted, it is set as '_default'.</p>

# Content

<p class="manual_param_dt"><span class="parameter">html</span></p>
<p class="manual_param_dd">Any valid HTML code can be enclosed between the tags, and will be parsed by mPDF as for any other content.</p>

# Changelog

<table class="table"> <thead>
<tr> <th>Version</th><th>Description</th> </tr>
</thead> <tbody>
<tr>
<td>2.0</td>
<td>The tag was added.</td>
</tr>
</tbody> </table>

# Examples

<p>For examples and further information please see:</p>
<ul>
<li class="manual_boxlist"><a href="{{ "/headers-footers/headers-footers.html" | prepend: site.baseurl }}">Headers &amp; Footers</a></li>
<li class="manual_boxlist"><a href="{{ "/headers-footers/method-4.html" | prepend: site.baseurl }}">Headers &amp; Footers - Method 4</a></li>
</ul>

# See Also

<ul>
<li class="manual_boxlist"> <a href="{{ "/reference/mpdf-functions/defhtmlfooterbyname.html" | prepend: site.baseurl }}">DefHTMLFooterByName()</a> </li>
<li class="manual_boxlist">&lt;<a href="{{ "/reference/html-control-tags/htmlpageheader.html" | prepend: site.baseurl }}">htmlpageheader</a>&gt; </li>
<li class="manual_boxlist"> <a href="{{ "/reference/mpdf-functions/sethtmlfooterbyname.html" | prepend: site.baseurl }}">SetHTMLFooterByName()</a></li>
<li class="manual_boxlist"> &lt;<a href="{{ "/reference/html-control-tags/sethtmlpagefooter.html" | prepend: site.baseurl }}">sethtmlpagefooter</a>&gt; </li>
<li class="manual_boxlist"> <a href="{{ "/paging/using-page.html" | prepend: site.baseurl }}">@page</a> </li>
</ul>