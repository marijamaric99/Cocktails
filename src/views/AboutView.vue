<template>
  <v-main class="custom-background">
    <div class="about">
      <v-app-bar app color="primary">
          <v-toolbar-title style="font-size: 30px; color: white; margin-right: 10px;">Cocktails <v-icon right style="color: white;">mdi-glass-cocktail</v-icon></v-toolbar-title>
          <v-spacer></v-spacer>
          <v-btn text to="/" style="color: white; font-size: 16px;">
            <v-icon left>mdi-home</v-icon>
            Početna
          </v-btn>
          <div style="width: 1px; background-color: white; height: 24px; margin: 0 12px;"></div> <!-- Uspravna crta između linkova -->
          <v-btn text to="/about" style="color: white; font-size: 16px;">
            <v-icon left>mdi-information</v-icon>
            O nama
          </v-btn>
      </v-app-bar>

      <div class="content">
        <p class="page-title">Key project features include:</p>
        <ul>
          <li>Retrieving cocktail data from a public API via the RapidAPI website.</li>
          <li>Fast cocktail search with real-time filtering.</li>
          <li>Filtering cocktails by preparation difficulty: easy, medium, hard.</li>
          <li>Pagination of results for easier navigation.</li>
          <li>Editing cocktail preparation difficulty.</li>
          <li>Adding new cocktails.</li>
        </ul>
        <p class="page-title">Used technologies:</p>
        <div class="technologies">
          <div class="technology">
            <a href="https://vuejs.org/" target="_blank">
              <img src="/vuejs.png" alt="Vue.js" class="tech-image" />
            </a>
            <p>Vue.js</p>
          </div>
          <div class="technology">
            <a href="https://vuetifyjs.com/en/" target="_blank">
              <img src="/vuetify.png" alt="Vuetify" class="tech-image" />
            </a>
            <p>Vuetify</p>
          </div>
          <div class="technology">
            <a href="https://axios-http.com/" target="_blank">
              <img src="/axios.png" alt="Axios" class="tech-image" />
            </a>
            <p>Axios</p>
          </div>
          <div class="technology">
            <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" target="_blank">
              <img src="/html.png" alt="HTML" class="tech-image" />
            </a>
            <p>HTML</p>
          </div>
          <div class="technology">
            <a href="https://developer.mozilla.org/en-US/docs/Web/CSS" target="_blank">
              <img src="/css.png" alt="CSS" class="tech-image" />
            </a>
            <p>CSS</p>
          </div>
          <div class="technology">
            <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">
              <img src="/javascript.png" alt="JavaScript" class="tech-image" />
            </a>
            <p>JavaScript</p>
          </div>
        </div>
      </div>
    </div>
  </v-main>
</template>

<style scoped>
.custom-background {
      width: 100%;
      height: 100%;
      background: linear-gradient(
         180deg,
         rgba(142, 182, 255, 0.3) 0%,
         rgba(211, 232, 251, 0.3) 100%
      );
      padding: 20px 0 0 0 !important;
   }

.about {
  max-width: 800px;
  margin: 0 auto;
  margin-bottom: 20px;
  padding: 20px;
  background-color: #64B5F6; /* Dodajte pozadinu */
}

.content {
  background-color: #fff; /* Dodajte pozadinu za sadržaj */
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
}

.page-title {
  font-size: 32px;
  margin-bottom: 20px;
  color: #333; /* Boja teksta */
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); /* Sjena teksta */
}

p {
  font-size: 16px;
  margin-bottom: 10px;
  color: #555; /* Boja teksta */
}

.technologies {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.technology {
  text-align: center;
  flex-basis: calc(33.33% - 20px); /* Postavite željeni broj stupaca */
}

.tech-image:hover {
  transform: scale(1.05); /* Povećajte sliku na hover */
  transition: transform 0.3s ease-in-out;
}

img {
  max-width: 100%;
  height: auto;
  margin-bottom: 10px;
}
</style>
