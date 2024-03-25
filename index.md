---
layout: default
---

<div class="row">
  <div class="col-lg-8">
    <div class="card">
      <h1 class="card-title">About Me</h1>

      <p class="indent">
        <img 
          src="/assets/img/nutt.jpg"
          alt="RK"
          width="20%"
          height="auto"
          class="left_img"
          align="left"
        />

        I am a Ph.D. student in computational chemistry and machine learning at 
        <a href="https://www.luber-group.com/">Department of Chemistry, University of Zurich, Switzerland</a>.
        My current research relies on atomistic simulation with <i>ab initio</i> molecular dynamics (based on quantum chemistry) 
        and enhanced sampling techniques to calculate free energies of condensed phased systems.
        I am now interested in applying machine learning and graph theory to design new molecules and 
        investigate chemical reactions. My interest also extends to the development and improvement of open-source software 
        using cloud-based and full stack technology. 
        I am currently a member of <a href="https://www.lightchec.uzh.ch/">LightChEC</a> and 
        <a href="https://www.nccr-catalysis.ch/">NCCR Catalysis</a> advised by Prof. Sandra Luber.
      </p>

      <p class="indent">
        Before Zurich, I was a scientist at the <a href="https://newequilibriumbio.com/">New Equilibrium Biosciences</a> 
        (from 2019 to 2020) working on computational chemistry and machine learning for drug discovery.
        I helped the team design and set up AWS infrastructures for performing high-performance molecular dynamics 
        simulations and training neural network models for developing specific-purpose molecular force fields 
        for studying intrinsically disordered proteins (IDP) structures.
      </p>

      <p class="indent">
        In 2016 and 2019, I received Bachelor's and Master's degrees respectively from Thammasat University, Thailand, 
        where I focused on several research topics in computer modeling ranging from density functional theory to multiscale 
        (coarse-grained model) simulation under the supervision of Prof. Yuthana Tantirungrotechai.
        During my education at that time, I received the NCTU Taiwan Elite International Internship Scholarship 
        and worked at NCTU in the research group of Prof. Jen-Shiang K. Yu in 2015 and 2018, respectively. 
        In 2016, I was also a visiting student at ICTP, Trieste, Italy. In addition, I won the royal winner award of 
        <a href="https://www.facebook.com/TCC.ChallengeUBE/">Thailand Computational Chemistry Challenge (TCCC) 2016</a>. 
        For the competition, I used the dissipative particle dynamics technique to investigate the mechanical properties 
        of crosslinking-polyisoprene (natural rubber) reinforced by single-walled carbon nanotubes. 
      </p>
    </div>

    <div class="card">
      <h1 class="card-title">Resources</h1>
        <ul>
          <li>
            <a href="algo-sim-mol-book">Book: Algorithms for Computer Simulation of Molecular Systems (in Thai)</a>
          </li>
          <li>
            <a href="qm-summary-book">Book: Summary of Quantum Chemistry (in Thai)</a>
          </li>
          <li>
            <a href="ml-qm-book">Book: Machine Learning for Quantum Chemistry (in Thai)</a>
          </li>
          <li>
            <a href="elec-struct">Slide: Computational Chemistry: Electronic Structure Calculation</a>
          </li>
          <li>
            <a href="moldyn">Note: Based-on-experiences Note on Statistical Molecular Dynamics for Soft Matter Simulations</a>
          </li>
        </ul>
    </div>

    <div class="card">
      <h1 class="card-title">Contributions</h1>
      <ul>
        <li>
          <a href="https://gdsc.community.dev/eth-zurich/">Google Developer Student Clubs (GDSC) Zurich</a>
        </li>
        <li>
          Thailand Machine Learning for Chemistry Competition 2021 (see <a href="https://competitions.codalab.org/competitions/34540">this</a> and <a href="https://tmlcc2021.devpost.com/">this</a>)
        </li>
        <li>
          HackZurich, 2020, <a href="https://devpost.com/software/mygarden">2021</a>, <a href="https://github.com/rangsimanketkaew/hackzurich2022-emotion">2022</a>
        </li>
        <li>
          <a href="https://github.com/JeanBaptiste-dlb/Skiptify">BaselHack 2022</a>
        </li>
        <li>
          PyCon 2019 & 2021
        </li>
        <li>
          <a href="https://www.kaggle.com/c/champs-scalar-coupling">Kaggle's Predicting Molecular Properties 2019</a>
        </li> 
      </ul>
    </div>

    <div class="card">
      <h1 class="card-title">Publications</h1>
        <ol>
        {% for paper in site.data.publications %}
          <li>
           {{ paper.title }}. <br>
           {{ paper.authors }}. 
           <a href="https://doi.org/{{ paper.link }}"
            >DOI: {{ paper.link }}</a
          >
          </li>
        {% endfor %}
        </ol>
    </div>
  </div>

  <div class="col-lg-4">
    <div class="card">
      <h1>Contact</h1>
      <h6><i class="fas fa-map-marker-alt"></i> {{ site.author_location }}</h6>
      <h6><i class="fas fa-envelope"></i> {{ site.author_email_uzh }}</h6>
      <h6><i class="fas fa-envelope"></i> {{ site.author_email }}</h6>
      <h6><i class="fas fa-phone"></i> {{ site.author_phone }}</h6>
      <h6><i class="fas fa-link"></i> {{ site.author_website_url }}</h6>
    </div>

    <div class="card">
      <h1>CV</h1>
      <p>My academic <a href="/cv.pdf" target="_blank">CV</a> and <a href="/resume.pdf" target="_blank">resume</a>.</p>
      <br>
      <p>My tech <a href="/cv-tech.pdf" target="_blank">CV</a> and <a href="/resume-tech.pdf" target="_blank">resume</a>.</p>
    </div>

    <div class="card">
      <h1>Skills</h1>
      <p>Bash, Python, C++, Fortran, LaTeX</p>
      <p>Unix/Linux, AWS Cloud and system administration, Git, Vi(m)</p>
      <p>Machine (Deep) learning, Sci-kit learn, TensorFlow </p>
      <p>Parallel/distributed computing, distributed system</p>
      <p>Computational chemistry software benchmarking</p>
    </div>

    <div class="card">
      <h1>Space</h1>
      <ul>
        <li><p><a href="https://github.com/rangsimanketkaew">https://github.com/rangsimanketkaew</a></p></li>
        <li><p><a href="https://scholar.google.com/citations?user=3wOKfJAAAAAJ&hl=en">Google Scholar</a></p></li>
      </ul>
    </div>

    <div class="card">
      <h1 class="card-title">Projects</h1>
      <ul>
        <li>
          <a href="https://github.com/rangsimanketkaew/skull-king">Skull King</a>
        </li>
        <li>
          <a href="https://github.com/rangsimanketkaew//ET-NWChem">ET-NWChem</a>
        </li>
        <li>
          <a href="https://github.com/rangsimanketkaew/QM-on-TAIWANIA">QM-on-TAIWANIA</a>
        </li>
        <li>
          <a href="https://octadist.github.io/">OctaDist</a>
        </li>
        <li>
          <a href="https://github.com/moleview/moleview">MoleView</a>
        </li>
        <li>
          <a href="https://github.com/rangsimanketkaew/tv_counting">tv_counting</a>
        </li>
        <li>
          <a href="https://sites.google.com/site/rangsiman1993/">Google Site Blog</a>
        </li>
      </ul>
    </div>

    <div class="card">
      <h1>Cabinet</h1>
      <h4>Favorite books</h4>
      <ul>
        <li><h6>
        <a 
          href="http://www.scielo.br/pdf/bjp/v36n4a/a35v364a.pdf" 
          target="_blank">
          A Bird’s-Eye View of Density-Functional Theory
        </a>
        </h6></li>

        <li><h6>
        <a 
          href="https://www.amazon.com/Statistical-Mechanics-Donald-Allan-McQuarrie/dp/1891389157" 
          target="_blank">
          Statistical Mechanics by Donald A. McQuarrie
        </a>
        </h6>
        </li>
      </ul>
      <h4>Favorite articles</h4>
      <ul>
        <li><h6><a href="https://docs.oracle.com/cd/E19957-01/800-7895/800-7895.pdf" target="_blank">What Every Computer Scientist Should Know About Floating-Point Arithmetic</a></h6></li>
        <li><h6><a href="https://www.moreisdifferent.com/2015/07/16/why-physicsts-still-use-fortran/" target="_blank">Why physicists still use Fortran</a></h6></li>
      </ul>
      <h4>Favorite discussions</h4>
      <ul>
        <li><h6><a href="https://stackoverflow.com/questions/101268/hidden-features-of-python" target="_blank">Hidden features of Python</a></h6></li>
        <li><h6><a href="https://scicomp.stackexchange.com/questions/3159/is-it-a-good-idea-to-use-vectorvectordouble-to-form-a-matrix-class-for-high" target="_blank">Is it a good idea to use vector&lt;vector&lt;double&gt;&gt; to form a matrix class for high performance scientific computing code?</a></h6></li>
      </ul>
    </div>
  </div>
</div>
