<template>
  <div>
    <PrivacyPolicyHeader />
    <div class="container mt-5">
      <PrivacyPolicy />
    </div>
  </div>
</template>

<script>
import PrivacyPolicy from "../components/privacy-policy/privacyPolicy.vue";
import PrivacyPolicyHeader from "../components/privacy-policy/privacyPolicyHeader.vue";

export default {
  data() {
    return {
      activeEl: "1",
    };
  },
  methods: {
    toggleActive(value) {
      this.activeEl = value;
    },
  },
  components: { PrivacyPolicy, PrivacyPolicyHeader },
};
</script>
<style scoped>
@media only screen and (max-width: 572px) {
  .privacy--policy_content {
    display: block;
    justify-content: center;
  }
  .privacy--policy_nav {
    justify-content: center;
    margin-left: 30px;
    margin-bottom: 30px;
  }
  li {
    font-size: 25px !important;
  }
  li.active {
    background-color: var(--primary-color);
    color: white !important;
    padding: 10px;
  }
}
</style>
