<template>
  <div class="home">
    <h1 class="title">Doom's Day Clock</h1>
    <DoomClock />
  </div>
</template>

<script>
// @ is an alias to /src
import DoomClock from "@/components/DoomClock.vue";

export default {
  name: "Home",
  components: {
    DoomClock
  }
};
</script>
