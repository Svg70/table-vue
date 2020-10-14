<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">

    <HelloWorld 
        :heroes="gridData"
        :columns="gridColumns"

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
          gridColumns: [],
          gridData: [

          ]
        }
  }

}
</script>
