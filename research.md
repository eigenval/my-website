---
layout: page
title: Research
permalink: /research/
---


[Google Scholar](https://scholar.google.com/citations?user=QuAclXoAAAAJ&hl=en) &middot; [GitHub](https://github.com/eigenval)

## Selected Papers

My most cited work, according to Google Scholar.

<ul class="paper-list">

  <li class="paper-entry">
    <img class="paper-thumb" src="{{ site.baseurl }}/assets/images/paper-thumbnails/whole-brain-network-models.png" alt="Figure from Whole-Brain Network Models: From Physics to Bedside">
    <div class="paper-body">
      <a class="paper-title" href="https://www.frontiersin.org/journals/computational-neuroscience/articles/10.3389/fncom.2022.866517/full">Whole-Brain Network Models: From Physics to Bedside</a>
      <p class="paper-summary">A review of the field of large-scale whole-brain computational models, tracing how physics-based approaches to neural dynamics are increasingly finding translational application at the clinical bedside.</p>
    </div>
  </li>

  <li class="paper-entry">
    <img class="paper-thumb" src="{{ site.baseurl }}/assets/images/paper-thumbnails/lifespan-coherent-communication.gif" alt="Figure from Lifespan associated global patterns of coherent neural communication">
    <div class="paper-body">
      <a class="paper-title" href="https://www.sciencedirect.com/science/article/pii/S1053811920303116">Lifespan associated global patterns of coherent neural communication</a>
      <p class="paper-summary">Using resting-state MEG recorded across the adult lifespan, we show that the global coherence and metastability of neural oscillations track healthy brain aging, offering compact markers of large-scale change in neural communication.</p>
    </div>
  </li>

  <li class="paper-entry">
    <img class="paper-thumb" src="{{ site.baseurl }}/assets/images/paper-thumbnails/biophysical-mechanism-synchrony.png" alt="Figure from Biophysical mechanism underlying compensatory preservation of neural synchrony over the adult lifespan">
    <div class="paper-body">
      <a class="paper-title" href="https://www.nature.com/articles/s42003-022-03489-4">Biophysical mechanism underlying compensatory preservation of neural synchrony over the adult lifespan</a>
      <p class="paper-summary">We combine dynamical systems modelling with MEG analysis to show that global synaptic scaling compensates for age-related white matter decline, preserving neural synchrony at the peak alpha frequency across the adult lifespan.</p>
    </div>
  </li>

  <li class="paper-entry">
    <img class="paper-thumb" src="{{ site.baseurl }}/assets/images/paper-thumbnails/virtual-ms-patient.jpg" alt="Figure from The virtual multiple sclerosis patient">
    <div class="paper-body">
      <a class="paper-title" href="https://www.cell.com/iscience/fulltext/S2589-0042(24)01326-9">The virtual multiple sclerosis patient</a>
      <p class="paper-summary">We integrate diffusion tensor imaging and MEG into individualized virtual brain models to estimate conduction velocities in MS patients versus controls, offering a route past the clinical-radiological paradox that standard tract-specific measures miss.</p>
    </div>
  </li>

  <li class="paper-entry">
    <div class="paper-thumb paper-thumb-empty" aria-hidden="true"></div>
    <div class="paper-body">
      <a class="paper-title" href="https://www.sciencedirect.com/science/article/abs/pii/S174680941830106X">Automatic seizure detection by modified line length and Mahalanobis distance function</a>
      <p class="paper-summary">We modify the classical line-length feature for seizure detection and combine it with a Mahalanobis-distance classifier across multichannel intracranial EEG, improving seizure-detection accuracy on the Freiburg dataset without added computational cost.</p>
    </div>
  </li>

  <li class="paper-entry">
    <img class="paper-thumb" src="{{ site.baseurl }}/assets/images/paper-thumbnails/metastability-brain-stimulation.png" alt="Figure from Metastability indexes global changes in the dynamic working point of the brain following brain stimulation">
    <div class="paper-body">
      <a class="paper-title" href="https://www.frontiersin.org/journals/neurorobotics/articles/10.3389/fnbot.2024.1336438/full">Metastability indexes global changes in the dynamic working point of the brain following brain stimulation</a>
      <p class="paper-summary">We characterize how single-pulse TMS transiently reduces metastability and increases coherence in global brain network dynamics, with higher EEG frequencies recovering faster than lower ones, offering a way to quantify how long stimulation effects linger.</p>
    </div>
  </li>

  <li class="paper-entry">
    <img class="paper-thumb" src="{{ site.baseurl }}/assets/images/paper-thumbnails/emotion-arousal-aperiodic-eeg.gif" alt="Figure from Emotion arousal but not valence is strongly represented in aperiodic EEG activity">
    <div class="paper-body">
      <a class="paper-title" href="https://www.biorxiv.org/content/10.1101/2024.03.11.584477v1">Emotion arousal but not valence is strongly represented in aperiodic EEG activity stemming from thalamocortical interactions</a>
      <p class="paper-summary">Using the DEAP dataset, we find that the aperiodic EEG exponent and offset track emotional arousal but not valence, and use a thalamocortical neural field model to show this stems from enhanced inhibitory coupling between thalamic reticular and relay populations.</p>
    </div>
  </li>

  <li class="paper-entry">
    <img class="paper-thumb" src="{{ site.baseurl }}/assets/images/paper-thumbnails/thalamic-relay-nuclei.jpg" alt="Figure from Inhibition of thalamic relay nuclei scales the aperiodic and alpha band oscillations associated with arousal">
    <div class="paper-body">
      <a class="paper-title" href="https://direct.mit.edu/imag/article/doi/10.1162/imag_a_00451/127395">Inhibition of thalamic relay nuclei scales the aperiodic and alpha band oscillations associated with arousal during naturalistic stimulus viewing</a>
      <p class="paper-summary">We show that arousal during naturalistic viewing is tracked by a rise in the aperiodic EEG exponent/offset and a drop in alpha power, and use a corticothalamic neural field model to trace both effects to stronger inhibitory drive onto thalamic relay nuclei.</p>
    </div>
  </li>

</ul>

<style>
  .paper-list {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  .paper-entry {
    display: flex;
    gap: 1.2em;
    align-items: flex-start;
    padding: 1.2em 0;
    border-bottom: 1px solid #eaeaea;
  }
  .paper-thumb {
    width: 120px;
    height: 90px;
    object-fit: cover;
    border-radius: 6px;
    border: 1px solid #e2e2e2;
    flex-shrink: 0;
    background: #f7f7f7;
  }
  .paper-thumb-empty {
    display: block;
  }
  .paper-body {
    flex: 1;
    min-width: 0;
  }
  .paper-title {
    display: block;
    font-weight: 700;
    font-size: 1.05em;
    margin-bottom: 0.3em;
  }
  .paper-summary {
    margin: 0;
    color: #333;
  }
  @media (max-width: 500px) {
    .paper-entry {
      gap: 0.8em;
    }
    .paper-thumb {
      width: 72px;
      height: 72px;
    }
  }
</style>
