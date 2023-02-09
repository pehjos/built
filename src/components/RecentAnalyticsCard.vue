<template >
    <div class="analtics_card">

        <div class="card_analytics">
        <div class="text">
      <h6>Todays sales</h6>  
      <h1>$20.4k</h1>
      <p>we have sold 123 items</p>
    </div>
    <div class="doughnut">
<DoughnutChart
class="px-2" per="75" color="blue"  text-size="40"/>

    </div>
</div>

<div class="card_analytics">
    <div class="text">
  <h6>Todays Revenue</h6>  
  <h1>$8.2k</h1>
  <p>Available to payout</p>
</div>
<div class="doughnut">
<DoughnutChart
class="px-2" per="35" color="lightgreen"  text-size="40"

/>

</div>
</div>

<div class="card_analytics">
    <div class="text">
  <h6>In Escrow</h6>  
  <h1>$18.2k</h1>
  <p>Available to payout</p>
</div>
<div class="doughnut">
<DoughnutChart
class="px-2" per="60" color="orange"  text-size="40"

/>

</div>
</div>
</div>
</template>
<script setup lang="ts">
import DoughnutChart from './DoughnutChart.vue';
</script>
<style scope>
 
    .analtics_card{
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin: 10px;
    }
    .card_analytics{
        display: flex;
        border-radius: 8px;
        align-items: center;
        box-shadow: rgba(0, 0, 0, 0.02) 0px 1px 3px 0px, rgba(27, 31, 35, 0.15) 0px 0px 0px 1px;
        width: 400px;
        padding: 10px;
        margin: 10px;
        justify-content: space-between;
        height: 140px;
    }
    .text>h6{
      font-size: 14px;
      font-weight: bolder;
    }
</style>