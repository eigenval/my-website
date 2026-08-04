---
layout: default
title: Home
---


<div class="intro">
  <img src="{{ site.baseurl }}/assets/images/SelfPhoto.jpeg" alt="Your Name" class="profile-photo">

  <div class="welcome-trilingual">
    <span class="welcome-word welcome-hi" lang="hi">स्वागतम्</span>
    <span class="welcome-sep">&middot;</span>
    <span class="welcome-word welcome-en">Welcome</span>
    <span class="welcome-sep">&middot;</span>
    <span class="welcome-word welcome-fr">Bienvenue</span>
  </div>

  <p>
    Hi, I'm <strong>Anagh</strong>, a neuroscientist and computational modeler. I'm currently a postdoctoral researcher at the University of Strasbourg, where I build computational models to better understand how the brain works in health and disease.
  </p>

  <p>
    Before moving to France, I completed my PhD at the National Brain Research Centre (NBRC), India, studying the dynamics of healthy and aging brains. Before neuroscience took over my life, I trained in engineering and physics—backgrounds that continue to shape how I think about complex systems.
  </p>

  <p>
    I'm fascinated by the intersection of neuroscience, dynamical systems, and artificial intelligence. While modern AI has achieved extraordinary successes, I believe there is still much it can learn from the principles that govern biological intelligence. Understanding how brains compute, adapt, and give rise to cognition remains, to me, one of the most compelling scientific challenges of our time.
  </p>

  <p>
    Outside the lab, I'm a happy dilettante—or perhaps a <em>flâneur</em>—with an enduring curiosity for philosophy, history, literature, geopolitics, culture, and strength training. I enjoy wandering across disciplines, convinced that some of the best ideas emerge at their intersections.
  </p>

  <p>
    This blog is a collection of my thoughts on science and life: essays on neuroscience and AI, reflections on research, notes on books and ideas, and the occasional detour into topics that simply capture my curiosity.
  </p>

  <p>
    Thanks for stopping by. I hope you find something here that makes you think.
  </p>
</div>

<style>
  .welcome-trilingual {
    display: flex;
    flex-wrap: wrap;
    align-items: baseline;
    justify-content: center;
    gap: 0.5em;
    margin: 0.6em 0 1em;
    text-align: center;
  }
  .welcome-word {
    font-size: 2em;
    font-weight: 700;
    line-height: 1.2;
  }
  .welcome-hi {
    font-family: "Noto Sans Devanagari", "Kohinoor Devanagari", "Nirmala UI", sans-serif;
  }
  .welcome-fr {
    font-style: italic;
    font-weight: 600;
  }
  .welcome-sep {
    color: #bbb;
    font-size: 1.5em;
  }
  @media (max-width: 500px) {
    .welcome-word {
      font-size: 1.4em;
    }
  }
</style>
