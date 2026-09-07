 ---
title: "About"
permalink: /about/
---

<style>

/* =========================================================
   ABOUT — INTERACTIVE ACADEMIC JOURNEY
   ========================================================= */

.journey {
  width: 100%;
  max-width: 1200px;
  margin: 10px auto 60px;
  font-family:
    -apple-system,
    BlinkMacSystemFont,
    "Segoe UI",
    Roboto,
    Helvetica,
    Arial,
    sans-serif;
}


/* =========================================================
   INTRO
   ========================================================= */

.journey-intro {
  max-width: 900px;
  margin: 0 auto 45px;
  text-align: left;
}

.journey-intro h2 {
  margin-bottom: 14px;
  color: #193b67;
  font-size: 30px;
  font-weight: 700;
}

.journey-intro p {
  margin: 0;
  color: #526b88;
  font-size: 17px;
  line-height: 1.75;
}


/* =========================================================
   TIMELINE WRAPPER
   ========================================================= */

.timeline-wrapper {
  width: 100%;
  overflow-x: auto;
  overflow-y: visible;
  padding: 35px 0 15px;
  -webkit-overflow-scrolling: touch;
  scrollbar-width: thin;
}


/* =========================================================
   TIMELINE
   ========================================================= */

.timeline {
  position: relative;

  min-width: 1120px;

  padding: 0 35px;

  display: flex;
  justify-content: space-between;
}


/* Base horizontal line */

.timeline::before {
  content: "";

  position: absolute;

  left: 60px;
  right: 60px;

  top: 125px;

  height: 4px;

  background: #b9c9dc;

  border-radius: 10px;
}


/* Blue progress line */

.timeline-progress {
  position: absolute;

  left: 60px;

  top: 125px;

  width: 0;

  height: 4px;

  background: linear-gradient(
    90deg,
    #4d8fd8,
    #2878d4
  );

  border-radius: 10px;

  transition:
    width 0.55s cubic-bezier(
      0.22,
      1,
      0.36,
      1
    );

  z-index: 1;
}


/* =========================================================
   TIMELINE ITEM
   ========================================================= */

.timeline-item {

  position: relative;

  width: 120px;

  flex-shrink: 0;

  text-align: center;

  cursor: pointer;

  z-index: 3;

}


/* =========================================================
   CLICK HERE LABEL
   ========================================================= */

.click-here {

  display: inline-block;

  margin-bottom: 9px;

  padding: 4px 10px;

  border-radius: 20px;

  background: #edf5ff;

  border: 1px solid #c7ddf5;

  color: #2878d4;

  font-size: 11px;

  font-weight: 600;

  letter-spacing: 0.2px;

  opacity: 0.72;

  transform: translateY(0);

  transition:
    all 0.25s ease;

  animation:
    clickPulse 2.4s ease-in-out infinite;
}


/* Slightly different animation timing
   for each node */

.timeline-item:nth-child(3) .click-here {
  animation-delay: 0.2s;
}

.timeline-item:nth-child(4) .click-here {
  animation-delay: 0.4s;
}

.timeline-item:nth-child(5) .click-here {
  animation-delay: 0.6s;
}

.timeline-item:nth-child(6) .click-here {
  animation-delay: 0.8s;
}

.timeline-item:nth-child(7) .click-here {
  animation-delay: 1s;
}

.timeline-item:nth-child(8) .click-here {
  animation-delay: 1.2s;
}

.timeline-item:nth-child(9) .click-here {
  animation-delay: 1.4s;
}


/* Hover */

.timeline-item:hover .click-here {

  background: #2878d4;

  border-color: #2878d4;

  color: #ffffff;

  opacity: 1;

  transform:
    translateY(-3px)
    scale(1.05);

  box-shadow:
    0 5px 14px
    rgba(40, 120, 212, 0.22);

  animation: none;
}


/* Active */

.timeline-item.active .click-here {

  background: #2878d4;

  border-color: #2878d4;

  color: #ffffff;

  opacity: 1;

  box-shadow:
    0 5px 16px
    rgba(40, 120, 212, 0.24);

  animation: none;
}


/* Click animation */

