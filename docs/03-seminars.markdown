---
layout: page
title: Seminars
permalink: /seminars/
order: 4
---


<style>
h3 {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  padding-right: 150px; 
  font-size: 1.2em;
}

.tags {
  position: absolute;
  top: 0.8rem;
  right: 0.9rem;

  display: flex;
  flex-direction: column;
  gap: 4px;
  align-items: flex-end;
}
.tag {
  font-size: 1.1em;
  font-weight: 700;
  color: black;
  background: #eef2ff;
  padding: 2px 8px;
  border-radius: 6px;
  white-space: nowrap;
  margin-top: 0.2rem;
}
@media (max-width: 768px) {
  .hero-section-fullscreen {
    background: linear-gradient(135deg, rgba(30, 42, 58, 0.85), rgba(212, 165, 116, 0.3)), url('{{ "/images/hero_simple.png" | relative_url }}') 80% center/100% no-repeat;
  }
}
#bulletin-board dl{
  position: relative;
  display: grid;
  grid-gap: 4px 16px;
  grid-template-columns: minmax(20ch, max-content) 1fr;
  border: 1px solid var(--border-color);
  border-radius: 12px;
  padding: 0.2rem 0.5rem 0.5rem;
  margin-bottom: 0.5em;
  transition: border-color 0.25s ease, transform 0.25s ease, box-shadow 0.25s ease;
}
#bulletin-board dl:hover{
  border-color: var(--accent-color);
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
  transform: translateY(-2px);
}
#bulletin-board dt
{
  background: var(--accent-color);
  color: var(--yang-light);
  padding: 0.2rem 0.5rem;
  margin-top: 0.3rem;
  border-radius: 4px;
  font-weight: 600;
  font-size: 1.5rem;
  letter-spacing: 0.5px;
  display: inline-block;
  align-self: start;
  white-space: nowrap;
  width: minmax(20ch, max-content);
  overflow: visible;
  text-align: right;
}
#bulletin-board dd
{
  background: white;
  color: var(--text-primary) !important;
  padding: 0.2rem 0.5rem;
  border-radius: 8px;
  font-weight: 600;
  font-size: 0.85rem;
  letter-spacing: 0.5px;
  margin-top: 0.3rem;
  display: inline-block;
  grid-column-start: 2;
}

/* mobile env*/ 
@media (max-width: 768px) {
  h3 {
    padding-right: 0;              /* remove reserved space */
    flex-direction: column;        /* stack */
    align-items: flex-start;
  }

  .tags {
    position: static;              /* 👈 back into flow (inside h3) */
    display: flex;
    flex-direction: row;           /* or column if you prefer */
    gap: 6px;
    margin-top: 4px;

    align-self: flex-end;          /* 👈 keep them right-aligned */
  }
  
  #bulletin-board dl {
    grid-template-columns: 1fr;   /* single column */
  }

  #bulletin-board dt {
    grid-column: 1;              /* ensure full width */
    text-align: left;            /* optional: better for mobile */
    width: auto;                 /* override your fixed width */
  }

  #bulletin-board dd {
    grid-column: 1;
  }
}

#bulletin-board li > details {
  list-style: none;
}
#bulletin-board li:has(> details) {
  list-style: none;
}

#bulletin-board details[open] summary::after {
  content: attr(data-open);
}

#bulletin-board details:not([open]) summary::after {
  content: attr(data-close);
}
</style>

<section class="hero-section hero-tight">
  <div class="wrapper">
    <h1 class="hero-title">Seminars</h1>
    <p class="hero-subtitle">AI + High Energy Physics research presentations and discussions</p>
  </div>
</section>


<div id="bulletin-board" markdown=1>

Our online joint seminars are at the intersection of AI and fundamental physics open to all participants. We are open to all interested participants across East Asia and beyond. For zoom links, please check out our slack channel or contact organizers.

Upcoming Seminars
-----------------

May 20 (Wed)
: ### TBA
  <span class="tags">
    <span class="tag">#CTPU-PTC seminar</span>
  </span>

  * Speaker: Marie Hein (RWTH Aachen)
  * Time: 3:00 PM JST/KST, 2:00 PM Beijing

<!-- ----------------------------------- -->


Mar. 24 (Tue)
: ### Connecting Simulations and Observations with Differentiable Simulations and Field Level Inference
  <span class="tags">
    <span class="tag">#AI4KMI seminar</span>
  </span>

  * Speaker: Benjamin Horowitz (IPMU)
  * Time: 5:00 PM JST/KST, 4:00 PM Beijing
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      The rapid growth of both astrophysical data and simulation capabilities is creating a new opportunity. Instead of being tied to summary statistics (like correlation functions and power spectra), we can begin to connect simulations and observations directly at the field level. In this talk, I will present a framework for field-level, multi-probe inference built around differentiable simulations, where gradients can be propagated through the forward model itself. I will focus on diffhydro, a differentiable hydrodynamics framework written in JAX that combines modern multiphysics solvers with end-to-end automatic differentiation. Starting from simple dark-matter models, we can incrementally add more realistic physics, including turbulence, radiative heating and cooling, and self-gravity, while retaining the ability to optimize directly through the simulation. This makes it possible to connect observations to initial conditions (i.e. latent fields), physical parameters, and unresolved processes in a unified way. I will show how these ideas open the door to reconstructing the history of the Universe and how the same framework can be a platform for embedded machine learning models for additional acceleration and new physics discovery.
    </details>

