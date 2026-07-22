<h2 id="publications">Selected Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="pub-media">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser" alt="Preview for {{ link.title }}" loading="lazy">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
    {% endif %}
  </div>
  <div class="pub-content">
      <h3 class="title"><a href="{{ link.pdf }}" target="_blank" rel="noopener noreferrer">{{ link.title }}</a></h3>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn" target="_blank" rel="noopener noreferrer">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn" target="_blank" rel="noopener noreferrer">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn" target="_blank" rel="noopener noreferrer">Project page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn" target="_blank" rel="noopener noreferrer">BibTeX</a>
      {% endif %}
      {% if link.dataset %}
      <a href="{{ link.dataset }}" class="btn" target="_blank" rel="noopener noreferrer">Dataset</a>
      {% endif %}
      {% if link.notes %} 
      <span class="pub-note">{{ link.notes }}</span>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>
{% endfor %}

</ol>
</div>
