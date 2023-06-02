<template>
    <div v-for="filme in lista">
        {{ filme }}
    </div>
</template>

<script>
export default {
    data() {
        return {
            lista: []
        }
    },
    mounted() {
        this.loadData();
    },
    methods: {
        loadData() {
            this.lista = [
                "O Senhor dos Anéis",
                "Titanic",
                "Ben-Hur",
                "Amor, Sublime Amor",
                "Gigi",
                "O último Imperador"
            ];
        }
    }
}
</script>

<style scoped></style>