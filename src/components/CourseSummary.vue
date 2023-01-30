<template>
  <div class="course-summary container">
    <div class="row">
      <h3 class="col-xs-12">
        {{ progress.title }}
      </h3>
    </div>
    <ul class="row">
      <li class="course-summary__item col-xs-12 col-sm-6" v-for="skill in progress.skills" :key="skill.label">
        {{ skill.label }}
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  name: "CourseSummary",

  data() {
    return {
      progress: {
        title: 'Your Progress',
        complete: {
          done: 1,
          steps: 4,
        },
        skills: [
          {
            label: 'Industry Knowledge 1',
            done: true,
          },
          {
            label: 'Industry Knowledge 2',
            done: false,
          },
          {
            label: 'Industry Knowledge 3',
            done: false,
          },
        ],
      }
    }
  }

};
</script>
<style>
.course-summary__item {
  list-style-type: none;
}
</style>