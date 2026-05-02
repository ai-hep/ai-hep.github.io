---
layout: page
title: Organizers
display-title: Our Team
subtitle: Researchers leading the AI+HEP East Asia community
permalink: /organizers/
order: 2
---

<script>
document.addEventListener('DOMContentLoaded', () => {
  document.querySelectorAll('.block-organizers dd').forEach(card => {
    const bio = card.querySelector('.person-bio');
    const btn = card.querySelector('.bio-toggle');
    if (!bio || !btn) return;

    bio.classList.add('is-clamped');

    btn.addEventListener('click', () => {
      const clamped = bio.classList.toggle('is-clamped');
      btn.textContent = clamped ? 'Read more' : 'Show less';
    });
  });
});
</script>


Organizers
----------
<div class="block-organizers" markdown=1>
Our community is guided by dedicated researchers across East Asia advancing AI and high energy physics.

Organizer Cards
: <!-- --------------------------------------------------- -->
  <!-- CARD: Tianji Cai                                    -->
  <!-- --------------------------------------------------- -->
  ![Photo of Tianji Cai]({{ '/images/tianji.JPG' | relative_url }})
  
  ### Tianji Cai
  <span class="person-role">Distinguished Researcher (Junior Faculty)</span>\\
  <span class="person-affiliation">School of Physical Science and Engineering, Tongji University</span>
  
  <!-- Tags -->
  - High Energy Theory
  - Particle Physics
  - Collider & Jet physics
  - AI for Science
  - Science for AI
  {:.person-tags}
  
  <!-- Bio -->  
  Tianji Cai (蔡恬吉) is a Distinguished Researcher (junior faculty) at Tongji University (Shanghai, CN). Before, she worked as a postdoctoral research associate in the Fundamental Physics Directorate at the SLAC National Accelerator Laboratory, and as a research affiliate at the Lawrence Berkeley National Laboratory. She obtained her Ph.D. degree in 2023 at University of California, Santa Barbara, and holds two bachelor's degrees from Duke University and Shanghai Jiao Tong University. Her research interest lies at the intersection of High Energy Theory (HEP) and Artificial Intelligence (AI), with the goal towards developing scientific AI. She is actively looking for interested students (undergrads & grads) to join her group, the Ψai Lab.
  {:.person-bio}
  <button class="bio-toggle">Read more</button>
  
  <!-- Email -->
  <span class="person-contact">
  Email: [tianjiresearch@gmail.com](mailto:tianjiresearch@gmail.com)
  </span>
  
: <!-- --------------------------------------------------- -->
  <!-- CARD: Sung Hak Lim                                    -->
  <!-- --------------------------------------------------- -->
  ![Photo of Sung Hak Lim]({{ '/images/sunghak.png' | relative_url }})

  ### Sung Hak Lim 
  <span class="person-role">Senior Researcher</span>\\
  <span class="person-affiliation">CTPU-PTC, Institute for Basic Science</span>
  
  <!-- Tags -->
  - Galactic Dynamics
  - Dark Matter Physics
  - Collider & Jet Physics
  - ML for Science
  {:.person-tags}
  
  <!-- Bio -->  
  Sung Hak Lim is a Senior Researcher at the Center for Theoretical Physics of the Universe (CTPU-PTC), Institute for Basic Science in South Korea. He earned his Ph.D. from KAIST in 2017, and worked in postdoctoral positions at KEK in Japan (2017-2020) and Rutgers University (2020-2024). His research focuses on combining physics principles with machine learning techniques to advance fundamental physics problems. His current primary work uses advanced neural network methods to map dark matter in the Milky Way and nearby dwarf galaxies. He also develops physics-inspired machine learning methods for identifying particle signals at large hadron colliders and studying dark matter halos of galaxies, with the ultimate goal of revealing the true nature of dark matter.
  {:.person-bio}
  <button class="bio-toggle">Read more</button>
  
  <!-- Email -->
  <span class="person-contact">
  Email: [sunghak.lim@ibs.re.kr](mailto:sunghak.lim@ibs.re.kr)
  </span>

