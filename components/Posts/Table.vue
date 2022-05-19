<script >

export default {
  data() {
    return {
      posts: [],

    };
  },

  async fetch() {
    this.posts = await fetch("https://jsonplaceholder.typicode.com/posts").then(
      (res) => res.json()
    );
  },

};

</script>

<template>

  <div class="table m-14">
    <div class="table-container flex justify-center align-center">
      <div class="table-col ">
        <h1 class="text-center mb-[2rem]">TOP 100: Posts</h1>
    <p v-if="$fetchState.pending">Loading....</p>
    <p v-else-if="$fetchState.error">Error while fetching posts</p>
    <div v-else class="table-container flex justify-center align-center">
      <div class="table-col w-[80%]" >
                  <PostsRow
          v-for="(post, index) in posts"
          :key="post.id"
          :title="post.title"
          :body="post.body"
          :index="index"
          :id="post.id"
          :isHeader="true"
          />
      </div>
            <!-- <div class="table-col ml-[5rem]">
      
        <PostsRow
          v-for="(post, index) in posts"
          :key="post.id"
          :title="post.title"
          :body="post.rank"
          :index="index"
          :id="post.id"
          :isHeader="true"

        />
      </div> -->
    </div>

      </div>

    </div>
  </div>
</template>

<style scoped>

/* .table h1 {
  margin-bottom: 2rem;
} */
/* .table-container {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
} */
/* .table-col {
  width: 48%;
} */
/* .posts-head {
  text-align: center;
} */
</style>
