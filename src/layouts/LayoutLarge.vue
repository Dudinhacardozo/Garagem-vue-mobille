<script setup>
  import LargeAside from '@/components/templates/large/LargeAside.vue';
</script>

<template>
  <div id="layout-large">
    <aside>
      <large-aside />
      <login-view/>
    </aside>
    <main>
      <router-view />
    </main>
    
  </div>
</template>

<style scoped>
#layout-large {
  display: grid;
  grid-template-columns: 1fr 5fr;
  grid-template-rows: auto 1fr auto;
  grid-template-areas:
    'aside header'
    'aside main'
    'aside footer';
  min-height: 100vh;
}

header {
  display: flex;
  widows: 100vw;
  justify-content: flex-end;
  padding: 1.5rem;
  grid-area: header;
}

aside {
  border-right: #F29F05 1px solid;
  box-shadow: 0 0 10px 0 #F29F05;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding-top: 1.5rem;
  padding-bottom: 1.5rem;
  grid-area: aside;
  background-color: #87CEEB	;			;
}

main {
  min-height: 80%;
  padding: 2rem;
  grid-area: main;
}

footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 3rem;
  background-color: #B0E0E6;
  grid-area: footer;
}

</style>