@keyframes clickPulse {

  0%,
  100% {
    opacity: 0.62;
    transform: translateY(0);
  }

  50% {
    opacity: 1;
    transform: translateY(-2px);
  }

}


/* =========================================================
   PLACE + FIELD
   ========================================================= */

.timeline-label {

  height: 58px;

}


.timeline-place {

  color: #193b67;

  font-size: 17px;

  font-weight: 700;

  line-height: 1.25;

  white-space: nowrap;

}


.timeline-field {

  margin-top: 6px;

  color: #3e73b7;

  font-size: 13px;

  line-height: 1.3;

}


/* Active text */

.timeline-item.active .timeline-place {

  color: #0e56a3;

}


.timeline-item.active .timeline-field {

  color: #2878d4;

}


/* =========================================================
   DOT
   ========================================================= */

.timeline-dot {

  position: relative;

  width: 18px;

  height: 18px;

  margin: 25px auto 0;

  background: #b8c7da;

  border: 4px solid #f8fbff;

  border-radius: 50%;

  box-shadow:
    0 0 0 2px #b8c7da;

  transition:
    all 0.3s ease;

}


/* Hover */

.timeline-item:hover .timeline-dot {

  background: #6b9ed5;

  box-shadow:
    0 0 0 3px #6b9ed5;

  transform: scale(1.15);

}


/* Active */

.timeline-item.active .timeline-dot {

  background: #2878d4;

  box-shadow:
    0 0 0 4px #2878d4,
    0 0 22px
    rgba(40, 120, 212, 0.35);

  transform: scale(1.2);

}


/* =========================================================
   INFORMATION CARD
   ========================================================= */

.journey-card {

  margin: 40px 35px 0;

  padding: 30px 38px;

  min-height: 145px;

  background:
    linear-gradient(
      135deg,
      #f1f7fd 0%,
      #ffffff 100%
    );

  border: 1px solid #cbdced;

  border-radius: 20px;

  box-shadow:
    0 8px 28px
    rgba(35, 70, 105, 0.08);

  transition:
    opacity 0.2s ease,
    transform 0.2s ease;

}


.journey-card.fade {

  opacity: 0;

  transform:
    translateY(8px);

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

  font-weight: 500;

}


.journey-description {

  margin-top: 15px;

  margin-bottom: 0;

  color: #526b88;

  font-size: 16px;

  line-height: 1.7;

}


/* =========================================================
   MOBILE
   ========================================================= */

