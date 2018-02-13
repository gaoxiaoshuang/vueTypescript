<template>
    <div>
        <table id="table">
            <caption>table title and/or explanatory text</caption>
            <thead>
                <tr>
                    <th>header</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>data</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
<script lang='ts'>
import * as $ from 'jquery'
import Vue from 'vue'
import {
    Component,
    Prop
} from 'vue-property-decorator'

@Component({})
export default class dataTable extends Vue {
    @Prop({
        type: String,
        default: 'Default Value'
    }) msg: string;
    mounted() {
        // console.log($('#table'))
        this.initTable()
    }
    initTable() {
        console.log("===", $('#table').DataTable)
        $('#table').DataTable()
    }
}
</script>
