<template>
<h1>{{ msg }}</h1>
<div class="container1">
  <div class="hello">
    
  
    <div class="card border-dark mb-3" style="max-width: 18rem;">
  <div class="card-header">Hola Pedro Perez</div>
  <div class="card-body text-dark">
    <h5 class="card-title">Toma Tu Primer Break</h5>
    <p class="card-text">Recuerda que tienes un break mas!.</p>
  </div>
</div>
  </div>
  
    <div id="break-2">
  <button class="btn-dark" v-on:click="firtbreak">Primer Break</button>
</div>
  </div>
</template>

<script>
export default {
  name: 'break-2',
  props: {
    msg: String
  },
  methods: {
    firtbreak: function (event) {
      alert('Hola ' + this.name + ' Es tu primer Break!' )
      if (event) {
        alert(event.target.tagName)
      }
    } 
  }
}
</script>

<style scoped>
.container1{
  
  margin-left: 38%;
  width: 20%;
  
  
}
</style>
