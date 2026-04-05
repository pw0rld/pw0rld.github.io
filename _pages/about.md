---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="home-page">

<span id="about-me" class="home-anchor"></span>

<p>I work on <strong>trusted execution environments (TEE)</strong>, <strong>confidential computing</strong>, and <strong>Web3 systems</strong> at <a href="https://x.com/teenet_io">Teenet</a>. Previously, I was a Research Assistant at <a href="https://teecertlabs.com/">Teecertlab</a> at Southern University of Science and Technology (SUSTech). I received my B.Eng. in <strong>Cybersecurity</strong> from <strong>Xi'an University of Posts and Telecommunications (XUPT)</strong> in July 2021.</p>

<p>My recent work focuses on state continuity for confidential computing, blockchain-assisted system design, and hardware memory-encryption analysis. This homepage collects my recent publications, background, and updates.</p>

<span id="news" class="home-anchor"></span>
<h1>🔥 News</h1>
<ul>
  <li><em>2025.08</em>: Our paper <a href="https://www.usenix.org/conference/usenixsecurity25/presentation/peng-wei">Shadows in Cipher Spaces: Exploiting Tweak Repetition in Hardware Memory Encryption</a> appeared at <strong>USENIX Security '25</strong>.</li>
  <li><em>2024.03</em>: Published <strong>Ensuring State Continuity for Confidential Computing: A Blockchain-based Approach</strong> in <strong>IEEE TDSC</strong>.</li>
  <li><em>2022.11</em>: Published <strong>Narrator: Secure and Practical State Continuity for Trusted Execution in the Cloud</strong> at <strong>ACM CCS 2022</strong>.</li>
</ul>

<span id="publications" class="home-anchor"></span>
<h1>📝 Publications</h1>

{% assign publications = site.publications | sort: "date" | reverse %}
<div class="home-pubs">
  {% for post in publications %}
    <article class="home-pub">
      <h2 class="home-pub__title"><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h2>
      {% if post.authors %}<p class="home-pub__authors">{{ post.authors }}</p>{% endif %}
      {% if post.venue %}<p class="home-pub__meta"><em>{{ post.venue }}</em></p>{% endif %}
      {% if post.excerpt %}<p class="home-pub__excerpt">{{ post.excerpt }}</p>{% endif %}
      <div class="home-pub__links">
        {% if post.paperurl %}<a class="home-pill" href="{{ post.paperurl }}">Paper</a>{% endif %}
        {% if post.projecturl %}<a class="home-pill home-pill--ghost" href="{{ post.projecturl }}">Project</a>{% endif %}
        {% if post.codeurl %}<a class="home-pill home-pill--ghost" href="{{ post.codeurl }}">Code</a>{% endif %}
        {% if post.artifacturl %}<a class="home-pill home-pill--ghost" href="{{ post.artifacturl }}">Artifact</a>{% endif %}
        <a class="home-pill home-pill--ghost" href="{{ base_path }}{{ post.url }}">Details</a>
      </div>
    </article>
  {% endfor %}
</div>

<span id="honors-and-awards" class="home-anchor"></span>
<h1>🎖 Honors and Awards</h1>
<ul>
  <li><em>2023.11</em>: First place, <strong>IDASH PRIVACY &amp; SECURITY WORKSHOP 2023</strong>, <a href="http://www.humangenomeprivacy.org/2023/index.html">Track 3</a>.</li>
</ul>

<span id="education" class="home-anchor"></span>
<h1>📖 Education</h1>
<ul>
  <li><em>2021</em>: B.Eng. in <strong>Cybersecurity</strong>, Xi'an University of Posts and Telecommunications (XUPT), Xi'an, China.</li>
</ul>

<span id="experience" class="home-anchor"></span>
<h1>💻 Experience</h1>
<ul>
  <li><em>Current</em>: <strong>Teenet</strong>. Working on <strong>TEE + Web3</strong> infrastructure and secure systems.</li>
  <li><em>Previous</em>: <strong>Research Assistant</strong>, <strong>Teecertlab</strong>, Southern University of Science and Technology (SUSTech). Worked on confidential computing and security analysis under the supervision of <a href="https://yinqian.org/">Yinqian Zhang</a>.</li>
</ul>

</div>
