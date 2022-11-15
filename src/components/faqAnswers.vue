<template>
  <h1>FAQ</h1>
  <p>Найдите ответы, на интересующие вопросы</p>
  <ul>
    <div v-for="q in questions" :key="q.id">
      <li>
        {{ q }}<button v-on:click="toggleMethod" v-bind:class="buttonClicked"></button>
      </li>
      <p v-if="showParagraf" :class="showArticle">
        Staking is a method of verifying and securing transactions on proof of stake
        blockchains. It’s faster and more energy efficient than other methods such as
        proof of work. Plus, participants get rewarded for helping in the process. In
        exchange for delegating your crypto, you get rewarded with more assets from the
        network. To generate staking rewards on a Proof of Stake blockchain, a node has to
        designate a certain amount of tokens on the network as a stake (similar to a
        security deposit). The chance of that node being chosen to validate the next block
        is typically proportional to the number of tokens being staked. If the node
        successfully validates a block, it is awarded the staking reward, similar to a
        miner being rewarded in Proof of Work chains. Validators lose part of their stake
        if they approve a fraudulent transaction — this incentivizes them to only approve
        valid transactions.
      </p>
    </div>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      questions: [
        "How does staking work?",
        "Which Proof of Stake asset(s) earn staking rewards?",
        "Who is eligible to stake on DEPO?",
        "How does ETH staking work?",
        "What are the risks associated with staking?",
        "How do I earn DeFi yield on DEPO?",
        "What’s the difference between staking and DeFi yield?",
      ],
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
}
p {
  height: 0;
}
.show {
  height: auto;
  width: auto;
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
button {
  margin-right: 0;
  margin-left: auto;
  width: 24px;
  height: 24px;
  padding: 0 0;
  background-image: url ("../assets/Add_Plus.svg");
}
</style>
