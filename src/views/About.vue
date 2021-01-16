<template>
  <div >
    <h1>hjsdkjhsdkjhdskjhksjhdkjhsdkjhks</h1>
  </div>
</template>

<script>
export default {
data(){
  return{
    index:null,
  }
},

created(){
  this.index=this.$route.params.id;
  console.log('ddjjddjjd',this.index);
}
}
</script>

<style>

</style>
