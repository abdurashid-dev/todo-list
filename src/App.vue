<template>
    <div class="main">
        <div class="title text-center p-3">
            <h1>To Do List</h1>
        </div>
        <Form/>
    </div>
</template>

<script>
import Form from "@/components/form/Form.vue";

export default {
    components: {Form}
}
</script>

<style>
.main {
    max-width: 500px;
    margin: 0 auto;
}
</style>