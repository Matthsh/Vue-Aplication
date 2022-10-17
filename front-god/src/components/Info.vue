<template>
    <div>
        <Picture/>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades!</p>
        <p>Utilizo as seguintes tecnologias:</p>
        <ul>
            <li>JavaScript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>
        <p v-show="mostrar_email">Mande um email para: {{email}}</p>
        <p>Para acessar o meu portifólio <a v-bind:href="portifolio">basta clicar aqui</a></p>
    </div>
</template>
<script>
import Picture from './Picture.vue';
    export default {
    name: "Info",
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email: "MattheusMedina@outlook.com",
            portifolio: "https://google.com"
        };
    },
    components: { Picture }
}
</script>