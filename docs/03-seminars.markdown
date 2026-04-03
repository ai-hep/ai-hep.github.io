---
layout: page
title: Seminars
permalink: /seminars/
order: 4
---


<style>
h1 {
  width: 100vw;
  margin-left: calc(50% - 50vw);
  margin-right: calc(50% - 50vw);

  background: linear-gradient(135deg, var(--yin-dark) 0%, #3b4a7a 100%);

  text-align: center;
  padding: 3rem 1rem;
  font-size: 3rem !important;
  font-weight: 700 !important;

  color: white;
}
h1::after {
  content: "AI + High Energy Physics research presentations and discussions";
  display: block;
  margin-top: 1.0rem;
  font-size: 1.2rem;
  font-weight: 400;
  color: rgba(255,255,255,0.9);
}

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

<!--
<section class="hero-section hero-tight">
  <div class="wrapper">
    <h1 class="hero-title">Seminars</h1>
    <p class="hero-subtitle">AI + High Energy Physics research presentations and discussions</p>
  </div>
</section>
-->
<!--
<p class="subtitle">
AI + High Energy Physics research presentations and discussions
</p>
-->


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

Past Seminars 2026
-------------


Apr. 1 (Wed)
: ### Neural Networks from the Perspective of Physics
  <span class="tags">
    <span class="tag">#CTPU-PTC seminar</span>
  </span>

  * Speaker: Jaeok Yi (KAIST)
  * Time: 3:00 PM JST/KST, 2:00 PM Beijing
  * [link to the seminar page](https://indico.ibs.re.kr/event/1254/)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      Despite the remarkable empirical success of deep learning, a comprehensive theoretical understanding of why and how neural networks learn remains a mystery. In this talk, we discuss physics-inspired approaches to understanding neural networks. We present synaptic field theory, a framework that reformulates the gradient descent dynamics of synaptic weights as classical field dynamics in de Sitter spacetime, constructing an action whose metric naturally matches that of a universe with a positive cosmological constant. This framework faces a challenge related to the non-locality of the cost function. To address this issue, we explore the idea of promoting neurons to dynamical degrees of freedom. Leveraging properties of stochastic gradient descent, the Lagrangian can be decomposed into a data-independent bulk part and a data-dependent boundary part. This decomposition is expected to separate the architectural structure from the stochastic properties of neural networks, enabling independent analysis of each. Through this line of research, we aim to provide physicists with a familiar language to investigate the theoretical foundations of machine learning.
    </details>

<!-- ----------------------------------- -->

Mar. 24 (Tue)
: ### Connecting Simulations and Observations with Differentiable Simulations and Field Level Inference
  <span class="tags">
    <span class="tag">#AI4KMI seminar</span>
  </span>

  * Speaker: Benjamin Horowitz (IPMU)
  * Time: 5:00 PM JST/KST, 4:00 PM Beijing
  * [link to the seminar page](https://www.kmi.nagoya-u.ac.jp/eng/seminar/3501/)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      The rapid growth of both astrophysical data and simulation capabilities is creating a new opportunity. Instead of being tied to summary statistics (like correlation functions and power spectra), we can begin to connect simulations and observations directly at the field level. In this talk, I will present a framework for field-level, multi-probe inference built around differentiable simulations, where gradients can be propagated through the forward model itself. I will focus on diffhydro, a differentiable hydrodynamics framework written in JAX that combines modern multiphysics solvers with end-to-end automatic differentiation. Starting from simple dark-matter models, we can incrementally add more realistic physics, including turbulence, radiative heating and cooling, and self-gravity, while retaining the ability to optimize directly through the simulation. This makes it possible to connect observations to initial conditions (i.e. latent fields), physical parameters, and unresolved processes in a unified way. I will show how these ideas open the door to reconstructing the history of the Universe and how the same framework can be a platform for embedded machine learning models for additional acceleration and new physics discovery.
    </details>
    
<!-- ----------------------------------- -->

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

Jan. 29 (Thu)
: ### Storage Capacity of Perceptron with Variable Selection
  <span class="tags">
    <span class="tag">#DEEP-IN seminar</span>
    <span class="tag">#iPI seminar</span>
  </span>

  * Speaker: Yingying Xu (University of Helsinki)
  * Time: 4:00 PM JST/KST, 3:00 PM Beijing
  * [link to the seminar page](https://ithems.riken.jp/en/events/deep-in-ipi-joint-meeting)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      A central challenge in machine learning is to distinguish genuine structure from chance correlations in high-dimensional data. In this work, we address this issue for the perceptron, a foundational model of neural computation. Specifically, we investigate the relationship between the pattern load α and the variable selection ratio ρ for which a simple perceptron can perfectly classify P = αN random patterns by optimally selecting M = ρN variables out of N variables. While the Cover–Gardner theory establishes that a random subset of ρN dimensions can separate αN random patterns if and only if α < 2ρ, we demonstrate that optimal variable selection can surpass this bound by developing a method, based on the replica method from statistical mechanics, for enumerating the combinations of variables that enable perfect pattern classification. This not only provides a quantitative criterion for distinguishing true structure in the data from spurious regularities, but also yields the storage capacity of associative memory models with sparse asymmetric couplings.
    </details>

<!-- ----------------------------------- -->

Jan. 29 (Thu)
: ### Physics of Machine Learning
  <span class="tags">
    <span class="tag">#DEEP-IN seminar</span>
    <span class="tag">#iPI seminar</span>
  </span>

  * Speaker: Gert Aarts (Swansea University)
  * Time: 2:30 PM JST/KST, 1:30 PM Beijing
  * [link to the seminar page](https://ithems.riken.jp/en/events/deep-in-ipi-joint-meeting)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      In recent years machine learning (ML) has started to make impact in lattice field theory (LFT), e.g. for the generation of ensembles of configurations. In this talk I will explore potential impact in the opposite direction, i.e. using theoretical physics to understand ML approaches. I will relate stochastic gradient descent to random matrix theory and then make the connection between neural networks and disordered systems, leading to a neural network phase diagram in the plane spanned by hyper parameters. I will conclude with the possible impact of our findings for practical ML applications.
    </details>

<!-- ----------------------------------- -->

Jan. 28 (Wed)
: ### Understanding Galactic Dark Matter with Generative Models
  <span class="tags">
    <span class="tag">#DEEP-IN seminar</span>
    <span class="tag">#iPI seminar</span>
  </span>

  * Speaker: Sung Hak Lim (IBS)
  * Time: 2:30 PM JST/KST, 1:30 PM Beijing
  * [link to the seminar page](https://ithems.riken.jp/en/events/deep-in-ipi-joint-meeting)
  * <details>
      <summary data-open="Abstract" data-close="Show Abstract"></summary>
      Mapping the Milky Way’s dark matter requires moving beyond traditional, rigid dynamical models. In this talk, generative models — specifically Normalizing Flows — are used to learn the stellar phase space distribution directly from Gaia data. This approach enables a flexible, model-independent reconstruction of the Galactic gravitational potential and local dark matter density. These data-driven techniques provide a promising avenue to handle complex observational biases and what they reveal about the dark sector’s influence on our Galaxy.
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
