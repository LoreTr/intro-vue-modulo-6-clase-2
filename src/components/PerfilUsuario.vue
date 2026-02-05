<template>
    <div class="perfil">
        <h1>{{ nombre }}</h1>
        <h2>{{ ocupacion }}</h2>

        <img :src="fotoUrl" alt="Foto de perfil">

        <form>
            <div>
                <label>Nombre:</label>
                <input type="text" v-model="nombre">
            </div>

            <div>
                <label>Ocupación:</label>
                <input type="text" v-model="ocupacion">
            </div>

            <div>
                <label>Biografía:</label>
                <textarea v-model="biografia"></textarea>
            </div>

            <div>
                <label>Foto URL:</label>
                <input type="text" v-model="fotoUrl">
            </div>

            <div>
                <label>Nivel de experiencia:</label>
                <input type="number" v-model="nivelExperiencia">
            </div>
        </form>
    </div>
</template>
<script>

export default {
    name:"PerfilUsuario",
    data() {
        return {
            nombre:'',
            ocupacion:"Desempleada",
            biografia:"Actualmente me encuentro en búsqueda activa de empleo, con disponibilidad inmediata y motivación por integrarme a un equipo de trabajo donde pueda aportar mis conocimientos y seguir desarrollándome profesionalmente.",
            fotoUrl:'https://picsum.photos/200/300',
            nivelExperiencia:0
        };
    }
};
</script>
<style scoped>
    
</style>