<template>
<!-- {{$route.params.id}} 해당 글 아이디 불러올수있다.-->
  <div>
    <h5>{{ 블로그글[$route.params.id].title }}</h5>
    <p>{{ 블로그글[$route.params.id].content }}</p>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'Detail',
  props:{
    블로그글 : Array,
  },
  components: {
},
}
</script>

<style>

</style>