<template>
  <div>
    <Menu />
    <Nuxt />
    <Footer />
  </div>
</template>

<style>
body {
  font-family: "Montserrat", sans-serif !important;
}
</style>

<script>
export default {
  data() {
    return {
      title: "Life"
    };
  },
  head() {
    return {
      title: this.title,
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: "description",
          name: "description",
          content: "E"
        }
      ],
      // link tags
      link: [
        {
          //rel: "stylesheet",
          //href: "https://unpkg.com/aos@next/dist/aos.css",
        }
      ],
      script: [
        {
          src: "https://unpkg.com/ionicons@5.2.3/dist/ionicons.js"
        }, // Insert in body
        {
          //type: "text/javascript",
          //src: "https://unpkg.com/aos@next/dist/aos.js",
        } // Insert in body
      ],
      style: [
        {
          /*
          type: "text/css",
          inner: "body { background-color: #000; color: #fff}",
          undo: false*/
        }
        // ...
      ]
    };
  }
};
</script>
