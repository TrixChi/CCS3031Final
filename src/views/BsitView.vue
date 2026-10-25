<script setup>
import { fetchProgramDetails } from '@/backend'
</script>

<template>
  <div class="bscs-page-container">
    //HERO SECTION
    <header class="hero-section">
      <div class="bg-shape shape-gold"></div>
      <div class="bg-shape shape-dark-green"></div>

      <div class="hero-content">
        <div class="hero-text">
          <h1>Information Technology</h1>
          <p>
            The Information Technology (IT) Program is designed for students who wants to study
            information technology in depth.
          </p>

          <div class="hero-buttons">
            <a href="#objectives" class="btn btn-dark"><i class="fas fa-list"></i> Objectives</a>
            <a href="#society" class="btn btn-green"><i class="fas fa-users"></i> Campus Life</a>
          </div>
        </div>

        <div class="hero-logo">
          <img
            src="https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/1-2048x2048.png"
            alt="Information Technology Society Logo"
          />
          <h3>INFORMATION TECHNOLOGY<br />SOCIETY</h3>
        </div>
      </div>
    </header>

    //MAIN CONTENT WRAPPER
    <div class="content-wrapper">
      //PROGRAM EDUCATIONAL OBJECTIVES
      <section id="objectives" class="section-block">
        <h2 class="section-title">PROGRAM EDUCATIONAL OBJECTIVES</h2>

        <div class="text-content">
          <ol>
            <li>
              Exhibit skills, knowledge and leadership to excel in their information technology
              careers and related discipline.
            </li>
            <li>
              Exhibit high standard of professionalism who are effective members of multi-discipline
              development teams.
            </li>
            <li>
              Involved in scholarly activities, research and outreach that contributes to the
              improvement and transformation of society.
            </li>
            <li>
              Demonstrate ethical, professional, spiritual values, and social responsibility
              associated with their Information Technology careers and related professions.
            </li>
            <li>
              Exhibit proficiency in the use of traditional and digital media arts, designing,
              developing and implementing digital media solutions in fields of entertainment and
              corporate environments.
            </li>
          </ol>
        </div>

        <!-- Anchor Links List -->
        <ul class="anchor-links">
          <li><a href="#outcomes">Program Outcomes</a></li>
          <li><a href="#rationale">Curriculum Rationale</a></li>
          <li><a href="#description">Curriculum Description</a></li>
          <li><a href="#society">Student Organization</a></li>
          <li><a href="#graduate-outcomes">Graduate Outcomes</a></li>
        </ul>
      </section>

      <!-- 3. PROGRAM OUTCOMES -->
      <section id="outcomes" class="section-block">
        <h2 class="section-title">PROGRAM OUTCOMES</h2>

        <h3 class="sub-title">The graduates have the ability to</h3>
        <div class="text-content">
          <p>
            a) articulate and discuss the latest developments in the specific field of practice.
            <em
              >(Philippine Qualifications Framework (PQF) level 6 descriptor) (Graduate Outcomes: CS
              10, IS 10, IT13).</em
            >
          </p>
          <p>
            b) effectively communicate orally and in writing using both English and Filipino
            <em>(Graduate Outcomes: CS08, 1508, IT10).</em>
          </p>
          <p>
            c) work effectively and independently in multi-disciplinary and multi-cultural teams.
            <em>(PQF level 6 descriptor) (Graduate Outcomes: CS07, ISO7, IT08).</em>
          </p>
          <p>
            d) act in recognition of professional, social and ethical responsibility
            <em>(Graduate Outcomes: CS09, 1509, IT12)</em>
          </p>
          <p>
            e) preserve and promote "Filipino historical and cultural heritage"
            <em>(based on RA 7722).</em>
          </p>
        </div>

        <h3 class="sub-title">The graduates of BSCS, BSIS, and BSIT must have the ability to</h3>
        <div class="text-content">
          <p>
            a) analyze complex problems, and identify and define the computing requirements needed
            to design an appropriate solution <em>(Graduate Outcomes: CS02, 1502-03, IT03).</em>
          </p>
          <p>
            b) apply computing and other knowledge domains to address real-world problems
            <em>(Graduate Outcomes: CS0 1, 1501, IT01).</em>
          </p>
          <p>
            c) design and develop computing solutions using a system-level perspective
            <em>(Graduate Outcomes: CS03-05, 1504-05, IT05).</em>
          </p>
          <p>d) utilize modern computing tools <em>(Graduate Outcomes: CSOS, ISOS, IT07).</em></p>
        </div>
      </section>

      //CURRICULUM RATIONALE
      <section id="rationale" class="section-block">
        <div class="ched-header">
          <h3>Based on CHED Memo Order No. 25 s. 2015</h3>
          <p>Effective: Academic Year 2018-2019</p>
        </div>

        <h3 class="sub-title">Curriculum Rationale:</h3>
        <p class="text-content">
          The computing field has grown enormously and is described as dynamic. It encompasses
          computer engineering, software engineering, computer science, information systems, and
          information technology. Based on the Guidelines for the Implementation of CMO 46 s 2012
          which implements the shift to learning competency-based standards/outcomes-based
          education" the Commission released CMO 25 s 2015 last August 2015 that integrates the
          outcomes-based education. It specifies the "core competencies" expected of graduates of
          Bachelor of Science in Computer Science (BSCS), Bachelor of Science in Information Systems
          (BSIS) and Bachelor of Science in Information Technology (BSIT). The Commission recognizes
          the need to be responsive to the current needs of the country and in order to face the
          challenges of advancement. It is essential and important that the country's computing
          capability be continually developed and strengthened. In this PSG it clearly defines the
          area of focus for each field, common outcomes for each discipline and new GE for K-12
          program. In the PSG it defines the BSCS program that includes the study of computing
          concepts and theories, algorithmic foundations and new developments in computing. The
          program prepares students to design and create algorithmically complex software and
          develop new and effective algorithms for solving computing problems.
        </p>
      </section>

      //CURRICULUM DESCRIPTION
      <section id="description" class="section-block">
        <h3 class="sub-title">Curriculum Description:</h3>
        <ul class="custom-bullets">
          <li>
            The BSIT curriculum includes basic and advanced courses on planning, development,
            integration, and management of information technology infrastructure that provide
            computing solutions to address the needs of organizations.
          </li>
          <li>
            The curriculum should include courses to cover Knowledge Areas recommended in ACM
            Computer Science Curricula 2013 (enumerated in PSG).
          </li>
          <li>
            Defines eleven (11) Knowledge Areas:
            <ul class="sub-bullets">
              <li>Information Technology Fundamentals</li>
              <li>Human Computer Interaction</li>
              <li>Information Assurance and Security</li>
              <li>Information Management</li>
              <li>Integrative Programming and Technologies</li>
              <li>Networking</li>
              <li>Platform Technologies</li>
              <li>Systems Administration and Maintenance</li>
              <li>Systems Integration and Architecture</li>
              <li>Social and Professional Issues</li>
              <li>Web Systems and Technologies</li>
            </ul>
          </li>
        </ul>
      </section>

      //COMPUTER SCIENCE SOCIETY (Campus Life)
      <section id="society" class="society-section">
        <!-- This section mimics the diagonal background split -->
        <div class="society-bg-gold"></div>
        <div class="society-bg-dark"></div>

        <div class="society-content">
          <div class="society-logo">
            <img
              src="https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/1-2048x2048.png"
              alt="Info"
            />
            <h3>Information Technology Students Organization</h3>
          </div>
          <div class="society-text">
            <p>
              TThe embodiment of Information Technology Students is enriched through camaraderie as
              they strengthen their bonds with each year level. Through different outreach
              activities and as well as the college and university, the members of this organization
              gets to meet and gather ideas to come up and be able to fulfill the mission of this
              organization, thus, giving them ample knowledge that could help them build a better
              personality through working together.
            </p>
          </div>
        </div>
      </section>

      //GRADUATE OUTCOMES TABLE
      <section id="graduate-outcomes" class="section-block">
        <h2 class="section-title">Bachelor of Science in Information Technology (BSIT)</h2>

        <div class="table-responsive">
          <table class="outcomes-table">
            <thead>
              <tr>
                <th>Graduate Outcomes Code</th>
                <th>Graduate Outcomes</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>CS01</td>
                <td>
                  Apply knowledge of computing fundamentals, knowledge of a computing
                  specialization, and mathematics, science, and domain knowledge appropriate for the
                  computing specialization to the abstraction and conceptualization of computing
                  models from defined problems and requirements.
                </td>
              </tr>
              <tr>
                <td>CS02</td>
                <td>
                  Identify, analyze, formulate, research literature, and solve complex computing
                  problems and requirements reaching substantiated conclusions using fundamental
                  principles of mathematics, computing sciences, and relevant domain disciplines.
                </td>
              </tr>
              <tr>
                <td>CS03</td>
                <td>
                  An ability to apply mathematical foundations, algorithmic principles and computer
                  science theory in the modeling and design of computer-based systems in a way that
                  demonstrates comprehension of the tradeoffs involved in decision choices.
                </td>
              </tr>
              <tr>
                <td>CS04</td>
                <td>
                  Knowledge and understanding of information security issues in relation to the
                  design, development and use of information systems.
                </td>
              </tr>
              <tr>
                <td>CS05</td>
                <td>
                  Design and evaluate solutions for complex computing problems, and design and
                  evaluate systems, components, or processes that meet specified needs with
                  appropriate consideration for public health and safety, cultural, societal, and
                  environmental considerations.
                </td>
              </tr>
              <tr>
                <td>CS06</td>
                <td>
                  Create, select, adapt and apply appropriate techniques, resources and modern
                  computing tools to complex computing activities, with an understanding of the
                  limitations to accomplish a common goal.
                </td>
              </tr>
              <tr>
                <td>CS07</td>
                <td>
                  Function effectively as an individual and as a member or leader in diverse teams
                  and in multidisciplinary settings.
                </td>
              </tr>
              <tr>
                <td>CS08</td>
                <td>
                  Communicate effectively with the computing community and with society at large
                  about complex computing activities by being able to comprehend and write effective
                  reports, design documentation, make effective presentations, and give and
                  understand clear instructions.
                </td>
              </tr>
              <tr>
                <td>CS09</td>
                <td>
                  An ability to recognize the legal, social, ethical and professional issues
                  involved in the utilization of computer technology and be guided by the adoption
                  of appropriate professional, ethical and legal practices.
                </td>
              </tr>
              <tr>
                <td>CS10</td>
                <td>
                  Recognize the need, and have the ability, to engage in independent learning for
                  continual development as a computing professional.
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped>
.bscs-page-container {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
  background-color: #f8f9fa;
  scroll-behavior: smooth;
}

