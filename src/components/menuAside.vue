<template>
  <aside>
    <nav>
      <ul>
        <!-- <div v-for="l in list" :key="l.id">
          <li>{{ l }}</li>
        </div>  -->
        <li>djfhdkjfdkfdk</li>
        <li>djfhdkjfdkfdk</li>
        <li>djfhdkjfdkfdk</li>
        <li>djfhdkjfdkfdk</li>
        <li>djfhdkjfdkfdk</li>
      </ul>
    </nav>
  </aside>
</template>

<script>
export default {
  data() {
    return {
      list: ["About", "How does it works", "Were we work", "FAQ", "Contacts"],
    };
  },
};
</script>

<style scoped>
aside {
  width: 192px;
  height: 600px;
}
nav {
  width: 100%;
  height: 100%;
}
ul {
  margin-block-start: 0;
  margin-block-end: 0;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  padding-inline-start: 0px;
  margin: 70px auto 24px 24px;
  display: flex;
  flex-direction: column;
  width: 100px;
  height: 200px;
}
li {
  list-style-type: none;
  color: black;
  width: 30px;
  height: 20px;
}
</style>
