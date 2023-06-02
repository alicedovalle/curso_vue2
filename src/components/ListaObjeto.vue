<template>
    <div>
        <select>
            <option :value="null">Nenhuma</option>
            <optio value="name">Alfabética</optio>
            <option value="year">Ano</option>
            <option value="awards">Prêmios</option>
        </select>
        <Filme div v-for="f in lista" :filme="f"></Filme>
    </div>
</template>

<script>
import Filme from './Filme.vue'

export default {
    components: { Filme },
    data() {
        return {
            lista: [],
            order:null
        }
    },
    mounted() {
        this.loadData();
    },
    methods: {
        loadData() {
            this.lista = [
                {
                    'name': "O Senhor dos Anéis",
                    'year': 2003,
                    'awards': 11
                },
                {
                    'name': "Titanic",
                    'year': 1997,
                    'awards': 11
                },
                {
                    'name': "Ben-Hur",
                    'year': 1959,
                    'awards': 11
                },
                {
                    'name': "Amor, Sublime Amor",
                    'year': 1961,
                    'awards': 10
                },
                {
                    'name': "Gigi",
                    'year': 1958,
                    'awards': 9
                },
                {
                    'name': "O último Imperador",
                    'year': 1987,
                    'awards': 9
                },
            ];
        }
    }
}
</script>

<style scoped></style>