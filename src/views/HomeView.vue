<!-- <script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <TheWelcome />
  </main>
</template> -->

<script setup>
import { ref } from 'vue'
const isHovered = ref(false)
</script>

<template>
  <div class="section">
    <div>
      <h4>About Company</h4>
      <h2>AI-enabled predictive safety technologies for all</h2>
      <button
        @mouseover="isHovered = true"
        @mouseleave="isHovered = false"
        :class="{ 'button-hover': isHovered }"
      >
        Discover Incognito
      </button>
    </div>
    <div>
      <section class="list">
        <div class="item">
          <img src="../assets/interpretation.png" width="50px" height="50px" />
          <h3>Powerful interpretations</h3>
          <span class="text"
            >Actionable insights and predictions to nip accidents before they even bud</span
          >
        </div>
        <div class="item">
          <img src="../assets/camera-con.png" width="50px" height="50px" />
          <h3>Sleepless Sentries 24/7</h3>
          <span class="text"
            >AI camera network that ensures total surveillance with 0 blind spots 24/7</span
          >
        </div>
      </section>
      <section class="list">
        <div class="item">
          <img src="../assets/scrum.png" width="50px" height="50px" />
          <h3>Agile AI</h3>
          <span class="text"
            >Versatile AI adapts quickly to any industry, ensuring personalized and
            industry-specific safety findings</span
          >
        </div>
        <div class="item">
          <img src="../assets/smarthome.png" width="50px" height="50px" />
          <h3>User-friendly and accessible</h3>
          <span class="text"
            >Human centric user-experience allowing for easy deriving of safety insights</span
          >
        </div>
      </section>
    </div>
  </div>
  <div>
    <section class="list-2">
      <div class="item-2">Sample</div>
      <div class="item-2">Sample</div>
      <div class="item-2">Sample</div>
    </section>
  </div>
</template>

<style>
.section {
  display: flex;
  flex-direction: row;
}

.button-hover {
  background-color: white;
}

button {
  background-color: lightskyblue;
  color: black;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.5s ease;
}

.list {
  display: flex;
  flex-direction: row;
  width: 70%;
}

.list-2 {
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-top: 100px;
}

.item {
  padding: 5px;
}

.item-2 {
  padding: 5px;
}

@media (min-width: 1024px) {
}
</style>
