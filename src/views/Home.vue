<template>
  <form>
    <input type="text"
      class="form-control my-2"
      placeholder="Ingrese su nombre"
      v-model="tarea.nombre"
    >
    <div class="form-check form-check-inline">
      <input 
        type="checkbox" 
        name="" 
        id="check-1"
        class="form-check-input"
        v-model="tarea.categorias"
        value="javascript"
      >
      <label for="check-1" class="form-check-label">JavaScript</label>
    </div>
    <div class="form-check form-check-inline">
      <input 
        type="checkbox" 
        name="" 
        id="check-2"
        class="form-check-input"
        v-model="tarea.categorias"
        value="nodejs"
      >
      <label for="check-2" class="form-check-label">NodeJs</label>
    </div>
    <div class="form-check form-check-inline">
      <input 
        type="checkbox" 
        name="" 
        id="check-3"
        class="form-check-input"
        v-model="tarea.categorias"
        value="php"
      >
      <label for="check-3" class="form-check-label">PHP</label>
    </div>

    <p>nombre: {{tarea}} </p>
  </form>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    
  },
  data(){
    return{
      tarea:{
        nombre: '',
        categorias: []
      }
    }
  }
}
</script>
