<script setup>
  //import SmallHeader from '@/components/templates/small/SmallHeader.vue';
  import SmallFooter from '@/components/templates/small/SmallFooter.vue';
</script>

<template>
  <div id="layout-small">
    <main>
      <router-view />
    </main>
    <footer>
      <small-footer />
    </footer>
  </div>
</template>
<style scoped>
#layout-small {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

header {
  display: flex;
  justify-content: space-between;
  padding: 1.5rem;
  border-bottom: #355783 2px solid;
  background-color: #355783;
  color: #eeeeee;
  z-index: 10;
  position: fixed;
  left: 0;
  top: 0;
  width: 100%;
  height: 7%;
}

main {
  margin-top: 5%;
  margin-bottom: 4rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  padding-bottom: 4rem;
  padding-top: 1.5rem;
  position: relative;
}

footer {
  border-top: #fe9103 2px solid;
  box-shadow: 0 0 30px 0 #fe9103;
  padding: 1.5rem;
  margin-top: auto;
  background-color: #355783;

  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  color: #B0E0E6;
  text-align: center;
  z-index: 10;
}
</style>