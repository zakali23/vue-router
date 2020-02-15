<template>
  <main>
    <h1 class="title">{{ title }}</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae, quos enim? Dignissimos accusamus omnis autem velit unde, labore quaerat, natus officia, enim quia ab voluptas delectus? Totam quod enim doloremque!</p>
  </main>
</template>

<script>
export default {
  name: "contact",
  data: function() {
    return {
      title: "Home"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.title {
  text-align: center;
}
</style>