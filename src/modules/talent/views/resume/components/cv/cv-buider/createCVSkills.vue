<template>
  <div>
    <div>
      <h5 style="font-size: 18px; font-weight: 600">Competency</h5>
      <p class="small text-muted">Tell us about your skills.</p>
      <div class="mt-2">
        <AddCompetency />
      </div>
      
    </div>

    <div class="mt-5">
      <h5 style="font-size: 18px; font-weight: 600">Honours/Awards</h5>
      <p class="small text-muted">Add all awards and achievements</p>
      <div class="mt-2">
        <AddHonours />
      </div>
    </div>

    <div class="mt-5">
      <h5 style="font-size: 18px; font-weight: 600">Languages</h5>
      <p class="small text-muted">
        Tell us about your language and proficiency.
      </p>
      <div class="mt-2">
        <AddLanguages />
      </div>
    </div>

    <div class="mt-5">
      <h5 style="font-size: 18px; font-weight: 600">Hobbies</h5>
      <p class="small text-muted">Tell us what you do for fun</p>
      <div class="mt-2">
        <AddHobbies />
      </div>
    </div>
  </div>
</template>

<script>
import AddCompetency from "./forms/addCompetency.vue";
import AddHobbies from "./forms/addHobbies.vue";
import AddHonours from "./forms/addHonours.vue";
import AddLanguages from "./forms/addLanguages.vue";
export default {
  components: { AddCompetency, AddHonours, AddLanguages, AddHobbies },
  data: () => {
    return {
      add_competency: false,
      add_honours: false,
      add_languages: false,
      add_hobbies: false,
    };
  },
};
</script>
