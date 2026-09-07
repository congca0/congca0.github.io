---
permalink: /about/
title: "About"
author_profile: true
---

## My Journey

---
title: "About"
permalink: /about/
---

<style>
/* =========================================================
   Interactive Academic Journey Timeline
   ========================================================= */

.journey {
  width: 100%;
  max-width: 1200px;
  margin: 20px auto 60px;
  font-family:
    -apple-system,
    BlinkMacSystemFont,
    "Segoe UI",
    Roboto,
    Helvetica,
    Arial,
    sans-serif;
}

/* ---------------------------------------------------------
   Timeline
   --------------------------------------------------------- */

.timeline-wrapper {
  width: 100%;
  overflow-x: auto;
  overflow-y: hidden;
  padding: 25px 0 15px;
  -webkit-overflow-scrolling: touch;
}

.timeline {
  position: relative;
  min-width: 1080px;
  padding: 0 35px;
  display: flex;
  justify-content: space-between;
}

/* Base line */
.timeline::before {
  content: "";
  position: absolute;
  left: 60px;
  right: 60px;
  top: 112px;
  height: 4px;
  background: #b8c7da;
  border-radius: 4px;
}

/* Active progress */
.timeline-progress {
  position: absolute;
  left: 60px;
  top: 112px;
  width: 0;
  height: 4px;
  background: #3278c8;
  border-radius: 4px;
  transition: width 0.45s ease;
  z-index: 1;
}

/* ---------------------------------------------------------
   Timeline item
   --------------------------------------------------------- */

.timeline-item {
  position: relative;
  width: 120px;
  flex-shrink: 0;
  text-align: center;
  cursor: pointer;
  z-index: 3;
}

.timeline-label {
  height: 78px;
}

.timeline-place {
  font-size: 17px;
  line-height: 1.25;
  font-weight: 700;
  color: #193b67;
  white-space: nowrap;
}

.timeline-field {
  margin-top: 7px;
  font-size: 14px;
  line-height: 1.25;
  color: #3e73b7;
}

/* Node */
.timeline-dot {
  position: relative;
  width: 18px;
  height: 18px;
  margin: 25px auto 0;

  background: #b8c7da;
  border: 4px solid #f8fbff;
  border-radius: 50%;

  box-shadow: 0 0 0 2px #b8c7da;

  transition:
    transform 0.25s ease,
    background 0.25s ease,
    box-shadow 0.25s ease;
}

/* Hover */
.timeline-item:hover .timeline-dot {
  transform: scale(1.15);
  background: #6c9ed3;
  box-shadow: 0 0 0 3px #6c9ed3;
}

/* Active */
.timeline-item.active .timeline-dot {
  transform: scale(1.2);
  background: #2878d4;
  box-shadow:
    0 0 0 4px #2878d4,
    0 0 22px rgba(40, 120, 212, 0.35);
}

.timeline-item.active .timeline-place {
  color: #0e56a3;
}

.timeline-item.active .timeline-field {
  color: #2878d4;
}


/* ---------------------------------------------------------
   Detail card
   --------------------------------------------------------- */

.journey-card {
  margin: 38px 35px 0;
  padding: 30px 38px;

  min-height: 135px;

  background:
    linear-gradient(
      135deg,
      #f1f7fd 0%,
      #ffffff 100%
    );

  border: 1px solid #cbdced;
  border-radius: 20px;

  box-shadow:
    0 8px 28px rgba(35, 70, 105, 0.08);

  transition:
    opacity 0.2s ease,
    transform 0.2s ease;
}

.journey-card.fade {
  opacity: 0;
  transform: translateY(6px);
}

.journey-title {
  margin: 0;
  color: #193b67;
  font-size: 27px;
  line-height: 1.25;
  font-weight: 700;
}

.journey-field {
  margin-top: 8px;
  color: #3278c8;
  font-size: 17px;
  line-height: 1.4;
}

.journey-description {
  margin-top: 16px;
  margin-bottom: 0;

  color: #526b88;
  font-size: 16px;
  line-height: 1.7;
}


/* ---------------------------------------------------------
   Hint
   --------------------------------------------------------- */

.journey-hint {
  margin-top: 14px;
  text-align: center;

  color: #8799ae;
  font-size: 13px;
}


/* ---------------------------------------------------------
   Mobile
   --------------------------------------------------------- */

@media (max-width: 700px) {

  .timeline-wrapper {
    margin-left: -10px;
    margin-right: -10px;
    width: calc(100% + 20px);
  }

  .journey-card {
    margin-left: 15px;
    margin-right: 15px;
    padding: 25px;
  }

  .journey-title {
    font-size: 24px;
  }

  .journey-description {
    font-size: 15px;
  }
}
</style>


