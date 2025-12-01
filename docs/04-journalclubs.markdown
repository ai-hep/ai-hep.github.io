---
layout: page
title: Journal Clubs
permalink: /journalclubs/
order: 5
---

<!--
<div class="hero-section" style="padding: 2rem 0; margin-bottom: 2rem;">
  <div class="wrapper">
    <h1 class="hero-title" style="font-size: 2.5rem;">Journal Clubs</h1>
    <p class="hero-subtitle">Exploring the Latest in AI + High Energy Physics</p>
  </div>
</div>
-->

<div class="wrapper">
  <div class="content-section">
    <p style="font-size: 1.1rem; line-height: 1.6; margin-bottom: 2rem;">
      Our journal clubs bring together researchers to discuss various developments 
      at the intersection of artificial intelligence and high energy physics. Join us for in-depth 
      discussions on both theoretical foundations and practical applications.
    </p>

    <div class="highlight-box">
      <h3>📅 Meeting Details</h3>
      <ul>
        <li><strong>Frequency:</strong> Bi-weekly sessions</li>
        <li><strong>Format:</strong> Virtual </li>
        <li><strong>Duration:</strong> 60 minutes with Q&A</li>
        <li><strong>Language:</strong> English</li>
        <li><strong>Time:</strong> Monday 3 PM Beijing, 4 PM JST/KST</li>
      </ul>
    </div>

    <!-- <h2 class="section-title">Upcoming Sessions</h2>
    
    {% assign upcoming_sessions = site.data.journal_clubs.upcoming | default: empty %}
    {% if upcoming_sessions.size > 0 %}
      {% for session in upcoming_sessions %}
      <div class="card journal-club-upcoming" style="margin-bottom: 2rem;">
        <div class="journal-club-date">{{ session.date }}</div>
        <h3 class="card-title">{{ session.topic }}</h3>
        
        <div style="margin: 1rem 0;">
          <p><strong>Time:</strong> {{ session.time }}</p>
          <p><strong>Format:</strong> {{ session.format }}</p>
          <p><strong>Discussion Lead:</strong> {{ session.presenter }}</p>
        </div>
        
        {% if session.papers %}
        <div style="margin: 1rem 0;">
          <h4 style="color: var(--accent-color); margin-bottom: 0.5rem;">Featured Papers:</h4>
          {% for paper in session.papers %}
          <div class="paper-link">
            <a href="{{ paper.url }}" target="_blank">{{ paper.title }}</a>
            <div style="font-size: 0.9rem; color: var(--text-muted);">{{ paper.journal }}</div>
          </div>
          {% endfor %}
        </div>
        {% endif %}
        
        <p style="margin-top: 1rem;">{{ session.description }}</p>
      </div>
      {% endfor %}
    {% else %}
      <div class="card">
        <h3 class="card-title">📅 July 14, 2025</h3>
        <p><strong>Time:</strong> 3-4 PM Beijing Time</p>
        <div class="news-section" style="margin: 1rem 0;">
          <p><strong>Topic:</strong> To be announced</p>
          <p><strong>Focused Paper:</strong> Coming soon</p>
        </div>
      </div>
    {% endif %} -->

    <h2 class="section-title">Past Sessions</h2>

    <!--
    <div class="journal-filter-bar" id="journal-filter-bar">
      <div class="journal-filter-controls">
        <label>
          Before date
          <input type="date" id="session-before-date" aria-label="Filter sessions before date" />
        </label>
        <label>
          Search
          <input type="search" id="session-keyword" placeholder="Topic, paper, arXiv..." aria-label="Keyword search" />
        </label>
        <button class="btn btn-outline" id="session-reset" type="button">Reset</button>
      </div>
      <div class="journal-filter-status" id="journal-filter-status" aria-live="polite"></div>
    </div>
    -->

    {% assign past_sessions = site.data.journal_clubs.past | default: empty %}
    {% assign sorted_past = past_sessions | sort: "date" | reverse %}
    {% if sorted_past.size > 0 %}
      <div id="past-sessions" class="journal-list" style="max-height: none;">
      {% for session in sorted_past %}
        <article class="journal-session-item" data-date="{{ session.date }}">
          <aside class="jsi-meta">
            <span class="journal-session-date">{{ session.date }}</span>
            <!-- <span class="journal-session-time">{{ session.time }}</span> -->
          </aside>
          <div class="jsi-body">
            <h3 class="journal-session-title">{{ session.topic }}</h3>
            {% if session.focused_paper and session.focused_paper.title %}
              <div class="journal-focused-paper minimal">
                <span class="jf-label">Focused</span>
                <span class="jf-title">
                        {% if session.focused_paper.url %}
                        <a href="{{ session.focused_paper.url }}" target="_blank">{{ session.focused_paper.title }}</a>
                        {% else %}
                        {{ session.focused_paper.title }}
                        {% endif %}
                        {% if session.focused_paper.arxiv %} (arXiv:{{ session.focused_paper.arxiv }}){% endif %}
                </span>
              </div>
            {% endif %}
            {% if session.description %}
            <p class="journal-session-description">{{ session.description }}</p>
            {% endif %}
            {% if session.related_papers and session.related_papers.size > 0 %}
            <details class="journal-related-papers" open>
              <summary>Related Papers ({{ session.related_papers.size }})</summary>
              <ul>
                {% for paper in session.related_papers %}
                <li>
                  {% if paper.url %}<a href="{{ paper.url }}" target="_blank">{{ paper.title }}</a>{% else %}{{ paper.title }}{% endif %}
                  {% if paper.arxiv %}<span class="journal-arxiv">(arXiv:{{ paper.arxiv }})</span>{% endif %}
                </li>
                {% endfor %}
              </ul>
            </details>
            {% endif %}
          </div>
        </article>
      {% endfor %}
      </div>
    {% else %}
      <p>No past sessions recorded yet.</p>
    {% endif %}

    <!-- TODO: Maybe expand or shorten this later. It looks like a wall of text right now! -->
    <!--
      <div class="content-section">
      <br>
        <h2 class="section-title">Discussion Topics</h2>
        <p style="margin-bottom: 2rem;">Our journal club sessions explore cutting-edge research at the intersection of AI and high energy physics, covering both foundational advances and cross-disciplinary applications:</p>
            
            <div class="card-grid">
              <div class="card">
              <h3 class="card-title"> Neural Architecture Design</h3>
              <p>Novel network architectures for particle physics, attention mechanisms in detector simulation, and physics-informed neural networks for field theory calculations.</p>
              </div>
              
              <div class="card">
              <h3 class="card-title"> Mechanistic Interpretability</h3>
              <p>Understanding how neural networks learn physical laws, interpretable models for particle classification, and discovering computational structures in physics-based AI systems.</p>
              </div>
              
              <div class="card">
              <h3 class="card-title"> Physics-Inspired AI</h3>
              <p>Thermodynamic approaches to machine learning, statistical mechanics in neural training, and energy-based models for generative particle physics.</p>
              </div>
              
              <div class="card">
              <h3 class="card-title"> Machine Learning in HEP</h3>
              <p>Transformer architectures for event reconstruction, graph neural networks for particle tracking, and deep learning approaches to Higgs boson analysis.</p>
              </div>
              
              <div class="card">
              <h3 class="card-title"> Symbolic & Generative Models</h3>
              <p>Symbolic regression for discovering physical laws, variational autoencoders for detector simulation, and diffusion models for particle generation.</p>
              </div>
              
              <div class="card">
              <h3 class="card-title"> Foundation Models</h3>
              <p>Large language models for scientific literature analysis, multimodal transformers for experimental data, and pre-trained models for cross-experiment transfer learning.</p>
              </div>
              
              <div class="card">
              <h3 class="card-title"> Optimization & Training</h3>
              <p>Double descent in overparameterized physics models, federated learning across experimental collaborations, and efficient training strategies for large-scale simulations.</p>
              </div>
              
              <div class="card">
              <h3 class="card-title"> Cross-Disciplinary Applications</h3>
              <p>AI techniques adapted for lattice QCD, physics principles applied to improve neural network training, and quantum machine learning for particle physics.</p>
              </div>
            </div>
     -->