<!-- ----------------------------------- -->

Past Seminars 2026
-------------

Mar. 18 (Wed)
: ### How LLM can help particle physicists 
  <span class="tags">
    <span class="tag">#AI4KMI seminar</span>
  </span>

  * Speaker: Mihoko Nojiri (KEK)
  * Time: 5:00 PM JST/KST, 4:00 PM Beijing
  * [link to the seminar page](https://www.kmi.nagoya-u.ac.jp/eng/seminar/3497/)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      In this talk, I want to discuss evolving field of application of LLM to the scientific coding. The HEP analysis often require lengthy coding of high reliability. We introduce CoLLM, which allows to generate analysis code from the LLM prompts quickly. The package include the automatic bug fixing, and it is now quickly evolving toward code reviews and refinements. I also comments the possible application to the other field and implication from brain functions.
    </details>

<!-- ----------------------------------- -->

Jan. 29 (Thu)
: ### Status on Generative Unfolding 
  <span class="tags">
    <span class="tag">#AI4KMI seminar</span>
  </span>

  * Speaker: Sofia Palacios (Rutgers University)
  * Time: 5:00 PM JST/KST, 4:00 PM Beijing
  * [link to the seminar page](https://www.kmi.nagoya-u.ac.jp/eng/seminar/3484/)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      Generative machine learning has become a powerful tool for unbinned, high-dimensional unfolding at the LHC.
This talk highlights recent progress on key open challenges: scaling to hundreds of dimensions, prior-independent parameter estimation, and the path toward fully analysis-ready unfolding.
    </details>

<!-- ----------------------------------- -->

Jan. 13 (Tue)
: ### Generative AI in Cosmology 
  <span class="tags">
    <span class="tag">#AI4KMI seminar</span>
  </span>

  * Speaker: Leander Thiele (IPMU)
  * Time: 3:00 PM JST/KST, 2:00 PM Beijing
  * [link to the seminar page](https://www.kmi.nagoya-u.ac.jp/eng/seminar/3469/)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      Increasing data volumes, pushing to non-linear scales, create opportunities for machine learning in cosmology. One primary challenges is the inverse problem implicitly defined through simulations. Neural simulation-based inference is increasingly being recognized as a tool. I will review this technique and present some work both on observational data as well as on methodological development, specifically multi-fidelity inference. In the second part of the talk, I will present recent work on probabilistic identification of cosmic voids.
    </details>

<!-- ----------------------------------- -->

Past Seminars 2025
------------------

Dec. 19 (Fri)
: ### Physics-Driven Learning for Solving Inverse Problems in QCD Physics 
  <span class="tags">
    <span class="tag">#AI4KMI seminar</span>
  </span>

  * Speaker: Lingxiao Wang (RIKEN)
  * Time: 5:00 PM JST/KST, 4:00 PM Beijing
  * [link to the seminar page](https://www.kmi.nagoya-u.ac.jp/eng/seminar/3443/)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      Discovery in the physical sciences relies on inverse modeling of observations. The combination of deep learning and physics-driven designs is reshaping how we solve inverse problems for extracting physical properties from data. This is particularly relevant for quantum chromodynamics (QCD), where non-trivial symmetries make both data interpretation and computation challenging. In this talk, I will present physics-driven learning from a probabilistic perspective, with a focus on applications in QCD physics. Examples include learning spectral functions and hadron forces from lattice QCD data, reconstructing hadron emission sources from Femtoscopy, and extracting the equation of state from neutron-star observations. If time permits, I will also introduce the physics of diffusion models and discuss physics-driven designs that enable expandable and reliable sampling for accelerating simulations.
    </details>

</div>


<div class="wrapper">

  <!--
  <section class="content-section">
    <h2 class="section-title">Upcoming</h2>
    <div class="card simple-card">
      <header class="card-head">
        <h3 class="card-title">🗓️ Fall 2025 Series</h3>
      </header>
      <p class="card-status"><strong>Schedule coming soon</strong></p>
      <!-- <p class="card-hint">We are finalizing invited speakers and dates.</p>
      <div class="card-actions">
        <a href="mailto:contact@ai-hep.org" class="btn btn-outline">Get Updates</a> 
      <!-- </div> 
    </div>
  </section>
  -->
 
  <section class="content-section">
    <h2 class="section-title">Participate</h2>
    <div class="highlight-box compact">
      <div class="participate-grid">
        <div>
          <h3 class="inline-heading"> Present Your Work</h3>
          <p>We welcome proposals from researchers at all career stages. Send a short abstract or idea to the Organizers!</p>
          <div class="btn-row">
            <a href="https://groups.google.com/g/hep-aiea" class="btn">Propose a Talk</a>
          </div>
        </div>

        <div>
          <h3 class="inline-heading"> Advertise Your Seminars</h3>
          <p>Share your own seminars and events with the community via our Slack workspace.</p>
          <div class="btn-row">
            <a href="mailto:tianjiresearch@gmail.com,vmikuni@cern.ch,huilin.qu@cern.ch?subject=Request%20Slack%20invitation%20for%20AI%20%2B%20HEP&body=Hi%2C%0A%0AI%27d%20like%20to%20join%20the%20AI%2BHEP%20East%20Asia%20Slack%20workspace.%0A%0AName%3A%20%0AInstitution%3A%20%0AResearch%20interests%3A%20%0A%0AThank%20you%21" class="btn">Join Slack</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</div>
