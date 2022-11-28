<template>
    <div class="main">
        <div class="title text-center p-3">
            <h1>To Do List</h1>
        </div>
        <Form/>
        <CardList/>
    </div>
</template>

<script>
import Form from "@/components/form/Form.vue";
import CardList from "@/components/cardList/CardList.vue";

export default {
    components: {CardList, Form}
}
</script>

<style>
.main {
    max-width: 500px;
    margin: 0 auto;
}
</style>