@media (max-width: 700px) {

  .journey {
    margin-left: -10px;
    margin-right: -10px;
  }

  .journey-intro {
    padding: 0 15px;
  }

  .journey-intro h2 {
    font-size: 27px;
  }

  .journey-intro p {
    font-size: 16px;
  }

  .timeline-wrapper {
    width: calc(100% + 20px);
    margin-left: -10px;
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


  <!-- =====================================================
       INTRO
       ===================================================== -->

  <div class="journey-intro">

    <h2>My Journey</h2>

    <p>
     A common theme runs through my work: understanding why health outcomes differ across people, environments, and treatments, and developing quantitative methods to better understand and address these differences. My work has taken me across environmental health, biomedical science, economics, machine learning, population health, and causal AI, and now focuses on precision medicine.
    </p>

  </div>



  <!-- =====================================================
       TIMELINE
       ===================================================== -->

  <div class="timeline-wrapper">

    <div
      class="timeline"
      id="academicTimeline"
    >


      <!-- Progress -->

      <div
        class="timeline-progress"
        id="timelineProgress"
      ></div>



      <!-- =================================================
           CHINA
           ================================================= -->

      <div
        class="timeline-item active"
        data-title="China"
        data-field="Environment"
        data-description="Grew up in one of China’s major coal-producing regions, where I became interested in the relationship between environmental exposures and human health."
      >

        <div class="click-here">
          Click here
        </div>

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
           MEDTECH
           ================================================= -->

      <div
        class="timeline-item"
        data-title="MedTech"
        data-field="Healthcare"
        data-description="I trained in pharmaceutical engineering and later worked in the medical technology industry, collaborating with physicians and software engineers on healthcare information systems."
      >

        <div class="click-here">
          Click here
        </div>

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
           HELMHOLTZ
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Helmholtz Centre"
        data-field="Biomedical Data"
        data-description="At the Helmholtz Centre for Infection Research in Germany, I applied machine learning to mass spectrometry data to study molecular signatures of viral infection."
      >

        <div class="click-here">
          Click here
        </div>

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
           GÖTTINGEN
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Göttingen"
        data-field="Genomics"
        data-description="At the University of Göttingen, I worked with mRNA sequencing and single-cell transcriptomic data, developing a foundation in computational genomics and biomedical data science."
      >

        <div class="click-here">
          Click here
        </div>

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
           NTNU
           ================================================= -->

      <div
        class="timeline-item"
        data-title="NTNU, Norway"
        data-field="Economics + ML"
        data-description="During my Ph.D., I studied nonlinear and delayed relationships between air pollution, weather, and cardiovascular health using nationwide data from Norway."
      >

        <div class="click-here">
          Click here
        </div>

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
           CALTECH
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Caltech"
        data-field="Physics-Based Deep Learning"
        data-description="At Caltech, I expanded my research across environmental exposures, aging, epigenetics, and postoperative outcomes, while collaborating with clinicians, epidemiologists, and biomedical scientists."
      >

        <div class="click-here">
          Click here
        </div>

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
           YALE
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Yale"
        data-field="Causal AI"
        data-description=" At Yale and VA, I moved more directly into causal AI for health research, studying treatment effects using large-scale observational and clinical trial data."
      >

        <div class="click-here">
          Click here
        </div>

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
           STANFORD
           ================================================= -->

      <div
        class="timeline-item"
        data-title="Stanford"
        data-field="Precision Medicine"
        data-description="At Stanford, I work on AI for precision medicine, developing quantitative methods to understand variation in treatment effects and support personalized treatment decisions."
      >

        <div class="click-here">
          Click here
        </div>

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
       DYNAMIC INFORMATION CARD
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
     Grew up in one of China’s major coal-producing regions, where I became interested in the relationship between environmental exposures and human health.
    </p>

  </div>


</div>



<script>

(function () {

  const items =
    document.querySelectorAll(
      ".timeline-item"
    );

  const card =
    document.getElementById(
      "journeyCard"
    );

  const title =
    document.getElementById(
      "journeyTitle"
    );

  const field =
    document.getElementById(
      "journeyField"
    );

  const description =
    document.getElementById(
      "journeyDescription"
    );

  const progress =
    document.getElementById(
      "timelineProgress"
    );


  /* =======================================================
     UPDATE TIMELINE
     ======================================================= */

  function updateJourney(
    item,
    index
  ) {

    /* Fade card out */

    card.classList.add(
      "fade"
    );


    setTimeout(
      function () {

        title.textContent =
          item.dataset.title;

        field.textContent =
          item.dataset.field;

        description.textContent =
          item.dataset.description;


        /* Fade card back in */

        card.classList.remove(
          "fade"
        );

      },
      150
    );


    /* =====================================================
       ACTIVE NODE
       ===================================================== */

    items.forEach(
      function (element) {

        element.classList.remove(
          "active"
        );

      }
    );


    item.classList.add(
      "active"
    );


    /* =====================================================
       PROGRESS LINE
       ===================================================== */

    const percentage =
      (index /
        (items.length - 1))
      * 100;


    progress.style.width =
      percentage + "%";


    /* =====================================================
       MOBILE SCROLL
       ===================================================== */

    if (
      window.innerWidth < 700
    ) {

      item.scrollIntoView({

        behavior: "smooth",

        inline: "center",

        block: "nearest"

      });

    }

  }


  /* =======================================================
     CLICK EVENTS
     ======================================================= */

  items.forEach(
    function (
      item,
      index
    ) {

      item.addEventListener(
        "click",
        function () {

          updateJourney(
            item,
            index
          );

        }
      );

    }
  );


  /* =======================================================
     INITIAL STATE
     ======================================================= */

  updateJourney(
    items[0],
    0
  );

})();

</script>
