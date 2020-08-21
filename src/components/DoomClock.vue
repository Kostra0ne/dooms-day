<template>
  <div class="hello">
    <b>{{time}}</b>
  </div>
</template>

<script>
import moment from "moment";
import Countdown from "moment-countdown";
console.log(moment, Countdown);
export default {
  name: "DoomsClock",
  data() {
    return {
      time: "...loading",
      interval: null
    };
  },
  methods: {
    getTick() {
      this.interval = setInterval(() => {
        this.time = moment(Date.now())
          .countdown("2020-10-19")
          .toString();
      }, 1000);
    }
  },
  created() {
    this.getTick();
  },
  beforeDestroy() {
    clearInterval(this.interval);
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
