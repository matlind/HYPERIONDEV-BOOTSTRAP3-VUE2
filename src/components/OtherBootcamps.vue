<template>
    <div class="other-bootcamp container">
    <div class="row">
      <h3 class="col-xs-12">
        {{ title }}
      </h3>
    </div>
    <ul class="row">
      <li class="other-bootcamp__item col-xs-12 col-sm-6" v-for="bootcamps in bootcamps" :key="bootcamps.label">
        {{ bootcamps.label }}
      </li>
    </ul>
  </div>
</template>

<script>

export default {
    name: "OtherBootcamps",
    data() {
        return {
            title: 'Trial another Bootcamp',
            bootcamps: [
                {
                    label: 'Mobile Developer Bootcamp',
                    image: {
                        src: "/images/layer-115.png",
                        alt: ""
                    },
                },
                {
                    label: 'Software Engineering Bootcamp',
                    image: {
                        src: "/images/layer-114.png",
                        alt: ""
                    },
                }
            ],
        }
    }
};
</script>
<style>
.other-bootcamps__item {
    list-style-type: none;
}
</style>