: <!-- --------------------------------------------------- -->
  <!-- CARD: Vinicius Mikuni                              -->
  <!-- --------------------------------------------------- -->
  ![Photo of Vinicius Mikuni]({{ '/images/mikuni.jpg' | relative_url }}){:.person-photo--contain}
  
  ### Vinicius Mikuni
  <span class="person-role">Associate Professor</span>\\
  <span class="person-affiliation">Kobayashi-Maskawa Institute</span>
  
  <!-- Tags -->
  - AI for Science
  {:.person-tags}
  
  <!-- Bio -->  
  Vinicius Mikuni is an Associate Professor using AI for scientific discovery at the KMI Institute. He earned his PhD in 2021 from the University of Zurich, and worked as a Postdoctoral Fellow at Berkeley Lab, California. His research lies at the intersection of machine learning and fundamental science, where he develops algorithms to tackle core challenges in scientific research. His recent work includes fast simulation frameworks for fluid flows, collider physics, nuclear physics, and astrophysics using diffusion-based generative models; innovative methods for solving inverse problems in collider and neutrino physics; and leveraging pre-trained models to accelerate discoveries in particle physics.
  {:.person-bio}
  <button class="bio-toggle">Read more</button>
  
  <!-- Email -->
  <span class="person-contact">
  Email: [vmikuni@cern.ch](mailto:vmikuni@cern.ch)
  </span>

: <!-- --------------------------------------------------- -->
  <!-- CARD: Huilin Qu                                     -->
  <!-- --------------------------------------------------- -->
  ![Photo of Huilin Qu]({{ '/images/huilin.JPG' | relative_url }})
  
  ### Huilin Qu
  <span class="person-role">Staff Research Physicist</span>\\
  <span class="person-affiliation">CERN</span>
  
  <!-- Tags -->
  - Jet Tagging
  - Deep Learning
  - Collider Physics
  - AI Integration
  {:.person-tags}
  
  <!-- Bio -->  
  Dr. Huilin Qu (曲慧麟) is a staff research physicist at CERN. He received his B.S. degree from Peking University in 2014 and his Ph.D. from the University of California, Santa Barbara in 2019. His research is at the forefront of artificial intelligence and particle physics, where he has pioneered several innovative deep learning techniques for jet tagging—most notably ParticleNet—which has significantly improved performance and is now widely adopted at the LHC and beyond. As a member of the CMS experiment, Dr. Qu has contributed to searches for Higgs decays to charm quarks and Higgs boson pair production, earning the 2023 CMS Young Researcher Prize for advances in AI-based jet tagging and measurements.
  {:.person-bio}
  <button class="bio-toggle">Read more</button>
  
  <!-- Email -->
  <span class="person-contact">
  Email: [huilin.qu@cern.ch](mailto:huilin.qu@cern.ch)
  </span>

: <!-- --------------------------------------------------- -->
  <!-- CARD: Marco Meyer-Conde                             -->
  <!-- --------------------------------------------------- -->
  ![Photo of Marco Meyer-Conde]({{ '/images/marco.jpg' | relative_url }})
  
  ### Marco Meyer-Conde
  <span class="person-role">Assistant Research Professor</span>\\
  <span class="person-affiliation">Tokyo City University</span>
  
  <!-- Tags -->
  - AI for Science
  - Gravitational Waves
  - Future Colliders
  - Quantum Chromodynamics
  - Pion Phenomenology
  {:.person-tags}
  
  <!-- Bio -->  
  Marco Meyer is an Assistant Research Professor at Tokyo City University since 2024, specializing in machine learning for scientific applications and advanced signal processing techniques. He is a high-energy physics researcher by education with a focus on hadronic physics. He completed his Ph.D. at Université Paris-Saclay on the extraction of absolute Drell-Yan 2015 cross-sections using a 200 GeV negatively charged pion beam at COMPASS/AMBER (CERN), under a co-direction with CEA/Irfu/DPhN at Saclay and the University of Illinois Urbana-Champaign (USA), followed by a junior postdoctoral position at UIUC hosted at CERN. In 2021, he was awarded the JSPS-CNRS Overseas Fellowship, working as a senior postdoctoral fellow at Osaka Metropolitan University, where he worked on gravitational wave experiment physics, software & computing design, and machine learning applications for waveform forecasting. Marco is a member of the LIGO-VIRGO-KAGRA gravitational wave collaboration and the ePIC collaboration for Electron-Ion Collider physics. Outside of research, he enjoys blogging online, skiing, and bouldering.
  {:.person-bio}
  <button class="bio-toggle">Read more</button>
  
  <!-- Email -->
  <span class="person-contact">
  Email: [marco@tcu.ac.jp](mailto:marco@tcu.ac.jp)
  </span>

