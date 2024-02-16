<script>

export default {
    data: () => ({
        contador: 10
    }),
    methods: {
        incrementar() {
            this.contador++
        },
        disminuir() {
            this.contador--
        },
        reset() {
            this.contador = 10
        }
    }
}

</script>

<template>
    <div class="container">
        <img src="./assets/logo.svg" alt="log vue" width="125" height="125"><br>
        <small><h1>Hola Mundo</h1></small>
        <br>
    
        <h2>Contador {{ contador }}</h2><br>
        <button @click="incrementar()">+1</button>
        <button @click="disminuir()">-1</button>
        <button @click="reset()">Reset</button>
    </div>

</template>

<style scoped>
.container {
    text-align: center;
}

small {
    color: #666;

}

h1 {
    font-weight: bolder
}

h2 {
    font-size: 2.5rem;
}

button {
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 6px;
}

</style>