/*HERO SECTION*/
.hero-section {
  position: relative;
  width: 100%;
  min-height: 60vh;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  background-color: #fff;
  padding-top: 80px;
}

.bg-shape {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
}

.shape-gold {
  background-color: #d4a017;
  clip-path: polygon(0 0, 100% 0, 30% 100%, 0 100%);
  z-index: 2;
}

.shape-dark-green {
  background-color: #3b4a45;
  clip-path: polygon(100% 0, 100% 100%, 30% 100%);
  z-index: 1;
}

.hero-content {
  position: relative;
  z-index: 10;
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  max-width: 1200px;
  padding: 0 2rem;
}

.hero-text {
  flex: 1;
  color: white;
  max-width: 600px;
}

.hero-text h1 {
  font-size: 3.5rem;
  font-weight: 300;
  margin-bottom: 1rem;
}

.hero-text p {
  font-size: 1.1rem;
  margin-bottom: 2rem;
  line-height: 1.6;
  color: #e0e0e0;
}

.hero-buttons {
  display: flex;
  gap: 1rem;
}

.btn {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 12px 24px;
  text-decoration: none;
  font-weight: 600;
  border-radius: 4px;
  transition: opacity 0.3s;
}

.btn:hover {
  opacity: 0.9;
}

.btn-dark {
  background-color: #1e3a5f;
  color: white;
}

