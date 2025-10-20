---
layout: page
title: Organizers
permalink: /organizers/
order: 2
---

<div class="hero-section" style="padding: 3rem 0; margin-bottom: 3rem;">
  <div class="wrapper">
    <h1 class="hero-title" style="font-size: 2.5rem;">Our Team</h1>
    <p class="hero-subtitle" style="font-size: 1.2rem;">Researchers leading the AI+HEP East Asia community</p>
  </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const wrappers = document.querySelectorAll('.person-bio-wrapper');
  wrappers.forEach(w => {
    const p = w.querySelector('.person-bio');
    const btn = w.querySelector('[data-toggle]');
    if(!p || !btn) return;
    
    // Initialize as clamped
    w.classList.add('is-clamped');
    btn.textContent = 'Read more';
    
    btn.addEventListener('click', () => {
      const isClamped = w.classList.contains('is-clamped');
      if(isClamped){
        w.classList.remove('is-clamped');
        w.classList.add('is-expanded');
        btn.textContent = 'Show less';
      } else {
        w.classList.add('is-clamped');
        w.classList.remove('is-expanded');
        btn.textContent = 'Read more';
      }
    });
  });
});
</script>

<style>
    .person-bio {
        border: none;
        font-size: 0.85rem;
    }    
</style>

<div class="wrapper">
  <div class="content-section">
    <h2 class="section-title">Organizers</h2>
    <p>Our community is guided by dedicated researchers across East Asia advancing AI and high energy physics.</p>

    <div class="organizer-grid">
      <!-- Organizer: Tianji Cai -->
      <div class="person-card">
        <div class="person-media">
          <img src="{{ '/images/tianji.JPG' | relative_url }}" alt="Photo of Tianji Cai" loading="lazy" />
        </div>
        <div class="person-body">
          <h3 class="person-name">Tianji Cai</h3>
          <div class="person-role-block">
            <span class="person-role">Distinguished Researcher (Junior Faculty)</span>
            <span class="person-affiliation">School of Physical Science and Engineering, Tongji University</span>
          </div>
          <ul class="person-tags">
            <li class="person-tag">High Energy Theory</li>
            <li class="person-tag">Particle Physics</li>
            <li class="person-tag">Collider & Jet physics</li>
            <li class="person-tag">AI for Science</li>
            <li class="person-tag">Science for AI</li>
          </ul>
          <div class="person-bio-wrapper" data-bio>
            <p class="person-bio">Tianji Cai (蔡恬吉) is a Distinguished Researcher (junior faculty) at Tongji University (Shanghai, CN). Before, she worked as a postdoctoral research associate in the Fundamental Physics Directorate at the SLAC National Accelerator Laboratory, and as a research affiliate at the Lawrence Berkeley National Laboratory. She obtained her Ph.D. degree in 2023 at University of California, Santa Barbara, and holds two bachelor's degrees from Duke University and Shanghai Jiao Tong University. Her research interest lies at the intersection of High Energy Theory (HEP) and Artificial Intelligence (AI), with the goal towards developing scientific AI. She is actively looking for interested students (undergrads & grads) to join her group, the Ψai Lab.</p>
            <button class="bio-toggle" data-toggle>Read more</button>
          </div>
          <p class="person-contact"><strong>Email:</strong> <a href="mailto:tianjiresearch@gmail.com">tianjiresearch@gmail.com</a></p>
        </div>
      </div>

      <!-- Organizer: Sung Hak Lim (Placeholder Image) -->
      <div class="person-card">
        <div class="person-media placeholder">
          <!-- <div class="placeholder-initials">SL</div> -->
          <img src="{{ '/images/sunghak.png' | relative_url }}" alt="Photo of Sung Hak Lim" loading="lazy" style="width:100%; height:100%; object-fit:contain; object-position:center; background:#f5f5f5;" />
        </div>
        <div class="person-body">
          <h3 class="person-name">Sung Hak Lim</h3>
          <div class="person-role-block">
            <span class="person-role">Senior Researcher</span>
            <span class="person-affiliation">CTPU-PTC, Institute for Basic Science</span>
          </div>
          <ul class="person-tags">
            <li class="person-tag">Galactic Dynamics</li>
            <li class="person-tag">Dark Matter Physics</li>
            <li class="person-tag">Collider & Jet Physics</li>
            <li class="person-tag">ML for Science</li>
          </ul>
          <div class="person-bio-wrapper" data-bio>
            <p class="person-bio">Sung Hak Lim is a Senior Researcher at the Center for Theoretical Physics of the Universe (CTPU-PTC), Institute for Basic Science in South Korea. He earned his Ph.D. from KAIST in 2017, and worked in postdoctoral positions at KEK in Japan (2017-2020) and Rutgers University (2020-2024). His research focuses on combining physics principles with machine learning techniques to advance fundamental physics problems. His current primary work uses advanced neural network methods to map dark matter in the Milky Way and nearby dwarf galaxies. He also develops physics-inspired machine learning methods for identifying particle signals at large hadron colliders and studying dark matter halos of galaxies, with the ultimate goal of revealing the true nature of dark matter.</p>
            <button class="bio-toggle" data-toggle>Read more</button>
          </div>
          <p class="person-contact"><strong>Email:</strong> <a href="mailto:sunghak.lim@ibs.re.kr">sunghak.lim@ibs.re.kr</a></p>
        </div>
      </div>

      <!-- Organizer: Vinicius Mikuni -->
      <div class="person-card">
        <div class="person-media" style="overflow:hidden;">
          <img src="{{ '/images/mikuni.jpg' | relative_url }}" alt="Photo of Vinicius Mikuni" loading="lazy" style="width:100%; height:100%; object-fit:contain; object-position:center; background:#f5f5f5;" />
        </div>    <div class="person-body">
          <h3 class="person-name">Vinicius Mikuni</h3>
          <div class="person-role-block">
            <span class="person-role">Associate Professor</span>
            <span class="person-affiliation">Kobayashi-Maskawa Institute</span>
          </div>
          <ul class="person-tags">
            <li class="person-tag">AI for Science</li>
          </ul>
          <div class="person-bio-wrapper" data-bio>
            <p class="person-bio">Vinicius Mikuni is an Associate Professor using AI for scientific discovery at the KMI Institute. He earned his PhD in 2021 from the University of Zurich, and worked as a Postdoctoral Fellow at Berkeley Lab, California. His research lies at the intersection of machine learning and fundamental science, where he develops algorithms to tackle core challenges in scientific research. His recent work includes fast simulation frameworks for fluid flows, collider physics, nuclear physics, and astrophysics using diffusion-based generative models; innovative methods for solving inverse problems in collider and neutrino physics; and leveraging pre-trained models to accelerate discoveries in particle physics.</p>
            <button class="bio-toggle" data-toggle>Read more</button>
          </div>
          <p class="person-contact"><strong>Email:</strong> <a href="mailto:vmikuni@cern.ch">vmikuni@cern.ch</a></p>
        </div>
      </div>

      <!-- Organizer: Huilin Qu -->
      <div class="person-card">
        <div class="person-media">
          <img src="{{ '/images/huilin.JPG' | relative_url }}" alt="Photo of Huilin Qu" loading="lazy" />
        </div>
        <div class="person-body">
          <h3 class="person-name">Huilin Qu</h3>
          <div class="person-role-block">
            <span class="person-role">Staff Research Physicist</span>
            <span class="person-affiliation">CERN</span>
          </div>
          <ul class="person-tags">
            <li class="person-tag">Jet Tagging</li>
            <li class="person-tag">Deep Learning</li>
            <li class="person-tag">Collider Physics</li>
            <li class="person-tag">AI Integration</li>
          </ul>
          <div class="person-bio-wrapper" data-bio>
            <p class="person-bio">Dr. Huilin Qu (曲慧麟) is a staff research physicist at CERN. He received his B.S. degree from Peking University in 2014 and his Ph.D. from the University of California, Santa Barbara in 2019. His research is at the forefront of artificial intelligence and particle physics, where he has pioneered several innovative deep learning techniques for jet tagging—most notably ParticleNet—which has significantly improved performance and is now widely adopted at the LHC and beyond. As a member of the CMS experiment, Dr. Qu has contributed to searches for Higgs decays to charm quarks and Higgs boson pair production, earning the 2023 CMS Young Researcher Prize for advances in AI-based jet tagging and measurements.</p>
            <button class="bio-toggle" data-toggle>Read more</button>
          </div>
          <p class="person-contact"><strong>Email:</strong> <a href="mailto:huilin.qu@cern.ch">huilin.qu@cern.ch</a></p>
        </div>
      </div>


      <!-- Organizer: Ahmad -->
      <div class="person-card">
        <div class="person-media">
          <img src="{{ '/images/hammad.jpg' | relative_url }}" alt="Photo of Vinicius Mikuni" loading="lazy" style="width:100%; height:100%; object-fit:contain; object-position:center; background:#f5f5f5;" />
        </div>
        <div class="person-body">
          <h3 class="person-name">Ahmed Hammad</h3>
          <div class="person-role-block">
            <span class="person-role">Postdoctoral researcher</span>
            <span class="person-affiliation"> Theory center, High energy accelerator research organization -KEK, Japan</span>
          </div>
          <ul class="person-tags">
            <li class="person-tag">Beyond SM</li>
            <li class="person-tag">Collider phenomenology</li>
            <li class="person-tag">Future colliders</li>
            <li class="person-tag">Jet physics</li>
            <li class="person-tag">AI for science</li>
          </ul>
          <div class="person-bio-wrapper" data-bio>
            <p class="person-bio">Ahmed Hammad is a Postdoctoral Researcher in the Theory Division at the High Energy Accelerator Research Organization (KEK, Tsukuba, Japan). He received his Ph.D. in Theoretical Physics in 2021 from the University of Basel (Switzerland). His research focuses on collider phenomenology and physics beyond the Standard Model, with a particular emphasis on applying advanced machine learning methods, both classical and quantum, to high energy physics. He has contributed to searches for new physics at the LHC and HL-LHC, with work spanning Higgs boson phenomenology, top quark flavor-changing neutral currents and anomaly detection techniques.</p>
            <button class="bio-toggle" data-toggle>Read more</button>
          </div>
          <p class="person-contact"><strong>Email:</strong> <a href="mailto:hamed@post.kek.jp">hamed@post.kek.jp</a></p>
        </div>
      </div>
    </div>
  </div>

  <div class="content-section">
    <h2 class="section-title">International Advisory Committee</h2>
    <p>Distinguished researchers worldwide providing guidance and support to our community.</p>
    
    <div class="advisory-grid">
      <!-- Advisory Member 1 -->
      <div class="advisory-card">
        <h3 class="advisory-name">Mihoko M. Nojiri </h3>
        <p class="advisory-position">Professor</p>
        <p class="advisory-affiliation">KEK, Japan</p>
        <a href="http://www2.kek.jp/theory-center/theory_e/archives/member/nojiri-mihoko/" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>

      <!-- Advisory Member 2 -->
      <div class="advisory-card">
        <h3 class="advisory-name">Satoshi Iso </h3>
        <p class="advisory-position">Professor</p>
        <p class="advisory-affiliation">RIKEN/KEK, Japan</p>
        <a href="http://www2.kek.jp/theory-center/theory_e/archives/member/iso-satoshi/" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>

      <!-- Advisory Member 3 -->
      <div class="advisory-card">
        <h3 class="advisory-name">Koji Hashimoto</h3>
        <p class="advisory-position">Professor</p>
        <p class="advisory-affiliation">Kyoto University, Japan</p>
        <a href="https://www-gauge.scphys.kyoto-u.ac.jp/hashimoto/welcome.html" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>

      <!-- Advisory Member 4 -->
      <div class="advisory-card">
        <h3 class="advisory-name">Yanqing Ma </h3>
        <p class="advisory-position">Professor</p>
        <p class="advisory-affiliation">Peking University, Japan</p>
        <a href="https://faculty.pku.edu.cn/yqma/en/index.htm" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>

      <!-- Advisory Member 5 -->
      <div class="advisory-card">
        <h3 class="advisory-name">David Shih</h3>
        <p class="advisory-position">Professor</p>
        <p class="advisory-affiliation">Rutgers University, USA</p>
        <a href="https://sites.rutgers.edu/david-shih/" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>

      <!-- Advisory Member 6 -->
      <div class="advisory-card">
        <h3 class="advisory-name">Matthew R Buckley </h3>
        <p class="advisory-position">Assistant Professor</p>
        <p class="advisory-affiliation">Rutgers University, USA</p>
        <a href="http://www.physicsmatt.com/" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>

      <!-- Advisory Member 7 -->
      <div class="advisory-card">
        <h3 class="advisory-name"> Gregor Kasieczka </h3>
        <p class="advisory-position">Professor</p>
        <p class="advisory-affiliation">University of Hamburg, Germany</p>
        <a href="https://www.physik.uni-hamburg.de/en/iexp/gruppe-kasieczka.html" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>
      
      <!-- Advisory Member 8 -->
      <div class="advisory-card">
        <h3 class="advisory-name"> Hua Xing Zhu</h3>
        <p class="advisory-position">Professor</p>
        <p class="advisory-affiliation">Peking University, China</p>
        <a href="https://konformal.github.io" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>

      <!-- Advisory Member 8 -->
      <div class="advisory-card">
        <h3 class="advisory-name"> Benjamin Nachman </h3>
        <p class="advisory-position">Associate Professor</p>
        <p class="advisory-affiliation">Stanford University/SLAC, USA</p>
        <a href="https://nachmangroup.github.io/" class="advisory-link" target="_blank" rel="noopener">Personal Website</a>
      </div>
    </div>
  </div>


  <div class="content-section">
    <h2 class="section-title">Volunteers</h2>
    <p>Community volunteers contribute to operations, events, outreach, and technical infrastructure.</p>
    <div class="volunteer-grid">
      <div class="person-card volunteer-card">
        <div class="person-media" style="overflow:hidden; position:relative;">
          <img src="{{ '/images/shiva.jpg' | relative_url }}"
               alt="Photo of Shivasankar K.A"
               loading="lazy"
               style="width:100%; height:100%; object-fit:cover; object-position:center; transform:scale(1.35);">
        </div>
        <div class="person-body">
          <h3 class="person-name">Shivasankar K.A</h3>
          <div class="person-role-block">
            <span class="person-role">Website Design & Admin</span>
            <span class="person-affiliation">PhD Student · Hokkaido University</span>
          </div>
          <ul class="person-tags">
            <li class="person-tag">Astroparticle</li>
            <li class="person-tag">Theory</li>
            <li class="person-tag">Deep Learning</li>
          </ul>
          <div class="person-bio-wrapper" data-bio>
            <p class="person-bio"> Shivasankar is a second-year Ph.D. student at Hokkaido University, Japan. His primary interests lie in theoretical astroparticle physics, where he studies Beyond Standard Model phenomena in astrophysical objects such as black holes, supernovae, and neutron stars, using theory and computation to explore how new physics could manifest. In parallel, he investigates AI-driven approaches in collider physics, specifically studying the physics learned by the models, and explores how concepts from fundamental physics might inspire new developments in AI. When he's not pondering black holes or neural networks, he enjoys learning new skills and exploring the endless possibilities simulated by the Cosmic++ code of the multiverse.</p>
            <button class="bio-toggle" data-toggle>Read more</button>
          </div>
          <p class="person-contact"><strong>Email:</strong> <a href="mailto:a-shiva@particle.sci.hokudai.ac.jp">a-shiva@particle.sci.hokudai.ac.jp</a></p>
        </div>
      </div>
    </div>
  </div>

  <div class="content-section">
    <h2 class="section-title">Get Involved</h2>
    <div class="highlight-box">
      <h3> Join Our Community</h3>
      <p>Interested in contributing to our organizing efforts or participating in our activities? We welcome new members and collaborators who want to advance AI+HEP research and education in East Asia.</p>
      <div style="text-align: center; margin-top: 2rem;">
        <a href="https://groups.google.com/g/hep-aie" class="btn">Contact Us</a>
        <a href="/workshops/" class="btn btn-outline">View events</a>
      </div>
    </div>
  </div>
</div>
