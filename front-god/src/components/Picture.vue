<template>
    <img v-bind:src="avatar" v-bind:alt="descricao">
</template>

<script>
export default {
    name: 'Picture',
    data() {
        return {
            avatar: "/img/burn.jpg",
            descricao: "Mattheus Medina"
        }
    }
}
</script>