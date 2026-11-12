---
layout: splash
title: "Call for submissions"
permalink: /call-for-submissions/
hidden: true
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Source+Sans+3:wght@400;600;700;800&display=swap" rel="stylesheet">

{% comment %}
  Shared styles: /assets/css/hpc-days.css (same file as the other pages).
  Page-specific styles are in the <style> block at the bottom of this file.
  submit_url: single submission form. If empty, buttons open an email to contact_email.
  Deadlines: edit the data-date / data-deadline attributes AND the visible text together.
{% endcomment %}
<link rel="stylesheet" href="{{ '/assets/css/hpc-days.css' | relative_url }}">

{% assign submit_url = "" %}
{% assign contact_email = "" %}

{% capture mail_workshop %}mailto:{{ contact_email }}?subject=Durham%20HPC%20Days%202027%3A%20Workshop%20proposal{% endcapture %}
{% capture mail_tutorial %}mailto:{{ contact_email }}?subject=Durham%20HPC%20Days%202027%3A%20Tutorial%20proposal{% endcapture %}
{% capture mail_talk %}mailto:{{ contact_email }}?subject=Durham%20HPC%20Days%202027%3A%20Talk%20proposal{% endcapture %}
{% capture mail_poster %}mailto:{{ contact_email }}?subject=Durham%20HPC%20Days%202027%3A%20Poster%20proposal{% endcapture %}
{% assign href_workshop = submit_url | default: mail_workshop %}
{% assign href_tutorial = submit_url | default: mail_tutorial %}
{% assign href_talk = submit_url | default: mail_talk %}
{% assign href_poster = submit_url | default: mail_poster %}

