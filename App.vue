<template>
  <div>
    
    <div>
      <button @click="toggleAwesome">Toggle</button>
      <h1 v-if="awesome">Vue</h1>
      <h1 v-else>vooooo </h1>
    </div>

   
    <div>
      <button @click="toggleOK">Toggle</button>
      <h1 v-show="ok">Hi</h1>
    </div>

    
    <div>
      <input type="text" v-model="message" placeholder="Type something">
      <p>You typed: {{ message }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      awesome: true,
      ok: true,
      message: '',
    };
  },
  methods: {
    toggleAwesome() {
      this.awesome = !this.awesome;
    },
    toggleOK() {
      this.ok = !this.ok;
    },
  },
};
</script>


