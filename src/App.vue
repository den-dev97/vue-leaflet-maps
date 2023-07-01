<template>
  <div id="app">
    <div>
      <AgGridVue
          :columnDefs="columnDefs"
          :rowData="rowData"
          class="ag-theme-alpine"
      />
    </div>

  </div>
</template>

<script>
import { AgGridVue } from "ag-grid-vue";


export default {
  name: 'App',
  components: {
    AgGridVue
  },
  data: function () {
    return {
      columnDefs: ['qwe', 'asd', 'zxc'],
      rowData: ['qwe', 'asd', 'zxc']
    }
  }

}
</script>

<style>
@import "~ag-grid-community/dist/styles/ag-grid.css";
@import "~ag-grid-community/dist/styles/ag-theme-alpine.css";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