: <!-- --------------------------------------------------- -->
  <!-- CARD: Lingxiao Wang                                 -->
  <!-- --------------------------------------------------- -->
  ![Photo of Lingxiao Wang]({{ '/images/lingxiao.jpg' | relative_url }})
  
  ### Lingxiao Wang
  <span class="person-role">Deputy Director of AI as Science Team</span>\\
  <span class="person-affiliation">RIKEN Center for Interdisciplinary Theoretical and Mathematical Sciences (iTHEMS) / Institute for Physics of Intelligence, University of Tokyo</span>
  
  <!-- Tags -->
  - Machine Learning in Physics
  - Quantum Chromodynamics
  - Lattice Field Theory
  - AI for Science
  {:.person-tags}
  
  <!-- Bio -->  
  Lingxiao Wang (王凌霄) is a Research Scientist at RIKEN-iTHEMS (Wako, Japan), and concurrently holds an Assistant Professor at the Institute for Physics of Intelligence(iPI), UTokyo. Before his current positions, he completed his Ph.D. in Physics at Tsinghua University (China, 2015-2020) and spent time as a visiting Ph.D. student at the University of Tokyo (Japan, 2018-2019). During his post-doctoral research he worked at the Frankfurt Institute for Advanced Studies (FIAS) (Germany, 2020-2023). His research lies at the intersection of QCD physics, lattice field theory and deep learning. He focuses on using deep neural networks and generative AI to explore QCD matter, solve inverse problems in physics, and push the frontier of “AI for Science”. He is especially interested in bridging physics insights (symmetries, continuity, field theory) with modern machine-learning architectures, aiming to empower scientific discovery.
  {:.person-bio}
  <button class="bio-toggle">Read more</button>
  
  <!-- Email -->
  <span class="person-contact">
  Email: [lwang@fias.uni-frankfurt.de](mailto:lwang@fias.uni-frankfurt.de)
  </span>

: <!-- --------------------------------------------------- -->
  <!-- CARD: Ahmed Hammad                                  -->
  <!-- --------------------------------------------------- -->
  ![Photo of Ahmed Hammad]({{ '/images/hammad.jpg' | relative_url }}){:.person-photo--contain}
  
  ### Ahmed Hammad
  <span class="person-role">Postdoctoral Researcher</span>\\
  <span class="person-affiliation">Theory Center, High Energy Accelerator Research Organization (KEK), Japan</span>
  
  <!-- Tags -->
  - Beyond SM
  - Collider Phenomenology
  - Future Colliders
  - Jet Physics
  - AI for Science
  {:.person-tags}
  
  <!-- Bio -->  
  Ahmed Hammad is a Postdoctoral Researcher in the Theory Division at the High Energy Accelerator Research Organization (KEK, Tsukuba, Japan). He received his Ph.D. in Theoretical Physics in 2021 from the University of Basel (Switzerland). His research focuses on collider phenomenology and physics beyond the Standard Model, with a particular emphasis on applying advanced machine learning methods, both classical and quantum, to high energy physics. He has contributed to searches for new physics at the LHC and HL-LHC, with work spanning Higgs boson phenomenology, top quark flavor-changing neutral currents and anomaly detection techniques.
  {:.person-bio}
  <button class="bio-toggle">Read more</button>
  
  <!-- Email -->
  <span class="person-contact">
  Email: [hamed@post.kek.jp](mailto:hamed@post.kek.jp)
  </span>

</div>


International Advisory Committee
--------------------------------
Distinguished researchers worldwide providing guidance and support to our community.


<div class="block-advisory" markdown=1>

