<template>
    <div v-for="(filme, ano) in lista">
        {{ ano }} : {{ filme }}
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
            this.lista = {
                "O Senhor dos Anéis: O Retorno do Rei": 2003,
                "Titanic": 1997,
                "Ben-Hur": 1959,
                "Amor, Sublime Amor": 1961,
                "Gigi": 1958,
                "O último Imperador": 1987
            };
        }
    }
}
</script>

<style scoped></style>