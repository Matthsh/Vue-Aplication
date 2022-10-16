<template>
    <div>
        <div>
            <Input />
        </div>
        <div>
            <Input />
        </div>
        <div>
            <Submit />
        </div>
    </div>

</template>
<script>
import Input from './Input.vue';
import Submit from './Submit.vue';
export default {
    name: "Form",
    components: { Input, Submit }
}
</script>