<div class="hpc" id="hpc" data-opens="2026-12-01T00:00:00">
  <div class="hpc-progress" aria-hidden="true"></div>

  <!-- ===== HEADER ===== -->
  <header class="hpc-pagehead" id="top">
    <div class="hpc-in">
      <nav class="hpc-crumbs" aria-label="Breadcrumb" data-reveal>
        <a href="{{ '/' | relative_url }}">Home</a>
        <span aria-hidden="true">/</span>
        <span aria-current="page">Call for submissions</span>
      </nav>
      <p class="hpc-host" data-reveal style="--i:1">Durham HPC Days 2027 · 12 to 16 July</p>
      <h1 data-reveal style="--i:1">Call for submissions</h1>
      <p class="hpc-lede" data-reveal style="--i:2">We are seeking workshops, tutorials, talks and posters on the theme “Sustainable Computing for Science”.</p>
    </div>
  </header>

  <!-- ===== TIMELINE ===== -->
  <section class="hpc-section" id="deadlines">
    <div class="hpc-in">
      <h2 data-reveal>Key dates</h2>
      <p class="cs-next" id="cs-next" data-reveal style="--i:1" hidden></p>
      <ol class="cs-tl" data-reveal style="--i:1">
        <li data-date="2026-12-01T00:00:00">
          <span class="cs-tl-date"><b>1</b> Dec 2026</span>
          <span class="cs-tl-what">Call opens</span>
        </li>
        <li class="cs-key" data-date="2027-01-25T23:59:00">
          <span class="cs-tl-date"><b>25</b> Jan 2027</span>
          <span class="cs-tl-what">Deadline: <strong>workshops and tutorials</strong></span>
        </li>
        <li class="cs-key" data-date="2027-03-12T23:59:00">
          <span class="cs-tl-date"><b>12</b> Mar 2027</span>
          <span class="cs-tl-what">Deadline: <strong>contributed talks</strong></span>
        </li>
        <li class="cs-key" data-date="2027-04-16T23:59:00">
          <span class="cs-tl-date"><b>16</b> Apr 2027</span>
          <span class="cs-tl-what">Deadline: <strong>posters</strong></span>
        </li>
        <li class="cs-key" data-date="2027-05-14T23:59:00">{% comment %} PLACEHOLDER DATE: confirm, then update here, in the card notes and in data-date {% endcomment %}
          <span class="cs-tl-date"><b>14</b> May 2027</span>
          <span class="cs-tl-what">Final details due: <strong>workshops and tutorials</strong><em>Speakers, programme, requirements</em></span>
        </li>
        <li class="cs-final" data-date="2027-07-16T23:59:00">
          <span class="cs-tl-date"><b>12–16</b> Jul 2027</span>
          <span class="cs-tl-what">Durham HPC Days</span>
        </li>
      </ol>
    </div>
  </section>

  <!-- ===== FORMATS ===== -->
  <section class="hpc-section hpc-alt" id="calls">
    <div class="hpc-in">
      <h2 data-reveal>Choose a format</h2>
      <p class="hpc-sub" data-reveal style="--i:1">All contributions go through one submission form. Every abstract is a maximum of 300 words.</p>

      <div class="cs-calls">

        <article class="cs-card" id="workshops" style="--c: var(--s-workshop)" data-reveal>
          <div class="cs-when" data-deadline="2027-01-25T23:59:00">
            <span class="cs-when-label">Deadline</span>
            <span class="cs-when-day">25</span>
            <span class="cs-when-month">Jan 2027</span>
            <span class="cs-status"></span>
          </div>
          <div class="cs-body">
            <h3>Workshops</h3>
            <p class="cs-meta">Half day · two 90-minute slots</p>
            <p class="cs-also"><strong>Final details by 14 May 2027:</strong> confirmed speakers, final programme and requirements.</p>
            <p>Interactive sessions on a topic you organise, with discussion, practical activities or collaborative work. Accepted workshops can take talks from the talk call.</p>
            <details class="cs-more">
              <summary>What to prepare</summary>
              <ul class="cs-list">
                <li>Title and abstract</li>
                <li>Provisional agenda for the two slots</li>
                <li>Provisional speakers and contributors</li>
                <li>One session leader</li>
                <li>Best-fit area</li>
              </ul>
            </details>
            <p class="cs-action"><a class="hpc-btn hpc-btn-purple" href="{{ href_workshop }}">Submit a workshop</a></p>
          </div>
        </article>

        <article class="cs-card" id="tutorials" style="--c: var(--s-tutorial); --i:1" data-reveal>
          <div class="cs-when" data-deadline="2027-01-25T23:59:00">
            <span class="cs-when-label">Deadline</span>
            <span class="cs-when-day">25</span>
            <span class="cs-when-month">Jan 2027</span>
            <span class="cs-status"></span>
          </div>
          <div class="cs-body">
            <h3>Tutorials</h3>
            <p class="cs-meta">90 or 180 minutes · lab room</p>
            <p class="cs-also"><strong>Final details by 14 May 2027:</strong> confirmed programme, materials and requirements.</p>
            <p>Structured, hands-on training that teaches a particular skill, technique or tool.</p>
            <details class="cs-more">
              <summary>What to prepare</summary>
              <ul class="cs-list">
                <li>Title and abstract</li>
                <li>Level (beginner, intermediate, advanced) and prerequisites</li>
                <li>Maximum class size and preferred duration</li>
                <li>Software, hardware, licences or accounts participants need</li>
              </ul>
            </details>
            <p class="cs-action"><a class="hpc-btn hpc-btn-purple" href="{{ href_tutorial }}">Submit a tutorial</a></p>
          </div>
        </article>

        <article class="cs-card" id="talks" style="--c: var(--s-talk)" data-reveal>
          <div class="cs-when" data-deadline="2027-03-12T23:59:00">
            <span class="cs-when-label">Deadline</span>
            <span class="cs-when-day">12</span>
            <span class="cs-when-month">Mar 2027</span>
            <span class="cs-status"></span>
          </div>
          <div class="cs-body">
            <h3>Talks</h3>
            <p class="cs-meta">25 minutes, including questions</p>
            <p>Research, technical developments, experiences, lessons learned or new ideas. Talks join a related workshop or an open session.</p>
            <details class="cs-more">
              <summary>What to prepare</summary>
              <ul class="cs-list">
                <li>Title and abstract</li>
                <li>Speaker and co-authors</li>
                <li>Best-fit area</li>
            
              </ul>
            </details>
            <p class="cs-action"><a class="hpc-btn hpc-btn-purple" href="{{ href_talk }}">Submit a talk</a></p>
          </div>
        </article>

        <article class="cs-card" id="posters" style="--c: var(--s-keynote); --i:1" data-reveal>
          <div class="cs-when" data-deadline="2027-04-16T23:59:00">
            <span class="cs-when-label">Deadline</span>
            <span class="cs-when-day">16</span>
            <span class="cs-when-month">Apr 2027</span>
            <span class="cs-status"></span>
          </div>
          <div class="cs-body">
            <h3>Posters</h3>
            <p class="cs-meta">One-to-one conversations</p>
            <p>A relaxed way to present your work and meet people. Early-career researchers are especially welcome.</p>
            <details class="cs-more">
              <summary>What to prepare</summary>
              <ul class="cs-list">
                <li>Title and abstract</li>
                <li>Presenter and co-authors</li>
                <li>Best-fit area</li>
              </ul>
            </details>
            <p class="cs-action"><a class="hpc-btn hpc-btn-purple" href="{{ href_poster }}">Submit a poster</a></p>
          </div>
        </article>

      </div>
    </div>
  </section>

  <!-- ===== AREAS ===== -->
  <section class="hpc-section" id="tracks">
    <div class="hpc-in">
      <h2 data-reveal>Three areas within the theme</h2>
      <p class="hpc-sub" data-reveal style="--i:1">You will pick the best fit when you submit. Topics are examples, not restrictions: any HPC-related contribution is welcome, and each day has an open session.</p>

      <div class="cs-tracks">
        <div class="cs-track" style="--c: var(--s-talk)" data-reveal>
          <h3>Systems and software</h3>
          <p class="cs-q">How do we build and maintain efficient, reliable and sustainable computing?</p>
          <p class="cs-eg">GPU and node performance, energy-aware computing, performance portability, compilers, testing and CI, legacy code, research software sustainability.</p>
        </div>
        <div class="cs-track" style="--c: var(--s-tutorial); --i:1" data-reveal>
          <h3>AI and simulation</h3>
          <p class="cs-q">How can simulation and AI be more sustainable, effective and accessible?</p>
          <p class="cs-eg">Simulation at scale, digital twins, ML surrogates, AI for discovery, uncertainty quantification, reproducible workflows.</p>
        </div>
        <div class="cs-track" style="--c: var(--s-social); --i:2" data-reveal>
          <h3>People and communities</h3>
          <p class="cs-q">How do we sustain the people, skills and communities behind scientific computing?</p>
          <p class="cs-eg">Knowledge exchange, EDI, RSE career paths, training, research facilitation, funding and policy, community building.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- ===== SELECTION + QUESTIONS ===== -->
  <section class="hpc-band" id="questions">
    <div class="hpc-in hpc-split">
      <div data-reveal>
        <h2>How we select</h2>
        <p>Two programme committee members review each submission for quality, relevance, interaction, and a diverse mix of topics, perspectives and speakers. Fit with the theme helps but is not required.</p>
      </div>
      <div data-reveal style="--i:1">
  <h2>Questions?</h2>
  <p>Unsure which format suits your idea? Get in touch before the deadline:
    <a href="mailto:{{ site.email }}">{{ site.email }}</a>
  </p>
  <p class="hpc-actions">
    <a class="hpc-btn hpc-btn-white" href="mailto:{{ site.email }}?subject=Durham%20HPC%20Days%202027%3A%20Question%20about%20submissions">Email us</a>
    <a class="hpc-btn hpc-btn-ghost" href="{{ '/' | relative_url }}">Back to Home</a>
  </p>
