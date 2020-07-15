<template>
    <form action="" method="POST">
        <h1>Encuesta Dojo</h1>
        <p>Nombre <input type="text" v-model="nombre"></p>
        <p>Ubicación:
            <select v-model="locacion">
                <option value="1">Dallas</option>
                <option value="2">Chicago</option>
                <option value="3">Seattle</option>
                <option value="4">Los Angeles</option>
                <option value="5">Oackland</option>
            </select>
        </p>
        <p>Framework/s:
            <select v-model="lenguaje">
                <option value="1">HTML</option>
                <option value="2">CSS</option>
                <option value="3">Javascript</option>
                <option value="4">Vue</option>
                <option value="5">React</option>
                <option value="6">Angular</option>
            </select>
        </p>
        <p>Comentarios: <textarea v-model="comentario"></textarea></p>
        <p><input type="submit" value="Añadir Item"></p>
    </form>
</template>

<script>
export default {
    name: 'Formulario',
    data() {
        return {
            nombre: "",
            locacion: "",
            lenguaje: "",
            comentario: "",
        }
    }
}

</script>
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