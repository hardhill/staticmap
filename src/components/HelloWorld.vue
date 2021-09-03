<template>
  <div class="hello">
    <img :src="`https://static-maps.yandex.ru/1.x/?ll=${coords[1]},${coords[0]}&size=${size[0]},${size[1]}&z=${zoom}&l=${typemap}&pt=${coords[1]},${coords[0]},pm2bll`"/>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    coords:{
      type:Array,
      required:true
    },
    zoom:{
      type:Number,
      required:true
    },
    typemap:{
      type:String,
      required:true,
      default(){
        return 'map'
      }
    },
    size:{
      type:Array,
      required:true,
      default(){
        return [450,450]
      }
    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
