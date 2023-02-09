<script  setup lang="ts">
import { onMounted, ref } from 'vue';

const props:any=defineProps({
  
  per: { type: String, required: true },
    color: { type: String, required: false, default: '#726A95' },
    colorBg: { type: String, required: false, default: '#e1e1e1' },
    textSize: { type: String, required: false, default: '2' },
})
    const DoughnutChart = ref(null);
    const sliceOne = ref(null);
    const sliceTwo = ref(null);
    const chartCenter = ref(null);
    const perTitle = ref(null);
    const getChartLine = () => {
      const per =props.per;
      let textSize = 16 + 'px';
      let base = '#E6E8F0';
      let color =props.color;


      let deg = (per / 100) * 360 + 'deg';
      let deg1 = '90deg';
      let deg2 = deg;
      let base2 = base;
      let center = '#fff';
      let color2 = color;
      let textColor = '2B2B2B';

      if (per < 50) {
        deg1 = (per / 100) * 360 + 90 + 'deg';
        deg2 = '0deg';

        base = color;
        color = base2;
        color2 = base2;
      }

      DoughnutChart.value.style.background = base;

      sliceOne.value.style.transform = 'rotate(' + deg1 + ')';
      sliceOne.value.style.background = color;

      sliceTwo.value.style.transform = 'rotate(' + deg2 + ')';
      sliceTwo.value.style.background = color2;

      chartCenter.value.style.background = center;

      perTitle.value.innerHTML = per + '%';
      perTitle.value.style.color = textColor;
      perTitle.value.style.fontSize = textSize;
    };

    onMounted(() => {
      getChartLine();
    });

</script>

<template>
  <div class="chart__wrapper">
    <div class="donut__chart" ref="DoughnutChart">
      <div class="donut__slice slice__one" ref="sliceOne"></div>
      <div class="donut__slice slice__two" ref="sliceTwo"></div>
      <div class="chart__center" ref="chartCenter">
        <span class="chart__title" ref="perTitle"></span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.chart__wrapper {
  float: left;
  background: #fff;
}

.donut__chart {
  width: 60px;
  height: 60px;
  position: relative;
  border-radius: 50%;
  overflow: hidden;
}

.donut__chart .chart__center {
  position: absolute;
  border-radius: 50%;
  top: 6px;
  left: 6px;
  width: calc(60px - (6px * 2));
  height: calc(60px - (6px * 2));
}

.donut__chart .donut__slice {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.donut__chart .donut__slice.slice__one {
  clip: rect(0 60px calc(60px / 2) 0);
}

.donut__chart .donut__slice.slice__two {
  clip: rect(0 calc(60px / 2) 60px 0);
}

.donut__chart > .chart__center > span {
  display: block;
  text-align: center;
  font-weight: bold;
  line-height: calc(60px - (6px * 2));
}

.chart__title {
  user-select: none;
  font-family: inherit;
}
</style>