.btn-green {
  background-color: #4caf50;
  color: white;
}

.hero-logo {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: #333;
}

.hero-logo img {
  width: 150px;
  margin-bottom: 1rem;
  border-radius: 10px;
}

.hero-logo h3 {
  font-weight: 600;
  letter-spacing: 1px;
}

/*CONTENT WRAPPER & SECTIONS*/
.content-wrapper {
  max-width: 1000px;
  margin: 0 auto;
  padding: 4rem 2rem;
  background-color: #f8f9fa;
}

.section-block {
  margin-bottom: 4rem;
}

.section-title {
  text-align: center;
  font-size: 1.5rem;
  color: #1e3a5f;
  margin-bottom: 2rem;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.sub-title {
  font-size: 1.1rem;
  color: #333;
  margin-top: 2rem;
  margin-bottom: 1rem;
}

.text-content {
  font-size: 0.95rem;
  line-height: 1.6;
  color: #555;
}

.text-content p {
  margin-bottom: 1rem;
}

.text-content ol {
  padding-left: 1.5rem;
}

.text-content ol li {
  margin-bottom: 0.5rem;
}

.anchor-links {
  list-style-type: disc;
  padding-left: 1.5rem;
  margin-top: 2rem;
}

.anchor-links li a {
  color: #2a7cc7;
  text-decoration: none;
  font-size: 0.9rem;
}

.anchor-links li a:hover {
  text-decoration: underline;
}

.ched-header {
  text-align: center;
  font-weight: bold;
  margin-bottom: 2rem;
  color: #333;
}

.custom-bullets {
  padding-left: 1.5rem;
  font-size: 0.95rem;
  line-height: 1.6;
  color: #555;
}

.custom-bullets > li {
  margin-bottom: 1rem;
}

.sub-bullets {
  list-style-type: none;
  padding-left: 1rem;
  margin-top: 0.5rem;
  border-left: 2px solid #ccc;
}

.sub-bullets li {
  margin-bottom: 0.3rem;
}

/*SOCIETY SECTION*/
.society-section {
  position: relative;
  width: 100%;
  min-height: 400px;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  margin: 4rem 0;
  background-color: #f8f9fa;
}

.society-bg-gold {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #d4a017;
  clip-path: polygon(0 0, 50% 0, 20% 100%, 0 100%);
  z-index: 1;
}

.society-bg-dark {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #2c3e35;
  clip-path: polygon(50% 0, 100% 0, 100% 100%, 20% 100%);
  z-index: 1;
}

.society-content {
  position: relative;
  z-index: 10;
  display: flex;
  align-items: center;
  justify-content: center;
  max-width: 1000px;
  padding: 0 2rem;
  gap: 4rem;
}

.society-logo {
  flex: 1;
  text-align: center;
  color: #1e3a5f;
}

.society-logo img {
  width: 180px;
  margin-bottom: 1rem;
  border-radius: 10px;
}

.society-text {
  flex: 2;
  color: #e0e0e0;
  font-size: 0.95rem;
  line-height: 1.6;
}

/*TABLE SECTION*/
.table-responsive {
  overflow-x: auto;
}

.outcomes-table {
  width: 100%;
  border-collapse: collapse;
  background-color: white;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
}

.outcomes-table th,
.outcomes-table td {
  padding: 1rem;
  text-align: left;
  border-bottom: 1px solid #ddd;
  font-size: 0.9rem;
  line-height: 1.5;
}

.outcomes-table th {
  background-color: #f1f1f1;
  font-weight: 600;
  color: #333;
  width: 20%;
}

.outcomes-table td:first-child {
  font-weight: bold;
  color: #1e3a5f;
}

/*Mobile Responsiveness*/
@media (max-width: 900px) {
  .hero-content,
  .society-content {
    flex-direction: column;
    text-align: center;
  }

  .hero-text h1 {
    font-size: 2.5rem;
  }

  .hero-buttons {
    justify-content: center;
  }

  .bg-shape,
  .society-bg-gold,
  .society-bg-dark {
    clip-path: none;
    height: 50%;
  }

  .shape-dark-green {
    top: 50%;
  }
  .society-bg-dark {
    top: 50%;
  }
}
</style>
