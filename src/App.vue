<script>


export default{
  data(){
    return{
      contador: 10
    }
  },
  methods:{
    incrementar(){
      this.contador++
    },
    decrementar(){
    if(this.contador > 0){
      this.contador--
    }
  },
  ressetar(){
    this.contador = 0
  },
  
  },
  
  Mounted(){
console.log(`Componente montado`)
console.log(`Contador:` + this.contador)
}

}



</script>

<template>
  <button @click="incrementar">+</button>
  <button @click="decrementar">-</button>
  <button @click="ressetar">C</button>
  <p>Valor do contador : {{contador}}</p>
  
</template>

<style scoped>
button{
  margin-left: 10px;
  border-radius: 8px;
  width: 20px;
  height: 20px;
  border: 0;
  background-color:#B78DF2
}

</style>
