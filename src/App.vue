<template>
  <div id="app">
    <hello
      :list="list" :title="title" :unit="num" 
      @callback="getMsg"
    ></hello>
  </div>
</template>

<script>
import Hello from './components/Hello'

export default {
  name: 'app',
  components: {
    Hello
  },
  data () {
    return {
      title: '列表',
      list: [
        {
          name: '1'
        },
        {
          name: '2'
        },
        {
          name: '3'
        },
        {
          name: '4'
        },
        {
          name: '5'
        },
        {
          name: '6'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        },
        {
          name: '7'
        }
      ],
      willShow:true,
      msg: '',
      unit:''
    }
  },
  methods: {
    getMsg (msg) {
      this.msg = msg
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
   -webkit-font-smoothing: antialiased;
   -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
