<template>
    <div class="card mt-3">
        <div class="card-header">
            <div class="card-title text-center">
                Todos
            </div>
        </div>
        <div class="card-body">
            <div class="d-flex justify-content-between align-items-center mt-1 cardList" v-for="card in cards">
                <input type="checkbox" id="{{card.id}}">
                <label for="{{card.id}}" class="user-select-none">{{ card.title }}</label>
                <button class="btn btn-danger"><i class="fas fa-trash"></i></button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        cards: {
            type: Object,
            required: true
        }
    }
}
</script>

<style scoped>
.cardList{
    border-bottom: 1px solid rgba(128, 128, 128, 0.58);
    padding: 1rem;
}
</style>