<template>
  <div class="container">

    <div class="row">
      <div class="col-md-12">
        <v-carousel
            height="400"
            hide-delimiters
            progress="primary"
        >
          <v-carousel-item
              v-for="(slide, i) in slides"
              :key="i"
          >
            <v-sheet
                height="100%"
            >
              <div class="d-flex fill-height justify-center align-center">
                <div class="text-h2">
                  {{ slide }} Slide
                </div>
              </div>
            </v-sheet>
          </v-carousel-item>
        </v-carousel>
      </div>
    </div>
  </div>

</template>
<script>
export default {
  data() {
    return {
      slides: [
        'First',
        'Second',
        'Third',
        'Fourth',
        'Fifth',
      ],
    }
  },
}

</script>