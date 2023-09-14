<template>
  <div class="tset">
    <form v-on:submit="onSubmitForm">
      <input type="text" v-model="myid" placeholder="아이디">
      <input type="text" v-model="mypw" placeholder="비밀번호">
      <!-- <div>{{myid}}</div>
      <div>{{mypw}}</div> -->
      <button type="submit">회원가입</button>
    </form>
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',
    data(){
      return{
        myid:"",
        mypw:""
      }
    },
    methods:{
      onSubmitForm(e){
        e.preventDefault();
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
