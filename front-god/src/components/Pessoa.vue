<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }} </h2>
        <Info />
    </div>
</template>
<script>
import Info from './Info.vue';
export default{
    name: "pessoa",
    data() {
        return {
            nome: "Mattheus"
        };
    },
    components: { Info }
}
</script>