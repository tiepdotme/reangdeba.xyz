---
layout: page
title: "Bucket list"
comments: false
permalink: /bucket/
---

### Life

<div class="container">
<div class="progress">
  <div class="progress-bar progress-bar-striped bg-danger" role="progressbar" aria-valuemin="0" aria-valuemax="100" id="lifeprogressbar"></div>
</div>
</div>

> Things I wish to do before I die.

### Progress
<div class="container">
<div class="progress">
  <div class="progress-bar progress-bar-striped bg-success" role="progressbar" aria-valuemin="0" aria-valuemax="100" id="theprogressbar"></div>
</div>
</div>

<div>
<ol>
{% for item in site.data.bucket_complete %}
<li><s>{{item}}</s></li>
{% endfor %}
</ol>
</div>

### List

<div>
<ol>
{% for item in site.data.bucket_list %}
<li>{{item}}</li>
{% endfor %}
</ol>
</div>

<blockquote><p>For suggestions please send me an <a href="mailto:hi@reangdeba.xyz">email</a>, or reach out on <a
        target="_blank" href="https://twitter.com/reangdeba">Twitter</a>.</p></blockquote>

<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
        integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
        crossorigin="anonymous"></script>

<script>
        var deno = {{ site.data.bucket_list.size }};
        var nume = {{ site.data.bucket_complete.size }};
        var newprogress = Math.round(nume/deno*100);
$('#theprogressbar').attr('aria-valuenow', newprogress).css('width', newprogress+'%');

$('#theprogressbar').text(newprogress + '%');
</script>

<script>
        var progress = Math.round(21/84*100);
$('#lifeprogressbar').attr('aria-valuenow', progress).css('width', progress+'%');

$('#lifeprogressbar').text(progress + '%');
</script>