</div>
    </div>
  </section>

  <button type="button" class="hpc-top" aria-label="Back to top">↑</button>
</div>

<style>
/* ===== Next-deadline banner ===== */
.hpc .cs-next { display: inline-block; margin: 18px 0 0; padding: 10px 16px; background: rgba(255,255,255,.08); border-left: 4px solid var(--purple-light); font-size: 17px; }
.hpc .cs-next strong { color: #fff; }

/* ===== Timeline ===== */
.cs-tl { list-style: none; margin: 28px 0 0; padding: 0; display: grid; grid-template-columns: repeat(6, minmax(0, 1fr)); position: relative; }
.cs-tl li { position: relative; padding: 34px 14px 0 0; }
.cs-tl li:before { content: ""; position: absolute; top: 8px; left: 0; width: 16px; height: 16px; border-radius: 50%; background: var(--card); border: 3px solid var(--muted); z-index: 1; }
.cs-tl li:after { content: ""; position: absolute; top: 14px; left: 0; right: 0; height: 4px; background: var(--line); }
.cs-tl li:last-child:after { right: 50%; }
.cs-tl li.past:after { background: var(--purple-light); }
.cs-tl li.past:before { background: var(--purple-light); border-color: var(--purple-light); }
.cs-tl li.cs-key:before { width: 24px; height: 24px; top: 4px; border-color: #fff; }
.cs-tl li.next:before { background: #fff; border-color: var(--purple-light); box-shadow: 0 0 0 6px rgba(255,255,255,.18); }
.cs-tl-date { display: block; color: var(--muted); font-size: 15px; font-weight: 700; text-transform: uppercase; letter-spacing: .04em; }
.cs-tl-date b { color: #fff; font-size: 34px; font-weight: 800; line-height: 1; margin-right: 4px; }
.cs-tl li.next .cs-tl-date b { color: var(--purple-light); }
.cs-tl-what { display: block; margin-top: 6px; font-size: 16px; line-height: 1.4; }
.cs-tl-what em { display: block; color: var(--muted); font-size: 14px; }
.cs-tl li.past { opacity: .6; }

/* ===== Format cards ===== */
.cs-calls { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 22px; }
.cs-card { --c: var(--purple-light); display: grid; grid-template-columns: 130px 1fr; background: var(--card); border: 1px solid var(--line); border-top: 4px solid var(--c); scroll-margin-top: 24px; }
.cs-when { display: flex; flex-direction: column; align-items: center; gap: 2px; padding: 24px 10px; background: rgba(255,255,255,.04); border-right: 1px solid var(--line); text-align: center; }
.cs-when-label { color: var(--muted); font-size: 12px; font-weight: 700; letter-spacing: .08em; text-transform: uppercase; }
.cs-when-day { color: var(--c); font-size: 54px; font-weight: 800; line-height: 1; }
.cs-when-month { color: #fff; font-size: 16px; font-weight: 700; }
.cs-tag { margin-top: 6px; padding: 2px 8px; border: 1px solid var(--c); color: var(--c); font-size: 12px; font-weight: 700; text-transform: uppercase; }
.cs-status { margin-top: 10px; padding: 4px 10px; background: var(--c); color: var(--ink); font-size: 13px; font-weight: 800; }
.cs-status:empty { display: none; }
.cs-status.closed { background: #F4A3A3; }
.cs-body { padding: 24px 26px; }
.hpc .cs-card h3 { margin: 0 0 4px; color: var(--c); font-size: 28px; }
.hpc .cs-meta { margin: 0 0 12px; color: var(--muted); font-size: 15px; font-weight: 700; }
.hpc .cs-also { margin: 0 0 12px; padding: 8px 12px; background: rgba(255,255,255,.04); border-left: 4px solid var(--c); font-size: 15px; line-height: 1.45; }
.hpc .cs-also strong { color: #fff; }
.cs-more { margin: 14px 0 0; }
.cs-more summary { cursor: pointer; color: #fff; font-weight: 700; }
.cs-more summary:focus-visible { outline: 2px solid var(--purple-light); outline-offset: 3px; }
.hpc .cs-list { margin-top: 10px; }
.hpc .cs-list li { position: relative; margin-bottom: 7px; padding-left: 18px; font-size: 16px; line-height: 1.5; }
.hpc .cs-list li:before { content: ""; position: absolute; left: 0; top: .6em; width: 8px; height: 8px; background: var(--c); }
.hpc .cs-action { margin: 20px 0 0; }

/* ===== Areas ===== */
.cs-tracks { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 18px; }
.cs-track { --c: var(--purple-light); padding: 24px; background: var(--card); border: 1px solid var(--line); border-top: 4px solid var(--c); }
.hpc .cs-track h3 { color: var(--c); font-size: 22px; }
.hpc .cs-track .cs-q { color: #fff; font-weight: 600; }
.hpc .cs-track .cs-eg { margin: 0; color: var(--muted); font-size: 16px; }

@media (max-width: 900px) {
  .cs-calls, .cs-tracks { grid-template-columns: 1fr; }
  .cs-tl { grid-template-columns: 1fr; }
  .cs-tl li { padding: 0 0 26px 40px; }
  .cs-tl li:before { top: 2px; left: 0; }
  .cs-tl li.cs-key:before { top: -2px; left: -4px; }
  .cs-tl li:after { top: 22px; bottom: 0; left: 6px; right: auto; width: 4px; height: auto; }
  .cs-tl li:last-child:after { display: none; }
}
@media (max-width: 520px) {
  .cs-card { grid-template-columns: 1fr; }
  .cs-when { flex-direction: row; flex-wrap: wrap; justify-content: center; align-items: baseline; gap: 4px 10px; border-right: 0; border-bottom: 1px solid var(--line); padding: 14px; }
  .cs-when-day { font-size: 36px; }
  .cs-status { margin-top: 0; }
}
</style>

<script>
(function () {
  var root = document.getElementById('hpc');
  if (!root) return;
  document.documentElement.classList.add('js');
  var reduce = window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  var $ = function (s, c) { return (c || root).querySelector(s); };
  var $$ = function (s, c) { return Array.prototype.slice.call((c || root).querySelectorAll(s)); };

  /* Reveal on scroll */
  var items = $$('[data-reveal]');
  if ('IntersectionObserver' in window && !reduce) {
    var io = new IntersectionObserver(function (es) {
      es.forEach(function (e) { if (e.isIntersecting) { e.target.classList.add('in'); io.unobserve(e.target); } });
    }, { threshold: .08, rootMargin: '0px 0px -40px 0px' });
    items.forEach(function (el) { io.observe(el); });
  } else { items.forEach(function (el) { el.classList.add('in'); }); }

  /* Progress bar + back to top */
  var bar = $('.hpc-progress'), topBtn = $('.hpc-top'), ticking = false;
  function update() {
    var max = document.documentElement.scrollHeight - window.innerHeight;
    if (bar && max > 0) bar.style.transform = 'scaleX(' + Math.min(1, window.scrollY / max) + ')';
    topBtn.classList.toggle('show', window.scrollY > 700);
    ticking = false;
  }
  window.addEventListener('scroll', function () { if (!ticking) { ticking = true; requestAnimationFrame(update); } }, { passive: true });
  update();
  topBtn.addEventListener('click', function () { window.scrollTo({ top: 0, behavior: reduce ? 'auto' : 'smooth' }); });

  /* Deadline chips on cards */
  var opens = new Date(root.getAttribute('data-opens')).getTime();
  function label(t) {
    var now = Date.now(), d = t - now;
    if (!isNaN(opens) && now < opens) return ['Opens 1 Dec', false];
    if (d <= 0) return ['Closed', true];
    var days = Math.ceil(d / 864e5);
    return [days <= 1 ? 'Last day' : days + ' days left', false];
  }
  function refresh() {
    $$('.cs-when[data-deadline]').forEach(function (box) {
      var t = new Date(box.getAttribute('data-deadline')).getTime();
      var s = $('.cs-status', box);
      if (isNaN(t) || !s) return;
      var r = label(t);
      s.textContent = r[0];
      s.classList.toggle('closed', r[1]);
    });

    /* Timeline: mark past + next */
    var now = Date.now(), nextSet = false;
    $$('.cs-tl li').forEach(function (li) {
      var t = new Date(li.getAttribute('data-date')).getTime();
      li.classList.remove('past', 'next');
      if (t < now) li.classList.add('past');
      else if (!nextSet) { li.classList.add('next'); nextSet = true; }
    });

    /* Banner: next upcoming submission deadline */
    var banner = $('#cs-next'), best = null;
    $$('.cs-card').forEach(function (card) {
      var box = $('.cs-when', card);
      var t = new Date(box.getAttribute('data-deadline')).getTime();
      if (t > now && (!best || t < best.t)) best = { t: t, names: [card.querySelector('h3').textContent] };
      else if (best && t === best.t) best.names.push(card.querySelector('h3').textContent);
    });
    if (banner) {
      if (best && now >= opens) {
        var days = Math.ceil((best.t - now) / 864e5);
        var when = new Date(best.t).toLocaleDateString('en-GB', { day: 'numeric', month: 'long', year: 'numeric' });
        banner.innerHTML = 'Next deadline: <strong>' + best.names.join(' and ').toLowerCase() + '</strong>, ' + when + ' (' + (days <= 1 ? 'last day' : days + ' days left') + ')';
        banner.hidden = false;
      } else if (now < opens) {
        banner.innerHTML = 'The call opens on <strong>1 December 2026</strong>.';
        banner.hidden = false;
      } else { banner.hidden = true; }
    }
  }
  refresh(); setInterval(refresh, 3600000);
})();
</script>