<h1>PageMe</h1>
<p>Copyright 2013 by Atec Media and Jens Eldering.</p>
<p>PageMe by <a href="http://www.atecmedia.com" rel="cc:attributionURL">Jens Eldering</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.</p>
<p>Based on a work at <a href="https://github.com/Scribilicious/jquery.pageme" rel="dct:source">https://github.com/Scribilicious/jquery.pageme</a>.</p>
<h2>Summary</h2>
<p>PageMe is a jQuery auto paging plug-in. Just scroll to the bottom to load the next page.</p>
<h2>Getting started</h2>
<p>Check the <a href="http://pageme.atecmedia.com" title="Show demo">demo</a> in this package.</p>
<p>Creating an basic instance is done as followed:</p>
<pre>
$(document).ready(function() {
    $(".content").pageme();
});
</pre>
<h2>Options</h2>
<p>PageMe can be customised by passing a set of options. The following example is the pageme instance with all the options and default settings:</p>
<pre>
$(".content").pageme({
    status     : '&lt;div class=&quot;scrollLoad&quot;&gt;&lt;/div&gt;',
    loading    : 'Loading...',
    finished   : 'Finished...',
    error      : 'Error loading...',
    statusfade : 500,
    statuspause: 1000,
    container  : '.container',
    next       : '.next',
    navigation : '.navigate',
    nextfade   : 500,
    type       : 'html'
});
</pre>
<h3>status</h3>
<p>Status contains the status container. This is the container that is being viewed while loading. This should contain only one element! If false or empty, all statuses will be ignored</p>
<h3>loading, finished, error</h3>
<p>These options contain the several statuses that pageme can contain. If needed HTML can be passed through these options. For example an animated loading image. If false no status is shown.</p>
<h3>statusfade</h3>
<p>The fading speed of the status message. If false no fading will occur.</p>
<h3>statuspause</h3>
<p>The waiting time between fading. This will only have effect on the error and finished status.</p>
<h3>container</h3>
<p>The container element that contains the actual content of the page without the navigation elements. So just the data that needs to be auto paginated.</p>
<h3>next</h3>
<p>The next page element. This element must be of the the type &lt;a&gt; and needs to contain a href link.</p>
<h3>navigation</h3>
<p>This is the navigation element that contains all the navigation elements.</p>
<h3>nextfade</h3>
<p>The fading speed of when viewing the next page. If set to false no fading will occur!</p>
<h3>type</h3>
<p>The content type of the to be loaded page. Normally this is HTML.</p>
<h2>Known issues</h2>
<p>When used from a file:// URL some access control errors can occur. Solution, run script instead in a local or online server environment.</p>