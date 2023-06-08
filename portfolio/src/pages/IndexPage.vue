<template>
  <q-page class="flex flex-center smaple">
    <div>
      <q-card
        flat
        class="text-white bg-transparent"
        style="max-width: 500px; width: 100%"
      >
        <q-card-section class="text-center">
          <q-item-label class="name">
            {{ myName }}
          </q-item-label>
        </q-card-section>
        <q-separator class="q-ma-md bg-white" />
        <q-card-section class="row justify-center q-gutter-md">
          <q-btn
            outline
            href="https://github.com/Andrew-1000"
            target="_blank"
            icon="fab fa-github"
            round
          ></q-btn>
          <q-btn outline href="https://www.linkedin.com/in/andrew-ambia-044171124/" target="_blank" icon="fab fa-linkedin" color="white" round></q-btn>
          <q-btn outline href="#" target="_blank" icon="fab fa-android" color="white" round></q-btn>
          <q-btn outline href="mailto:andrew.ambia@gmail.com" target="_blank" icon="fab fa-google" color="white" round></q-btn>
        </q-card-section>
      </q-card>
    </div>
  </q-page>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "IndexPage",
  setup() {
    return {
      myName: ref("Andrew Ambia"),
      positions: ref([]),
    };
  },

  mounted() {},
  methods: {},
});
</script>

<style>
.smaple {
  background-image: url("../assets/backg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  text-shadow: 0 0 10px #c2a6a6;
}

.name {
  font-size: 5em;
  font-weight: bolder;
}
</style>
