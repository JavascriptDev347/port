<template>

  <div class="container">
    <div class="col-md-12 col-sm-12-col-xs-12">
      <div class="section_heading text-center"><strong>Works</strong>
        <h2>My Work</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer tellus est, finibus ut congue sed,
          faucibus ut dui. Sed congue nisl dolor, id dapibus leo elementum posuere.</p>

      </div>
      <div class="cards">
        <v-card
            class="mx-auto"
            max-width="400"
            v-for="(item,index) in data"
            :key="index"
            style="overflow: hidden"
        >
          <v-img
              class="align-end "
              height="200"
              contain
              :src="`workImg/${item.img}`"
              alt="o no o no onononon"
          >
            <v-card-title>
              {{ item.name }}
            </v-card-title>
          </v-img>


          <v-card-subtitle class="pt-4">
            Work
          </v-card-subtitle>

          <v-card-text>
            <div style="text-transform: uppercase">{{ item.name }}</div>

            <div>{{ item.title }}</div>
          </v-card-text>

          <v-card-actions>
            <v-btn color="orange">
              <a :href="item.url" target="_blank">Share</a>
            </v-btn>

            <v-btn color="orange">
              <a :href="item.code" target="_blank">Code</a>
            </v-btn>
          </v-card-actions>
        </v-card>
      </div>

    </div>
  </div>

</template>

<script setup>

const data = [
  {
    name: "Pizza",
    title: "Pizza sayti React jsda tuzilgan",
    url: "https://affectionate-brahmagupta-e9d4ac.netlify.app/",
    img: "work1.jpg",
    code: "https://github.com/RustambekJavascript"
  },
  {
    name: "allin.uz",
    title: "allin.uz saytini bir qismi qilingan",
    url: "https://vueoneproject.netlify.app/",
    img: "work2.svg",
    code: "https://github.com/RustambekJavascript"
  },
  {
    name: "Books",
    title: "Kitoblarni saqlab quyadi",
    url: "https://thisbook.netlify.app/",
    img: "work3.jpg",
  },
  {
    name: "JS Todo List",
    title: "Javascriptda Todo app",
    url: "https://todolistitemsjs.netlify.app/",
    img: "work4.png",
    code: "https://github.com/RustambekJavascript"
  },
  {
    name: "Safia Backery ",
    title: "Safia Backery tort do'koning veb site",
    url: "https://pedantic-visvesvaraya-eef631.netlify.app/",
    img: "work5.png",
    code: "https://github.com/RustambekJavascript"
  },
  {
    name: "Music Player ",
    title: "Music Player Javascriptda ",
    ulr: "https://temurbekmusic.netlify.app/",
    code: "https://github.com/RustambekJavascript/musicPlayer",
    img: "work6.jpg"
  }
]

</script>

<style>

.cards {
  display: flex;
  justify-content: space-between;
  width: 100%;
  flex-wrap: wrap;
  gap: 25px;
}
</style>