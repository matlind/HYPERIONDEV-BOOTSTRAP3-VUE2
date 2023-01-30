<template>
    <div class="card-media container">
      <div class="row">
        <div class="col-xs-3">
          <img :src="image.src" :alt="image.alt" />
        </div>
        <div class="col-xs-9">
          <div class="row">
            <div class="col-xs-12">
              <h2> {{ title }}</h2>
            </div>
          </div>
          <div class="row">
            <div class="col-xs-12">
              <button class = "CardMedia__button" 
                @click="onButtonClick(cta.link)"
              >
                {{ cta.copy }}
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
    name: "CardMedia",
    data() {
        return {
            title: 'Web Developer Bootcamp Trial',
            image: {
                src: "/images/beginner-php-fundamentals.png",
                alt: ""
            },
            cta: {
                copy: "Continue your tiral",
                href: ""
            }
        }
    },
    methods: {
      onButtonClick (link) {
        // navigate to link
        console.log(link);
      }
    }
}
</script>

<style>
.CardMedia__button {
    list-style-type: none;
}
</style>