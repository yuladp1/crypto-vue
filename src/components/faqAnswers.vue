<template>
  <ul>
    <div>
      <li>
        {{ article.articleTitle }}
        <button v-on:click="toggleMethod" v-bind:class="buttonClicked"></button>
      </li>
      <p v-if="showParagraf">
        {{ article.article }}
      </p>
    </div>
  </ul>
</template>

<script>
export default {
  name: "FaqAnswers",
  props: ["article"],
  data() {
    return {
      showParagraf: false,
      showArticle: "",
      buttonClicked: "",
    };
  },
  methods: {
    toggleMethod() {
      this.showParagraf = !this.showParagraf;
      this.showArticle = "show";
      if (this.showParagraf == true) {
        this.buttonClicked = "button-active";
      } else {
        this.buttonClicked = "";
      }
    },
  },
};
</script>

<style scoped>
.button-active {
  background-image: url ("../assets/Minus.svg");
  background-color: aqua;
}

ul {
  display: flex;
  flex-direction: column;
  margin-block-start: 0;
  margin-block-end: 0;
  padding-inline-start: 0;
  margin: 16px 24px;
}
li {
  width: 100%;
  list-style: none;
  display: flex;
  justify-content: space-between;
  padding: 16px 0;
  border-top: 2px solid rgba(207, 219, 213, 0.6);
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
}
p {
  font-size: 14px;
  font-weight: 500;
  line-height: 20px;
  text-align: left;
  color: #6f767e;
}
button {
  margin-right: 0;
  margin-left: auto;
  height: 24px;
  padding: 0 0;
  background-image: url ("../assets/Add_Plus.svg");
  min-width: 24px;
}
</style>
