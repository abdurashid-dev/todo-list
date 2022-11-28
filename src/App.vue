<template>
    <div class="main">
        <div class="title text-center p-3">
            <h1>To Do List</h1>
        </div>
        <Form/>
        <CardList :cards="cards"/>
    </div>
</template>

<script>
import Form from "@/components/form/Form.vue";
import CardList from "@/components/cardList/CardList.vue";

export default {
    components: {CardList, Form},
    data() {
        return {
            cards: [
                {
                    id: 1,
                    title: "Do homework",
                    finished: false
                },
                {
                    id: 2,
                    title: "Drink water",
                    finished: false
                },
                {
                    id: 3,
                    title: "Sleep",
                    finished: false
                }
            ]
        }
    }
}
</script>

<style>
.main {
    max-width: 500px;
    margin: 0 auto;
}
</style>