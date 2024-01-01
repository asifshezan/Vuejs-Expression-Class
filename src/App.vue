<script setup>
import Image from './components/Image.vue';
import Expression from './components/Expression.vue';

 const title = "This is just normal title.";
 const desc = "This is just normal desc.";
 const newtitle = "This title is declared by v-text.";
 const newdesc = "<strong>This description is declared by v-html.</strong>"

 const data = {
  title: "This is a object title.",
  desc: "This is a object desc."
 }

 const array = [
  {
    title: "This is a array title 1.",
    desc: "This is a array desc 1."
  },
  {
    title: "This is a array title 2.",
    desc: "This is a array desc 2."
  }
 ]




</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>

  <Expression/>
  <!-- <Image/> -->
  <!-- <HelloWorld msg="Vite + Vue" /> -->

  <div class="">
    <h2>
      {{ title }}
    </h2>
    <p>
      {{ desc }}
    </p>
    <h2 v-text="newtitle"></h2>
    <p v-html="newdesc"></p>
  </div>

  <div class="">
    <h2>
      {{ data.title }}
    </h2>
    <p>
      {{ data.desc }}
    </p>
  </div>

  <div class="">
    <h2>
      {{ array[0].title }}
    </h2>
    <p>
      {{ array[0].desc }}
    </p>
  </div>

  <div class="">
    <h2>
      {{ array[1].title }}
    </h2>
    <p>
      {{ array[1].desc }}
    </p>
  </div>



</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
