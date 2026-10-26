<template>
  <div class="faculty-page-container">
    <section class="faculty-hero">
      <p class="small-text">Academically Knowledgeable and Here For You</p>
      <h1 class="main-title">Faculty and Staff Members</h1>
    </section>

    <section class="meet-our-people">
      <div class="people-content">
        <div class="left-title">
          <p class="small-text-dark">Teaching With A Smile</p>
          <h2>Meet Our<br />People</h2>
        </div>
        <div class="right-text">
          <p>
            Lorem ipsum dolor sit amet, conetur adipiscing elit Lorem ipsum dolor sit amet, cons
            ectetur adipiscing elit Lorem ipsum dolor sit almet, conse cteur adipiscing elit aloma
            lomlur off
          </p>
          <p>
            silder tolos. Lorem ipsum dolor sitlor amet, conetur adipiscing elit Lorem ipsum dolor
            sit amet, consectetur adipiscing elit.
          </p>
        </div>
      </div>
    </section>

    <section class="faculty-group">
      <h2 class="section-heading">Dean</h2>

      <div class="hover-card dean-card">
        <img :src="deanInfo.imageUrl" :alt="deanInfo.name" />
        <div class="card-overlay">
          <h3 class="person-name">{{ deanInfo.name }}</h3>
          <p class="person-title">{{ deanInfo.title }}</p>

          <div class="social-icons">
            <a href="#" class="icon facebook">f</a>
            <a href="#" class="icon twitter">t</a>
            <a href="#" class="icon google">G+</a>
            <a href="#" class="icon linkedin">in</a>
          </div>
        </div>
      </div>
    </section>

    <section class="faculty-group">
      <p class="small-text-dark">Teaching as a Way of Life</p>
      <h2 class="section-heading">Department Head and Coordinators</h2>

      <div class="photo-grid">
        <div class="hover-card" v-for="(person, index) in departmentHeads" :key="'dh-' + index">
          <img :src="person.imageUrl" :alt="person.name" />
          <div class="card-overlay">
            <h3 class="person-name">{{ person.name }}</h3>
            <p class="person-title">{{ person.title }}</p>
            <div class="social-icons">
              <a href="#" class="icon facebook">f</a>
              <a href="#" class="icon twitter">t</a>
              <a href="#" class="icon linkedin">in</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="faculty-group">
      <p class="small-text-dark">Teaching as a Way of Life</p>
      <h2 class="section-heading">Faculty</h2>

      <div class="photo-grid">
        <div class="hover-card" v-for="(person, index) in facultyMembers" :key="'fac-' + index">
          <img :src="person.imageUrl" :alt="person.name" />
          <div class="card-overlay">
            <h3 class="person-name">{{ person.name }}</h3>
            <p class="person-title">{{ person.title }}</p>
            <div class="social-icons">
              <a href="#" class="icon facebook">f</a>
              <a href="#" class="icon twitter">t</a>
              <a href="#" class="icon linkedin">in</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="faculty-group">
      <p class="small-text-dark">Service and Teaching</p>
      <h2 class="section-heading">Staff</h2>

      <div class="photo-grid">
        <div class="hover-card" v-for="(person, index) in staffMembers" :key="'staff-' + index">
          <img :src="person.imageUrl" :alt="person.name" />
          <div class="card-overlay">
            <h3 class="person-name">{{ person.name }}</h3>
            <p class="person-title">{{ person.title }}</p>
            <div class="social-icons">
              <a href="#" class="icon facebook">f</a>
              <a href="#" class="icon twitter">t</a>
              <a href="#" class="icon linkedin">in</a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>

import { ref, computed } from 'vue'

const deanInfo = {
  name: 'MA. CHRISTINA A. QUIJANO, MSCS',
  title: 'DEAN',
  imageUrl:
    'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/quijano-e1637132499305.png',
}

const departmentHeads = [
  {
    name: 'REA P. BALONTONG, MBA',
    title: 'DEPARTMENT HEAD(IT & IS)',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/balontong-754x1024.jpg',
  },
  {
    name: 'MARJEE ROSE B. PARRENO, MSCS, MBA',
    title: 'PROGRAM COORDINATOR (BSCS, BSDMIA, and MSCS)',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/parreno-754x1024.jpg',
  },
  {
    name: 'ANA MAE B. CANTEL. MLIS',
    title: 'PROGRAM COORDINATOR (BLIS and MLIS)',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/cantel-754x1024.jpg',
  },
  {
    name: 'LENNON D. PAJAR',
    title: 'COMPUTER LABORATORY COORDINATOR',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/pajar-754x1024.jpg',
  },
]

const facultyMembers = [
  {
    name: 'LEO PAULO B. BELDIA',
    title: 'BSIT AND BSIS PROGRAM',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/beldia-754x1024.jpg',
  },
  {
    name: 'PEDRO PETER RHYS B. CAMBRONERO, MSCS',
    title: 'BSCS PROGRAM',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/cambronero-754x1024.jpg',
  },
  {
    name: 'LESLEY JOY L. DIGNADICE, MBA',
    title: 'BSIT AND BSIS PROGRAM',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/dignadice-1-754x1024.jpg',
  },
  {
    name: 'RODOLFO C. EREGIA, JR.',
    title: 'BSIT AND BSIS PROGRAM',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/eregia-754x1024.jpg',
  },
  {
    name: 'DONIE S. JARDELEZA, MSCS',
    title: 'BSIT AND BSIS PROGRAM',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/jardleza-754x1024.jpg',
  },
  {
    name: 'ANTONIO M. MONTANO, JR.',
    title: 'BSIT AND BSIS PROGRAM',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/montano-754x1024.jpg',
  },
  {
    name: 'ROSE LEAH JOY A. OJACASTRO, MSCS',
    title: 'BSIT AND BSIS PROGRAM',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/ojacastro-754x1024.jpg',
  },
  {
    name: 'MA. SHEILA C. SAPUL, Ph. D.',
    title: 'BSCS PROGRAM',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/sapul-754x1024.jpg',
  },
]

