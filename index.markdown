---
layout: default
---
<div class="container">

<div class="row">
{% for post in site.posts limit:1 %}
    {% include blogPostItemFullRow.html %}
{% endfor %}
</div>

<div class="row">
{% for post in site.posts offset:1 limit:3 %}
  <div class="col-sm d-flex align-items-stretch">
    {% include blogPostItem.html %}
  </div>
{% endfor %}
</div>

<!-- <br>
<div class="row">
{% for post in site.posts offset:3 limit:6 %}
  <div class="col-sm d-flex align-items-stretch">
    {% include blogPostItem.html %}
  </div>
{% endfor %}
</div> -->

<br/>
<div class="row">
{% for post in site.posts offset:4 limit:1 %}
  <div class="col-sm d-flex align-items-stretch">
    {% include blogPostItemHalfRow.html %}
  </div>
{% endfor %}
</div>
<div class="row">
{% for post in site.posts offset:5 limit:1 %}
  <div class="col-sm d-flex align-items-stretch">
    {% include blogPostItemHalfRow.html %}
  </div>
{% endfor %}
</div>

</div>