<div class="journey">

  <div class="timeline-wrapper">

    <div class="timeline" id="academicTimeline">

      <div
        class="timeline-progress"
        id="timelineProgress">
      </div>


      <!-- =================================================
           1. China
           ================================================= -->

      <div
        class="timeline-item active"
        data-title="China"
        data-field="Environment"
        data-description="Grew up in Shanxi Province, one of China’s major coal-producing regions, where I became interested in environmental health and the relationship between environmental exposures and human health."
      >

        <div class="timeline-label">
          <div class="timeline-place">
            China
          </div>

          <div class="timeline-field">
            Environment
          </div>
        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- =================================================
           2. MedTech
           ================================================= -->

      <div
        class="timeline-item"
        data-title="MedTech"
        data-field="Healthcare"
        data-description="I trained in pharmaceutical engineering and later worked in the medical technology industry, collaborating with physicians and software engineers on healthcare information systems."
      >

        <div class="timeline-label">
          <div class="timeline-place">
            MedTech
          </div>

          <div class="timeline-field">
            Healthcare
          </div>
        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- =================================================
           3. Helmholtz Centre
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Helmholtz Centre"
        data-field="Biomedical Data"
        data-description="At the Helmholtz Centre for Infection Research in Germany, I worked with mass spectrometry data and machine learning to study biomedical and virological questions."
      >

        <div class="timeline-label">
          <div class="timeline-place">
            Helmholtz Centre
          </div>

          <div class="timeline-field">
            Biomedical Data
          </div>
        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- =================================================
           4. Göttingen
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Göttingen"
        data-field="Genomics"
        data-description="At the University of Göttingen, I worked with mRNA sequencing and single-cell transcriptomic data, developing a foundation in computational genomics and biomedical data science."
      >

        <div class="timeline-label">
          <div class="timeline-place">
            Göttingen
          </div>

          <div class="timeline-field">
            Genomics
          </div>
        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- =================================================
           5. NTNU
           ================================================= -->

      <div
        class="timeline-item"
        data-title="NTNU, Norway"
        data-field="Economics + ML"
        data-description="During my Ph.D. in Economics, with a focus on machine learning, I studied nonlinear and delayed relationships between air pollution, weather, and cardiovascular health using nationwide data from Norway."
      >

        <div class="timeline-label">
          <div class="timeline-place">
            NTNU, Norway
          </div>

          <div class="timeline-field">
            Economics + ML
          </div>
        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- =================================================
           6. Caltech
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Caltech"
        data-field="Physics-Based Deep Learning"
        data-description="At Caltech, I expanded my research across environmental exposures, aging, epigenetics, and postoperative outcomes, while collaborating with clinicians, epidemiologists, and biomedical scientists."
      >

        <div class="timeline-label">
          <div class="timeline-place">
            Caltech
          </div>

          <div class="timeline-field">
            Physics-Based Deep Learning
          </div>
        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- =================================================
           7. Yale
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Yale"
        data-field="Causal AI"
        data-description="At Yale, I moved more directly into causal AI for health research, studying treatment effects using large-scale observational and clinical trial data."
      >

        <div class="timeline-label">
          <div class="timeline-place">
            Yale
          </div>

          <div class="timeline-field">
            Causal AI
          </div>
        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- =================================================
           8. Stanford
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Stanford"
        data-field="Precision Medicine"
        data-description="At Stanford, I work on AI for precision medicine, developing quantitative approaches to understand variation in health and treatment outcomes and to support more informed treatment decisions."
      >

        <div class="timeline-label">
          <div class="timeline-place">
            Stanford
          </div>

          <div class="timeline-field">
            Precision Medicine
          </div>
        </div>

        <div class="timeline-dot"></div>

      </div>

    </div>
  </div>


  <!-- =====================================================
       Dynamic information card
       ===================================================== -->

  <div
    class="journey-card"
    id="journeyCard"
  >

    <h3
      class="journey-title"
      id="journeyTitle"
    >
      China
    </h3>

    <div
      class="journey-field"
      id="journeyField"
    >
      Environment
    </div>

    <p
      class="journey-description"
      id="journeyDescription"
    >
      Grew up in Shanxi Province, one of China’s major
      coal-producing regions, where I became interested in
      environmental health and the relationship between
      environmental exposures and human health.
    </p>

  </div>


  <div class="journey-hint">
    Click a stage to explore my research journey.
  </div>

</div>


<script>
(function () {

  const items =
    document.querySelectorAll(".timeline-item");

  const card =
    document.getElementById("journeyCard");

  const title =
    document.getElementById("journeyTitle");

  const field =
    document.getElementById("journeyField");

  const description =
    document.getElementById("journeyDescription");

  const progress =
    document.getElementById("timelineProgress");


  function updateJourney(item, index) {

    /* Fade out */
    card.classList.add("fade");


    setTimeout(function () {

      title.textContent =
        item.dataset.title;

      field.textContent =
        item.dataset.field;

      description.textContent =
        item.dataset.description;


      /* Fade in */
      card.classList.remove("fade");

    }, 150);


    /* Active node */

    items.forEach(function (element) {
      element.classList.remove("active");
    });

    item.classList.add("active");


    /* Progress line */

    const percentage =
      (index / (items.length - 1)) * 100;

    progress.style.width =
      percentage + "%";


    /* Keep selected node visible on mobile */

    if (window.innerWidth < 700) {

      item.scrollIntoView({
        behavior: "smooth",
        inline: "center",
        block: "nearest"
      });

    }

  }


  /* Click events */

  items.forEach(function (item, index) {

    item.addEventListener(
      "click",
      function () {
        updateJourney(item, index);
      }
    );

  });


  /* Initial state */

  updateJourney(items[0], 0);

})();
</script>

From environmental health to precision health at Stanford, my research journey has crossed pharmaceutical engineering, healthcare technology, biomedical science, economics, and AI.


