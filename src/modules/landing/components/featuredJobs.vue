<template>
  <div class="featured--jobs">
    <div class="container">
      <div class="top d-flex align-items-center justify-content-between mb-4">
        <h4 class="header--text" data-aos="fade-up">Featured Jobs</h4>
        <div class="d-lg-flex align-items-center see--all" style="gap: 5px">
          <span>Show all jobs</span>
          <i class="isax isax-arrow-right-1"></i>
        </div>
      </div>

      <!-- Featured Jobs -->
      <cx-jobs data-aos="fade-up" :jobsCount="numberOfItems" />
    </div>
  </div>
</template>

<script>
import cxJobs from "@/components/cards/cxJobs.vue";
export default {
  props: ["numberOfItems"],
  components: { cxJobs },
};
</script>