const staffMembers = [
  {
    name: 'CHRISLYN C. CASTANO',
    title: 'SECRETARY',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/castano-754x1024.jpg',
  },
  {
    name: 'A.M.P. LATTER P. TAASAN',
    title: 'COMPUTER LABORATORY TECHNICIAN',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/taasan-754x1024.jpg',
  },
  {
    name: 'CHRISELDA ELAINE ADOR',
    title: 'GUIDANCE COUNSELOR',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/ador-754x1024.jpg',
  },
  {
    name: 'DONNA MAY RIVERA',
    title: 'LIBRARY LIAISON OFFICER',
    imageUrl:
      'https://ccs.cpu.edu.ph/wp-content/uploads/2021/11/rivera-754x1024.png',
  },
]
</script>

<style scoped>
.faculty-page-container {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #0a1f1e;
  padding-bottom: 5rem;
}

.small-text {
  font-size: 0.9rem;
  color: #a0aab2;
  margin-bottom: 0.5rem;
  letter-spacing: 0.5px;
}

.small-text-dark {
  font-size: 0.85rem;
  color: #a0aab2;
  margin-bottom: 0.5rem;
}

.faculty-hero {
  background: linear-gradient(135deg, #071514 0%, #0a1f1e 100%);
  text-align: center;
  padding: 5rem 2rem;
  color: white;
}

.faculty-hero .main-title {
  font-size: 2.8rem;
  font-weight: 700;
  color: #fca311;
  margin: 0;
}

.meet-our-people {
  background-color: #071514;
  padding: 4rem 2rem;
  display: flex;
  justify-content: center;
}

.people-content {
  display: flex;
  max-width: 1000px;
  width: 100%;
  gap: 4rem;
  align-items: center;
}

.left-title {
  border-left: 2px solid #fca311;
  padding-left: 1.5rem;
  flex: 1;
}

.left-title h2 {
  font-family: 'Georgia', serif;
  font-size: 3.5rem;
  color: #ffffff;
  margin: 0;
  line-height: 1.1;
  font-weight: normal;
}

.right-text {
  flex: 2;
  display: flex;
  gap: 2rem;
  color: #a0aab2;
  font-size: 0.95rem;
  line-height: 1.6;
}

.faculty-group {
  text-align: center;
  padding: 3rem 2rem;
  max-width: 1100px;
  margin: 0 auto;
}

.section-heading {
  font-family: 'Georgia', serif;
  font-size: 2rem;
  color: #ffffff;
  margin-bottom: 2.5rem;
  font-weight: normal;
}

.dean-card {
  width: 300px;
  height: 300px;
  margin: 0 auto;
}

.photo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  gap: 1.5rem;
  justify-items: center;
}

/*THE HOVER CARD EFFECT*/
.hover-card {
  position: relative;
  overflow: hidden;
  border: 3px solid #fca311;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
  cursor: pointer;
  width: 100%;
  max-width: 250px;
  aspect-ratio: 3 / 4;
}

.hover-card img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.4s ease;
}

.hover-card:hover img {
  transform: scale(1.08);
}

.card-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(7, 21, 20, 0.9);
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 1.5rem; 
  word-wrap: break-word;
  overflow-wrap: break-word; 
  box-sizing: border-box; 
  text-align: left;

  opacity: 0;
  transition: opacity 0.3s ease;
}

.hover-card:hover .card-overlay {
  opacity: 1;
}

.person-name {
  color: #fca311;
  font-size: 1.2rem; 
  line-height: 1.3; 
  margin-bottom: 0.5rem;
  white-space: normal; 
  width: 100%;
  margin: 0 0 0.5rem 0;
  line-height: 1.3;
  text-transform: uppercase;
}

.person-title {
  color: #ffffff;
  font-size: 0.9rem;
  line-height: 1.4;
  white-space: normal;
  width: 100%;
  margin: 0 0 1.5rem 0;
  font-weight: 600;
  letter-spacing: 1px;
}

.social-icons {
  display: flex;
  gap: 10px;
}

.social-icons .icon {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 32px;
  height: 32px;
  background-color: #fca311;
  color: #0a1f1e;
  border-radius: 50%;
  text-decoration: none;
  font-weight: bold;
  font-family: Arial, sans-serif;
  font-size: 0.9rem;
  transition:
    background-color 0.2s,
    color 0.2s;
}

.social-icons .icon:hover {
  background-color: #ffffff;
  color: #0a1f1e;
}

@media (max-width: 768px) {
  .people-content {
    flex-direction: column;
    gap: 2rem;
    text-align: center;
  }

  .left-title {
    border-left: none;
    border-top: 2px solid #fca311;
    padding-left: 0;
    padding-top: 1rem;
  }

  .right-text {
    flex-direction: column;
    gap: 1rem;
  }

  .faculty-hero .main-title {
    font-size: 2rem;
  }
}
</style>
