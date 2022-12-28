<template>
  <ul>
    <div>
      <li>
        {{ article.articleTitle }}
        <div @click="toggleMethod">
          {{ symbol }}
        </div>
      </li>
      <p v-if="showParagraf">
        {{ article.article }}
      </p>
    </div>
  </ul>
</template>
/*----------------*/
<script>
export default {
  name: "FaqAnswers",
  props: ["article"],
  data() {
    return {
      showParagraf: false,
      showArticle: "",
      symbol: "+",
    };
  },
  methods: {
    toggleMethod() {
      this.showParagraf = !this.showParagraf;
      this.showArticle = "show";
      if (this.showParagraf == true) {
        this.symbol = "-";
      } else {
        this.symbol = "+";
      }
    },
  },
};
</script>

<style scoped>
ul {
  display: flex;
  flex-direction: column;
  background: white;
  padding: 16px 24px;
}
li {
  width: 100%;
  list-style: none;
  display: flex;
  justify-content: space-between;
  padding: 16px 0;
  border-top: 2px solid rgba(207, 219, 213, 0.6);
  font-size: 24px;
  font-weight: 700;
  line-height: 32px;
}
p {
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
  text-align: left;
  color: #6f767e;
}
figure {
  margin-right: 0;
  margin-left: auto;
  width: 24px;
  height: 24px;
  padding: 0 0;
  background-position: center;
  background-repeat: no-repeat;
  background-size: 10px 10px;
  min-width: 24px;
}
</style>
