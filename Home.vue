<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App" v-bind:title.sync="doc.title" />
    <div v-if="abb">
      搭撒发
    </div>
    <button @click="abb = !abb">按钮</button>
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
  data(){
    return{
      doc:{
        title:'33333333',
        aaa:'22222'
      },
      abb:true
    }
  },
  /***********
  beforeCreate(){
    alert('beforCreate')
  },
  created(){
    alert('created')
  },
  beforeMount(){
    alert('beforMount')
  },
  mounted(){
    alert('mounted')
  },
  beforeUpdate(){
    alert('brforUpdate')
  },
  updated(){
    alert('upDate')
  }
  ** */
}
</script>
