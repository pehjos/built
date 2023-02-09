<template >
  <div class="item_">
    <div class="items_sold">
      <h6>Most Sold Items</h6>
      <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-three-dots" viewBox="0 0 16 16">
        <path d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z"/>
      </svg>
        </div>

    <div class="doughnut_layout">
  <!-- (A) DONUT CHART -->

  <div class="donut"><div class="hole"><p>Total Sold</p></div></div>

 <!-- lengend -->
<div class="legend">
<div class="legend_child legend_child_div">
<div></div><p>Jeans</p>
</div>
<div class="legend_child1 legend_child_div">
  <div></div><p>Shirts</p>
  </div>
  <div class="legend_child2 legend_child_div">
    <div></div><p>Caps</p>
    </div>
    <div class="legend_child3 legend_child_div">
      <div></div><p>Others</p>
      </div>
</div>
</div>

    </div>
</template>
<script setup lang="ts" >

</script>
<style scoped>
  /* (A) PIE CHART */
.donut {
  /* (A1) CIRCLE */
  width: 200px; height: 200px;
  border-radius: 50%;

  /* (A2) SEGMENTS */
  background: conic-gradient(
    blue 0deg 90deg,
    green 90deg 180deg,
    violet 180deg 270deg,
    orangered 270deg 360deg
  );
}

/* (B) DONUT "CONVERSION" */
/* (B1) SMALLER CIRCLE */
.hole {
  width: 160px; height: 160px;
  border-radius: 50%;
  background: #fff;
}
.item_{
  box-shadow: rgba(0, 0, 0, 0.02) 0px 1px 3px 0px, rgba(27, 31, 35, 0.15) 0px 0px 0px 1px;
  padding: 10px;
  height: 400px;
  width: 40%;
  border-radius: 8px;
  margin: 20px;
}
.doughnut_layout{
    display: flex;
    align-items: center;
   
   
}
/* (B2) "CONVERT PIE TO DONUT" - CENTER SMALLER CIRCLE */
.donut {
  display: flex;
  align-items: center;
  justify-content: center;
}

/* (C) LEGEND */
/* (C1) LEGEND CONTAINER */
.legend {
  display: flex;
flex-direction: column;


}

.legend_child_div{
display: flex;
align-items: center;
margin: 10px;

font-size: 12px;
}
.legend_child>div{
width: 10px;
height: 10px;
border-radius: 50%;
background-color: blue;
padding: 2px;
display: flex;
margin: 10px;
  }
  .legend_child1>div{
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background-color: green;
    padding: 2px;
    display: flex;
    margin: 10px;
      }
      .legend_child2>div{
        width: 10px;
        height: 10px;
        border-radius: 50%;
        background-color: violet;
        padding: 2px;
        display: flex;
        margin: 10px;
          }
          .legend_child3>div{
            width: 10px;
            display: flex;
            margin: 10px;
            height: 10px;
      
            border-radius: 50%;
            background-color: orangered;
            padding: 2px;
               font-size: 13px;
              }
              .items_sold{
            
               display: flex;
               justify-content: space-between;
              }
              .items_sold>h6{
                font-size: 14px; 
              
               }
              .items_sold>svg{
             height: 30px;
             box-shadow: rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px;
             border-radius: 8px;
             padding: 5px;
             width: 30px;
               }
               .hole::before{
                content: '120K';
                font-weight: bolder;
                margin-top: 60px;
                font-size: 25px;
                margin-left: 55px;
                position: absolute;
              }
              .hole>p{
              
                margin-top: 100px;
             
                margin-left: 55px;
                position: absolute;
              }
</style>