<template>
  <div id="app">
    <!-- test -->
    <Table />
    <Flog />
  </div>
</template>

<script>
import Table from './Table';
import Flog from './Flog';

export default {
  name: 'app',
  components: {
    Table,
    Flog
  }
}
</script>

<!-- CSS libraries -->
<style src="normalize.css/normalize.css"></style>

<!-- Global CSS -->
<style>
  code {
    font-family: Menlo, Monaco, Lucida Console, Liberation Mono, DejaVu Sans Mono, Bitstream Vera Sans Mono, Courier New, monospace, serif;
    font-size: 0.9em;
    white-space: pre-wrap;
    color: #2c3e50;
  }

  code::before, code::after {
    content: '`';
  }
</style>

<!-- Scoped component css -->
<!-- It only affect current component -->
<style scoped>
  #app {
    /* text-align: center; */
    padding: 12px;
  }

  #app h1 {
    color: #2c3e50;
    font-weight: 300;
    margin: 0;
  }


  @keyframes spin {
    from {transform:rotate(0deg);}
    to {transform:rotate(360deg);}
  }
</style>