<script>
  (function(){
    const beforeInput = document.getElementById('session-before-date');
    const keywordInput = document.getElementById('session-keyword');
    const resetBtn = document.getElementById('session-reset');
    const statusEl = document.getElementById('journal-filter-status');
    const container = document.getElementById('past-sessions');
    if(!container) return;
    const cards = Array.from(container.querySelectorAll('.journal-session-item'));

    cards.forEach(card => {
      const ds = card.getAttribute('data-date');
      card._date = new Date(ds + 'T00:00:00Z');
      let text = card.querySelector('.journal-session-title')?.textContent || '';
      const focused = card.querySelector('.journal-focused-paper');
      if(focused) text += ' ' + focused.textContent;
      const related = card.querySelectorAll('.journal-related-papers li');
      related.forEach(li => { text += ' ' + li.textContent; });
      card._search = text.toLowerCase();
    });

    function debounce(fn, wait=180){
      let t; return function(...args){ clearTimeout(t); t=setTimeout(()=>fn.apply(this,args), wait); };
    }

    function formatDate(d){
      if(!(d instanceof Date) || isNaN(d)) return ''; const iso = d.toISOString().slice(0,10); return iso;
    }

    function applyFilters(){
      const beforeVal = beforeInput.value ? new Date(beforeInput.value + 'T00:00:00Z') : null;
      const kwRaw = keywordInput.value.trim().toLowerCase();
      const kwTokens = kwRaw.length ? kwRaw.split(/\s+/).filter(Boolean) : [];

      const filtered = cards.filter(c => {
        if(beforeVal && c._date >= beforeVal) return false;
        if(kwTokens.length){
          for(const token of kwTokens){
            if(!c._search.includes(token)) return false;
          }
        }
        return true;
      });

      cards.forEach(c => c.classList.add('is-filter-hidden'));
      filtered.forEach(c => c.classList.remove('is-filter-hidden'));

      let emptyState = container.querySelector('.journal-empty-state');
      if(!filtered.length){
        if(!emptyState){
          emptyState = document.createElement('div');
          emptyState.className = 'journal-empty-state';
          emptyState.innerHTML = '<p>No sessions match your filters.</p>';
          container.appendChild(emptyState);
        }
        emptyState.style.display = 'block';
      } else if(emptyState) {
        emptyState.style.display = 'none';
      }

      const parts = [];
      parts.push(filtered.length + ' match');
      if(kwTokens.length) parts.push('keywords: ' + kwTokens.join(', '));
      if(beforeVal) parts.push('before ' + formatDate(beforeVal));
      parts.push('total ' + cards.length);
      statusEl.textContent = parts.join(' · ');
    }

    const applyFiltersDebounced = debounce(applyFilters, 160);

    beforeInput.addEventListener('change', applyFilters);
    keywordInput.addEventListener('input', applyFiltersDebounced);
    resetBtn.addEventListener('click', () => {
      beforeInput.value = '';
      keywordInput.value = '';
      applyFilters();
      keywordInput.focus();
    });

    applyFilters();
  })();
</script>
