<template>
  <div class="about">
    <h1>This is an about page</h1>
    <div v-for="x in [1, 2, 3, 4, 5, 6, 7]" :key="x">
      <router-link :to="'/demo/' + x">User {{ x }}</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutView",
  data() {
    return {
      users: [
        {
          id: 1,
          name: "John Doe",
        },
        {
          id: 2,
          name: "Jane Doe",
        },
        {
          id: 3,
          name: "Juan Dela Cruz",
        },
      ],
    };
  },
};
</script>
