<template>
  <div
    class="w-192 h-64 sm:text-sm md:text-md xl:text-xl rounded-xl shadow-xl bg-gray-100 flex flex-row"
  >
    <div class="w-1/2 flex flex-wrap content-center justify-center pl-8">
      <mt-dashboard-pie color="#FF8C8C" backgroundColor="#FFE5E5" label="prueba" :percent="50"/>
    </div>
    <div class="w-1/2 align-left  flex flex-wrap justify-center content-center ">
      <span class="font-bold text-left text-3xl pl-4">
        Progreso del tablero
      </span>
    </div>
  </div>
</template>

<script>

import MTDashboardPieChart from '@/components/MTDashboardPieChart.vue';


export default {
  name: "HelloWorld",
  props: {
    msg: String,
    projectProgress: String
  },
  components: {
    'mt-dashboard-pie': MTDashboardPieChart
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
