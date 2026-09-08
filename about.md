 ---
layout: page
title: ""
permalink: /about/
---

<style>

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

.journey-intro {
  max-width: 900px;
  margin: 0 auto 45px;
  text-align: left;
}

.journey-intro h2 {
  margin-bottom: 14px;
  color: #8C1515;
  font-size: 30px;
  font-weight: 700;
}

.journey-intro p {
  margin: 0;
  color: #4F4F4F;
  font-size: 17px;
  line-height: 1.75;
}

.timeline-wrapper {
  width: 100%;
  overflow-x: auto;
  overflow-y: visible;
  padding: 35px 0 15px;
  -webkit-overflow-scrolling: touch;
  scrollbar-width: thin;
}

.timeline {
  position: relative;
  min-width: 1120px;
  padding: 0 35px;
  display: flex;
  justify-content: space-between;
}

.timeline::before {
  content: "";
  position: absolute;
  left: 60px;
  right: 60px;
  top: 125px;
  height: 4px;
  background: #D8B4B4;
  border-radius: 10px;
}

.timeline-progress {
  position: absolute;
  left: 60px;
  top: 125px;
  width: 0;
  height: 4px;
  background: #8C1515;
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

.timeline-item {
  position: relative;
  width: 120px;
  flex-shrink: 0;
  text-align: center;
  cursor: pointer;
  z-index: 3;
}

.click-here {
  display: inline-block;
  margin-bottom: 9px;
  padding: 4px 10px;
  border-radius: 20px;
  background: #F9EEEE;
  border: 1px solid #E6C7C7;
  color: #8C1515;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.2px;
  opacity: 0.72;
  transform: translateY(0);
  transition: all 0.25s ease;
  animation: clickPulse 2.4s ease-in-out infinite;
}

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

.timeline-item:hover .click-here {
  background: #8C1515;
  border-color: #8C1515;
  color: #ffffff;
  opacity: 1;
  transform: translateY(-3px) scale(1.05);
  box-shadow:
    0 5px 14px
    rgba(140, 21, 21, 0.20);
  animation: none;
}

.timeline-item.active .click-here {
  background: #8C1515;
  border-color: #8C1515;
  color: #ffffff;
  opacity: 1;
  box-shadow:
    0 5px 16px
    rgba(140, 21, 21, 0.22);
  animation: none;
}

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

.timeline-label {
  height: 58px;
}

.timeline-place {
  color: #333333;
  font-size: 17px;
  font-weight: 700;
  line-height: 1.25;
  white-space: nowrap;
}

.timeline-field {
  margin-top: 6px;
  color: #777777;
  font-size: 13px;
  line-height: 1.3;
}

.timeline-item.active .timeline-place {
  color: #8C1515;
}

.timeline-item.active .timeline-field {
  color: #8C1515;
}

.timeline-dot {
  position: relative;
  width: 18px;
  height: 18px;
  margin: 25px auto 0;
  background: #C9A3A3;
  border: 4px solid #ffffff;
  border-radius: 50%;
  box-shadow:
    0 0 0 2px #C9A3A3;
  transition: all 0.3s ease;
}

.timeline-item:hover .timeline-dot {
  background: #A85C5C;
  box-shadow:
    0 0 0 3px #A85C5C;
  transform: scale(1.15);
}

.timeline-item.active .timeline-dot {
  background: #8C1515;
  box-shadow:
    0 0 0 4px #8C1515,
    0 0 22px
    rgba(140, 21, 21, 0.28);
  transform: scale(1.2);
}

.journey-card {
  margin: 40px 35px 0;
  padding: 30px 38px;
  min-height: 145px;
  background:
    linear-gradient(
      135deg,
      #FBF5F5 0%,
      #ffffff 100%
    );
  border: 1px solid #E1CACA;
  border-radius: 20px;
  box-shadow:
    0 8px 28px
    rgba(80, 40, 40, 0.07);
  transition:
    opacity 0.2s ease,
    transform 0.2s ease;
}

.journey-card.fade {
  opacity: 0;
  transform: translateY(8px);
}

.journey-title {
  margin: 0;
  color: #8C1515;
  font-size: 27px;
  line-height: 1.25;
  font-weight: 700;
}

.journey-field {
  margin-top: 8px;
  color: #8C1515;
  font-size: 17px;
  line-height: 1.4;
  font-weight: 500;
}

.journey-description {
  margin-top: 15px;
  margin-bottom: 0;
  color: #4F4F4F;
  font-size: 16px;
  line-height: 1.7;
}

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

  <div class="journey-intro">

    <h2>My Journey</h2>

    <p>
      My work focuses on understanding why health outcomes and treatment responses differ across people. Over time, I have worked across healthcare, environmental health, economics, machine learning, genomics, and biostatistics. These experiences have led me to my current work in Mechanism-Informed Causal AI for Precision Medicine.
    </p>

  </div>


  <div class="timeline-wrapper">

    <div
      class="timeline"
      id="academicTimeline"
    >

      <div
        class="timeline-progress"
        id="timelineProgress"
      ></div>


      <!-- CHINA -->

      <div
        class="timeline-item"
        data-title="China"
        data-field="Environment"
        data-description="Growing up in Shanxi, a major coal-producing region in China, first led me to think about how environmental conditions can affect human health."
      >

        <div class="click-here">
          Research highlights
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


      <!-- MEDTECH -->

      <div
        class="timeline-item"
        data-title="MedTech"
        data-field="Healthcare"
        data-description="I trained in pharmaceutical engineering and later worked in healthcare technology, developing clinical information systems and working with clinicians on operating room workflow."
      >

        <div class="click-here">
          Research highlights
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


      <!-- HELMHOLTZ -->

      <div
        class="timeline-item"
        data-title="Helmholtz Centre"
        data-field="Machine Learning"
        data-description="At the Helmholtz Centre for Infection Research in Germany, I began applying machine learning to biomedical and epidemiological data."
      >

        <div class="click-here">
          Research highlights
        </div>

        <div class="timeline-label">

          <div class="timeline-place">
            Helmholtz Centre
          </div>

          <div class="timeline-field">
            Machine Learning
          </div>

        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- GÖTTINGEN -->

      <div
        class="timeline-item"
        data-title="Göttingen"
        data-field="Genomics"
        data-description="At the University of Göttingen, I worked with sequencing and transcriptomic data, developing a foundation in bioinformatics and computational genomics."
      >

        <div class="click-here">
          Research highlights
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


      <!-- NTNU -->

      <div
        class="timeline-item"
        data-title="NTNU, Norway"
        data-field="Economics + ML"
        data-description="During my Ph.D., I combined economics, machine learning, and causal methods to study environmental exposures, transportation, and population health."
      >

        <div class="click-here">
          Research highlights
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


      <!-- CALTECH -->

      <div
        class="timeline-item"
        data-title="Caltech"
        data-field="Physics-Based ML"
        data-description="At Caltech, I explored how scientific knowledge and physical principles can be incorporated into machine learning, with applications in environmental health and population health."
      >

        <div class="click-here">
          Research highlights
        </div>

        <div class="timeline-label">

          <div class="timeline-place">
            Caltech
          </div>

          <div class="timeline-field">
            Physics-Based ML
          </div>

        </div>

        <div class="timeline-dot"></div>

      </div>


      <!-- YALE -->

      <div
        class="timeline-item"
        data-title="Yale"
        data-field="Causal AI"
        data-description="At Yale and VA, I moved toward causal AI and individualized treatment effects, using large-scale health data to study why patients respond differently to treatments."
      >

        <div class="click-here">
          Research highlights
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


      <!-- STANFORD -->

      <div
        class="timeline-item active"
        data-title="Stanford"
        data-field="Mechanism-Informed Causal AI"
        data-description="At Stanford, I work on Mechanism-Informed Causal AI for Precision Medicine, combining causal inference, machine learning, and biomedical knowledge to better understand variation in treatment response."
      >

        <div class="click-here">
          Research highlights
        </div>

        <div class="timeline-label">

          <div class="timeline-place">
            Stanford
          </div>

          <div class="timeline-field">
            Mechanism-Informed Causal AI
          </div>

        </div>

        <div class="timeline-dot"></div>

      </div>

    </div>

  </div>


  <div
    class="journey-card"
    id="journeyCard"
  >

    <h3
      class="journey-title"
      id="journeyTitle"
    >
      Stanford
    </h3>

    <div
      class="journey-field"
      id="journeyField"
    >
      Precision Medicine
    </div>

    <p
      class="journey-description"
      id="journeyDescription"
    >
      I work on AI for precision medicine, combining causal inference, machine learning, and biomedical knowledge to better understand variation in treatment response.
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


  function updateJourney(
    item,
    index
  ) {

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

        card.classList.remove(
          "fade"
        );

      },
      150
    );


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


    const percentage =
      (index /
        (items.length - 1))
      * 100;

    progress.style.width =
      percentage + "%";


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


  updateJourney(
    items[7],
    7
  );

})();

</script>
