<template >
    <div class="main">
        <h6>Total Revenue</h6>
        <div class="bar_labels">

           <div class="label_left">
           
            <div class="label_top">
            <h6>$50.4K</h6>  
            <p>8% than last month<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-up" viewBox="0 0 16 16">
                <path fill-rule="evenodd" d="M8 15a.5.5 0 0 0 .5-.5V2.707l3.146 3.147a.5.5 0 0 0 .708-.708l-4-4a.5.5 0 0 0-.708 0l-4 4a.5.5 0 1 0 .708.708L7.5 2.707V14.5a.5.5 0 0 0 .5.5z"/>
              </svg></p>  
            </div>
           </div>
            <div class="label_right">
            <p>Data Updates Every 3 Hours</p>
            <button>View All Orders</button>
           </div> 
                    </div>
    <div class="bar">
   
<div class="bar_scale">
<ul>
    <li>100k</li>   
    <li>80k</li>   
    <li>60k</li>   
    <li>50k</li>   
    <li>20k</li>   
    <li>0</li>   
</ul>

</div>
<div class="bar_class">
<div class="bars">
<div class="single_bar">
    <div class="bar_inner">

    </div>
</div>
</div>
<div>
    <p>Jan</p>
</div>

</div>
<div class="bar_class">
    <div class="bars">
    <div class="single_bar">
        <div class="bar_inner1">
    
        </div>
    </div>
    </div>
    <div>
        <p>Feb</p>
    </div>
    
    </div>
    <div class="bar_class">
        <div class="bars">
        <div class="single_bar">
            <div class="bar_inner2">
        
            </div>
        </div>
        </div>
        <div>
            <p>Mar</p>
        </div>
        
        </div>
        <div class="bar_class">
            <div class="bars">
            <div class="single_bar">
                <div class="bar_inner3">
            
                </div>
            </div>
            </div>
            <div>
                <p>Apr</p>
            </div>
            
            </div>
            <div class="bar_class">
                <div class="bars">
                <div class="single_bar">
                    <div class="bar_inner4">
                
                    </div>
                </div>
                </div>
                <div>
                    <p>May</p>
                </div>
                
                </div>
                <div class="bar_class">
                    <div class="bars">
                    <div class="single_bar">
                        <div class="bar_inner5">
                    
                        </div>
                    </div>
                    </div>
                    <div>
                        <p>Jun</p>
                    </div>
                    
                    </div>
                    <div class="bar_class">
                        <div class="bars">
                        <div class="single_bar">
                            <div class="bar_inner6">
                        
                            </div>
                        </div>
                        </div>
                        <div>
                            <p>Jul</p>
                        </div>
                        
                        </div>
                        <div class="bar_class">
                            <div class="bars">
                            <div class="single_bar">
                                <div class="bar_inner7">
                            
                                </div>
                            </div>
                            </div>
                            <div>
                                <p>Aug</p>
                            </div>
                            
                            </div>
                            <div class="bar_class">
                                <div class="bars">
                                <div class="single_bar">
                                    <div class="bar_inner8">
                                
                                    </div>
                                </div>
                                </div>
                                <div>
                                    <p>Sep</p>
                                </div>
                                
                                </div>
    </div>
</div>
</template>
<script setup lang="ts">

</script>
<style  scoped>
.label_right{
display: flex;
align-items: center;
}
.main>h6{
    margin: 10px;
    font-size: 14px;
}
.bar{
    display: flex;
justify-content: space-between;
margin-top: 20px;
font-size: 13px;
}
.label_top{
    display: flex;
    margin-top: 10px;
    align-items: center;
    font-size: 16px;
}
.label_top>p{
   font-size: 14px;
   color: green;
}
.label_top>h6{
font-size: 20px;
margin: 10px;
}
.bar_scale{

    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
.bars{
    height: 250px; 
}
.single_bar{
    height: 250px;  
    width: 20px; 
    background-color: whitesmoke;
    border-radius: 4px;
}
.bar_inner{
    height: 23px;  
    width: 20px; 
    position: absolute;
    margin-top: 227px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_inner1{
    height: 60px;  
    width: 20px; 
    position: absolute;
    margin-top: 190px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_inner2{
    height: 40px;  
    width: 20px; 
    position: absolute;
    margin-top: 210px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_inner3{
    height: 50px;  
    width: 20px; 
    position: absolute;
    margin-top: 200px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_inner4{
    height: 60px;  
    width: 20px; 
    position: absolute;
    margin-top: 190px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_inner5{
    height: 19px;  
    width: 20px; 
    position: absolute;
    margin-top: 231px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_inner6{
    height: 50px;  
    width: 20px; 
    position: absolute;
    margin-top: 200px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_inner7{
    height: 30px;  
    width: 20px; 
    position: absolute;
    margin-top: 220px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_inner8{
    height: 30px;  
    width: 20px; 
    position: absolute;
    margin-top: 220px;
    background-color: blue;  
    border-bottom-left-radius: 4px;
    border-bottom-right-radius:4px ;
}
.bar_class{
    display: flex;
    flex-direction: column;

}
li{
    list-style-type: none;
   
}
ul{
    height: 250px;
    display: flex;
    align-items: center;
    margin-left: -30px;
    flex-direction: column;
    justify-content: space-between;
}
.bar_labels{
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: -25px;
    
    height: 40px;
}
.main{
    box-shadow: rgba(0, 0, 0, 0.02) 0px 1px 3px 0px, rgba(27, 31, 35, 0.15) 0px 0px 0px 1px;
    padding: 10px;
    height: 400px;
    width: 85%;
    margin-left: 20px;
    margin-top: 20px;
    border-radius: 8px;
}
</style>