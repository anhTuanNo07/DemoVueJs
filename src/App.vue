<template>
  <div id="app">
    {{ tongTien | dauChamPhanTach}}
    <button @click="tongTien += 20000"></button>
  </div>
</template>

<script>

export default {
  data() {
    return {
      tongTien: 1000000
    }
  },
  filters: {
    dauChamPhanTach: function(soTien) {
      return soTien.toFixed(2).replace(/\d(?=(\d{3})+\.)/g, '$&,')
    }
  }
}
</script>

<style>

</style>
