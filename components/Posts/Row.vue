<script>
export default {
  props: ["title", "id", "body", "index", "isHeader"],
};
</script>

<template>
  <div
    v-if="isHeader"
    :style="
      index % 2 === 0 ? { background: 'rgba(128, 128, 128, 0.15)' } : null
    "
    class="row flex align-center border-t-1 border-r-gray-400"
  >
    <h4 class="header"></h4>
    <a
      :href="`/posts/${id}`"
      class="header link text-[rgb(10, 31, 148)] m-0 mr-[2rem] py-[0.5rem] px-[1rem] font-bold w-[4rem] text-lg"
      >{{ id }}. {{ title }}</a
    >
  </div>
  <div class="row" v-else>
    <h4>Search for posts</h4>
  </div>
</template>

<style scoped>
/* .row {
  border-top: 1px solid rgba(128, 128, 128, 0.336);
  display: flex;
  align-items: center;
} */
/* .header {
  font-size: 1.25rem;
  color: rgb(10, 31, 148);
  margin: 0;
  margin-right: 2rem;
  padding: 0.5rem 1rem;
  font-weight: 700;
  width: 4rem;
} */
.link {
  text-decoration: none;
  color: rgb(228, 157, 27);
  width: auto;
  font-weight: 500;
}
</style>
