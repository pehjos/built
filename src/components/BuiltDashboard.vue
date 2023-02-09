<template >
    <div class="dashboard">
        <div class="dashboard_side_menu">
            <SideMenu/>
            </div>
             <div class="dashboard_analytics">
                <div class="appbar_section">
    <AppbarComponentVue/>
</div>
    <RecentAnalyticsCardVue/>
    <div class="middle_chart">
        <BarAnalytics/>
       <DoughnutPieVue/> 
    </div>
  <TableComponent/>
            </div>
    </div>
</template>
<script setup lang="ts">
import SideMenu from './SideMenu.vue';
import AppbarComponentVue from './AppbarComponent.vue';
import RecentAnalyticsCardVue from './RecentAnalyticsCard.vue'
import BarAnalytics from './BarAnalytics.vue'
import DoughnutPieVue from './DoughnutPie.vue';
import TableComponent from './TableComponent.vue'
</script>
<style scoped>
    .dashboard{
        display: flex;
 
        top: 0;
    }
    .dashboard_side_menu{
        flex: 0.2;
left: 0;
margin-left: 10px;
    }
  
    .dashboard_analytics{
flex: 0.8;

    }
    .middle_chart{
        display: flex;
        width: 100%;
    
        justify-content: space-between;
    }
  
</style>