<template>
    <div class="hello">
        <dataTable msg="'你好'" />
    </div>
</template>
<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'
import dataTable from './common/dataTable.vue'
@Component({
    components: {
        dataTable
    }
})
export default class HelloWorld extends Vue {
    msg: string = 'Welcome to Your Vue.js App'
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
    font-weight: normal;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: #42b983;
}
</style>