Advisory Committee
: ### Mihoko Nojiri
  <span class="advisory-position">Professor</span>\\
  <span class="advisory-affiliation">Tokyo City University</span>\\
  [Personal Website](http://www2.kek.jp/theory-center/theory_e/archives/member/nojiri-mihoko/)
  
: ### Satoshi Iso
  <span class="advisory-position">Professor</span>\\
  <span class="advisory-affiliation">RIKEN/KEK, Japan</span>\\
  [Personal Website](http://www2.kek.jp/theory-center/theory_e/archives/member/iso-satoshi/)
  
: ### Koji Hashimoto
  <span class="advisory-position">Professor</span>\\
  <span class="advisory-affiliation">Kyoto University, Japan</span>\\
  [Personal Website](https://www-gauge.scphys.kyoto-u.ac.jp/hashimoto/welcome.html){:target="_blank" rel="noopener"}

: ### Yanqing Ma
  <span class="advisory-position">Professor</span>\\
  <span class="advisory-affiliation">Peking University, China</span>\\
  [Personal Website](https://faculty.pku.edu.cn/yqma/en/index.htm){:target="_blank" rel="noopener"}

: ### David Shih
  <span class="advisory-position">Professor</span>\\
  <span class="advisory-affiliation">Rutgers University, USA</span>\\
  [Personal Website](https://sites.rutgers.edu/david-shih/){:target="_blank" rel="noopener"}

: ### Matthew R. Buckley
  <span class="advisory-position">Assistant Professor</span>\\
  <span class="advisory-affiliation">Rutgers University, USA</span>\\
  [Personal Website](http://www.physicsmatt.com/){:target="_blank" rel="noopener"}

: ### Gregor Kasieczka
  <span class="advisory-position">Professor</span>\\
  <span class="advisory-affiliation">University of Hamburg, Germany</span>\\
  [Personal Website](https://www.physik.uni-hamburg.de/en/iexp/gruppe-kasieczka.html){:target="_blank" rel="noopener"}

: ### Hua Xing Zhu
  <span class="advisory-position">Professor</span>\\
  <span class="advisory-affiliation">Peking University, China</span>\\
  [Personal Website](https://konformal.github.io){:target="_blank" rel="noopener"}

: ### Benjamin Nachman
  <span class="advisory-position">Associate Professor</span>\\
  <span class="advisory-affiliation">Stanford University/SLAC, USA</span>\\
  [Personal Website](https://nachmangroup.github.io/){:target="_blank" rel="noopener"}
</div>


Volunteers
----------
Community volunteers contribute to operations, events, outreach, and technical infrastructure.

<div class="block-organizers block-volunteers" markdown=1>

Volunteer Cards
: <!-- --------------------------------------------------- -->
  <!-- CARD: Shivasankar K.A                              -->
  <!-- --------------------------------------------------- -->
  ![Photo of Shivasankar K.A]({{ '/images/shiva.jpeg' | relative_url }}){:.person-photo--zoom-135}
  
  ### Shivasankar K.A
  <span class="person-role">Website Design & Admin</span>\\
  <span class="person-affiliation">PhD Student · Hokkaido University</span>
  
  <!-- Tags -->
  - Astroparticle
  - Theory
  - Deep Learning
  {:.person-tags}
  
  <!-- Bio -->  
  Shivasankar is a second-year Ph.D. student at Hokkaido University, Japan. His primary interests lie in theoretical astroparticle physics, where he studies Beyond Standard Model phenomena in astrophysical objects such as black holes, supernovae, and neutron stars, using theory and computation to explore how new physics could manifest. In parallel, he investigates AI-driven approaches in collider physics, specifically studying the physics learned by the models, and explores how concepts from fundamental physics might inspire new developments in AI. When he's not pondering black holes or neural networks, he enjoys learning new skills and exploring the endless possibilities simulated by the Cosmic++ code of the multiverse.
  {:.person-bio}
  <button class="bio-toggle">Read more</button>
  
  <!-- Email -->
  <span class="person-contact">
  Email: [a-shiva@particle.sci.hokudai.ac.jp](mailto:a-shiva@particle.sci.hokudai.ac.jp)
  </span>

</div>


Get Involved
------------

<div class="highlight-box" markdown=1>

### Join Our Community

Interested in contributing to our organizing efforts or participating in our activities? We welcome new members and collaborators who want to advance AI+HEP research and education in East Asia.

[Contact Us](https://groups.google.com/g/hep-aiea){:.btn}
[View events](/workshops/){:.btn .btn-outline}
{:.cta-center}

</div>
