<h2 id="underreview" style="margin: 2px 0px -15px;">Under Review</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.underreview.main %}

<li>
<div class="pub-row">
  <div class="col-sm-9" style="padding-right: 15px; padding-left: 20px; padding-bottom: -30px">
      <div class="title"><a href="{{ link.pdf }}" target="_blank" rel="noopener noreferrer">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="keyword keyword-text-color">{{ link.keyword }}</div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>
