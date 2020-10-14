<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
          <form id="search">
        Search <input name="query" v-model="searchQuery" />
      </form>
    <HelloWorld 
        :heroes="gridData"
        :columns="gridColumns"
        :filter-key="searchQuery"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  data: function() {
  return{
          searchQuery: "",
          gridColumns: ["name", "power"],
          gridData: [
            { name: "Chuck Norris", power: Infinity },
            { name: "Bruce Lee", power: 9000 },
            { name: "Jackie Chan", power: 7000 },
            { name: "Jet Li", power: 8000 }
          ]
        }
  }

}
</script>
