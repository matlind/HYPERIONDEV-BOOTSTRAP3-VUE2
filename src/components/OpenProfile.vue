<template>
  <div class="open-profile container">
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
              <button class = "OpenProfile__button" 
                @click="onButtonClick(cta.link)"
              >
                {{ cta.copy }}
              </button>
            </div>
          </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OpenProfile",
  data() {
    return {
      title: 'Profile',
      image: {
        src: "/images/student.png",
        alt: ""
      },
      label: 'Edit Profile',
      label2: 'Log out'
    }
  },
  methods: {
    onButtonClick(link) {
      // navigate to link
      console.log(link);
    }
  }
}
</script>

<style>
.OpenProfile2__button {
  list-style-type: none;
}
</style>