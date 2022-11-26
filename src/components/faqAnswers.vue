<template>
  <ul>
    <div>
      <li>
        {{ article.articleTitle }}
        <figure v-on:click="toggleMethod" v-bind:class="buttonClicked" />
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
@media screen and (min-width: 320px) and (max-width: 720px) {
  .button-active {
    background-image: url("../assets/Minus.svg");
  }

  ul {
    display: flex;
    flex-direction: column;
    padding: 16px 24px;
    width: 100%;
  }
  li {
    width: 100%;
    list-style: none;
    display: flex;
    justify-content: space-between;
    padding: 16px 0;
    border-top: 2px solid rgba(207, 219, 213, 0.6);
    font-size: 16px;
    font-weight: 700;
    line-height: 24px;
  }
  p {
    font-size: 14px;
    font-weight: 500;
    line-height: 20px;
    text-align: left;
    color: #6f767e;
  }
  figure {
    margin-right: 0;
    margin-left: auto;
    width: 24px;
    height: 24px;
    padding: 0 0;
    background-image: url ("../assets/addplus.svg");
    min-width: 24px;
  }
}
@media screen and (min-width: 721px) and (max-width: 1440px) {
  .button-active {
    background-image: url("../assets/Minus.svg");
  }

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
    background-image: url ("../assets/addplus.svg");
    min-width: 24px;
  }
}

@media screen and (min-width: 1441px) {
  .button-active {
    background-image: url("../assets/Minus.svg");
  }

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
    background-image: url ("../assets/addplus.svg");
    min-width: 24px;
  }
}
</style>
