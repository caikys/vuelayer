<template>
  <div class="hello">
    <button @click.stop="fn()">{{unit}}{{msg}}</button>
    <div class="pop" v-if="willShow"  @click="checktanchuceng">
      <div class="list">
        <div class="title">{{title}}</div>
        <ul>
          <li v-for="item in list" @click.stop="getMsg(item.name)">
            {{item.name}}
          </li>
        </ul>  
      </div>
      
    </div>
  </div>
</template>
<style scoped src='../../static/sass/Hello.css'></style>

<script>
  export default {
    name: 'hello',
    props: {
      unit: {   // 可选字段，有默认值
        type: Number,
        default:1
      },
      title: {
        type: String,
        required : true
      },
      willShow: {
        type: Boolean
        //required : true
      },
      list: {
        type: Array,
        default () {
          return []
        }
      }
    },
    data () {
      return {
        msg: ''
      }
    },
    methods: {
      getMsg (name) {
        this.msg = name;
        this.unit='';
        this.$emit('callback', name)
      },
      checktanchuceng (){
              if(this.willShow=true){
                  this.willShow=false;
              }
          },
      fn:function(){
          if(this.willShow==true){
              this.willShow=false;
            }else{
              this.willShow=true
            }
      }
    }
  }

</script>

