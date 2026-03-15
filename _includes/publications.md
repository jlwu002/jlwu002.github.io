<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">

  {% assign llm_pubs = site.data.publications.main | where: "area", "LLM / Learning from Feedback" %}
  {% assign rl_pubs = site.data.publications.main | where: "area", "Reinforcement Learning / Safe Control" %}
  {% assign csc_pubs = site.data.publications.main | where: "area", "Computational Social Choice / Game Theory" %}

  {% if llm_pubs.size > 0 %}
  <h3 style="margin-top: 10px;">LLM / Learning from Feedback</h3>
  <ol class="bibliography">
  {% for link in llm_pubs %}
    <li>
      <div class="pub-row">
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
          <div class="title"><a href="{{ link.pdf }}" target="_blank" rel="noopener noreferrer">{{ link.title }}</a></div>
          <div class="author">{{ link.authors }}</div>
          <div class="conference-text-color{% if link.conference_short == 'Preprint' %} preprint{% endif %}">
            <em>
              {% if link.conference_short == 'Preprint' %}
                Preprint (under review)
              {% else %}
                {{ link.conference }}
              {% endif %}
            </em>
          </div>
          <div class="links">
            {% if link.code %} 
            <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
            {% endif %}
            {% if link.page %} 
            <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
            {% endif %}
            {% if link.bibtex %} 
            <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
            {% endif %}
            {% if link.notes %} 
            <strong><i style="color:#c0392b">{{ link.notes }}</i></strong>
            {% endif %}
            {% if link.others %} 
            {{ link.others }}
            {% endif %}
          </div>
        </div>
      </div>
    </li>
    <br>
  {% endfor %}
  </ol>
  {% endif %}

  {% if rl_pubs.size > 0 %}
  <h3 style="margin-top: 10px;">Reinforcement Learning / Safe Control</h3>
  <ol class="bibliography">
  {% for link in rl_pubs %}
    <li>
      <div class="pub-row">
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
          <div class="title"><a href="{{ link.pdf }}" target="_blank" rel="noopener noreferrer">{{ link.title }}</a></div>
          <div class="author">{{ link.authors }}</div>
          <div class="conference-text-color{% if link.conference_short == 'Preprint' %} preprint{% endif %}">
            <em>
              {% if link.conference_short == 'Preprint' %}
                Preprint (under review)
              {% else %}
                {{ link.conference }}
              {% endif %}
            </em>
          </div>
          <div class="links">
            {% if link.code %} 
            <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
            {% endif %}
            {% if link.page %} 
            <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
            {% endif %}
            {% if link.bibtex %} 
            <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
            {% endif %}
            {% if link.notes %} 
            <strong><i style="color:#c0392b">{{ link.notes }}</i></strong>
            {% endif %}
            {% if link.others %} 
            {{ link.others }}
            {% endif %}
          </div>
        </div>
      </div>
    </li>
    <br>
  {% endfor %}
  </ol>
  {% endif %}

  {% if csc_pubs.size > 0 %}
  <h3 style="margin-top: 10px;">Computational Social Choice / Game Theory</h3>
  <ol class="bibliography">
  {% for link in csc_pubs %}
    <li>
      <div class="pub-row">
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
          <div class="title"><a href="{{ link.pdf }}" target="_blank" rel="noopener noreferrer">{{ link.title }}</a></div>
          <div class="author">{{ link.authors }}</div>
          <div class="conference-text-color{% if link.conference_short == 'Preprint' %} preprint{% endif %}">
            <em>
              {% if link.conference_short == 'Preprint' %}
                Preprint (under review)
              {% else %}
                {{ link.conference }}
              {% endif %}
            </em>
          </div>
          <div class="links">
            {% if link.code %} 
            <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
            {% endif %}
            {% if link.page %} 
            <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
            {% endif %}
            {% if link.bibtex %} 
            <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
            {% endif %}
            {% if link.notes %} 
            <strong><i style="color:#c0392b">{{ link.notes }}</i></strong>
            {% endif %}
            {% if link.others %} 
            {{ link.others }}
            {% endif %}
          </div>
        </div>
      </div>
    </li>
    <br>
  {% endfor %}
  </ol>
  {% endif %}

</div>
