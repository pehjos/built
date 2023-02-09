<template >
    <div class="table">
        <div class="table_top">
            <p>Latest Orders</p>
            <div class="last">
<p>Data Updates Every 3 Hours</p>
<button>View All Orders</button>
            </div>
        </div>  
        <div class="table_contents">
            <main>
                <div>
                  <table
                    aria-label="orders table"
                   
                  >
                    <thead >
                      <tr>
                        <th scope="col">Products</th>
                        <th scope="col" >Order ID</th>
                        <th scope="col" >Date</th>
                        <th scope="col" >Customer name</th>
                        <th scope="col" >Status</th>
                        <th scope="col" >Amount</th>
                        <th scope="col" >Action</th>
                      </tr>
                    </thead>
                    <tbody >
                      <tr v-for="(item, i) in 4" :key="i">
                        <td >
                          <div class="table_img">
                            <img src="https://m-cdn.phonearena.com/images/review/5440-wide-two_1200/Apple-iPhone-14-Pro-vs-iPhone-14-one-is-new-the-other-is-not.jpg"/>
                            <p>Iphone</p>
                          </div>
                        </td>
          
                        <td >
                       <p>#11232</p>
                        </td>
                        <td >
                        <p>Jul 29, 2022</p>
                             </td>
                             <td >
                                <p>Anastasia Hasuna</p>
                                 </td>
                                 <td >
                                    <p>Pending</p>
                                     </td>
                                     <td >
                                        <p>$1100.00</p>
                                         </td>
                        <td >
                          <div class="dropdown">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-three-dots" viewBox="0 0 16 16">
                                <path d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z"/>
                              </svg>
                            <div class="dropdown-content">
                              <p >ACTIONS</p>
                              <a href="#" class="flex P200 O400" >
                               Edit</a
                              >
                              <a
                                href="#"
                              
                              >
                              Delete</a
                              >
                            </div>
                          </div>
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </div>
          
              
                <!-- End of Empty State -->
              </main>
              <!-- Ending of table content -->
        </div>
    </div>
</template>
<script setup lang="ts">

</script>
<style scoped>
table {
    border: 1px solid #e6e8f0;
    border-radius: 8px;
  }
  
  tr:nth-child(even) {
 background-color:  #f9fafd;
  }
  th{
    background-color: #e6e8f0;
  }
  tbody tr:hover {
    background-color: #edeff5;
  }

  /* Dropdown Button */
  .dropbtn {
    /* background-color: #ffffff; */
    color: white;
    padding: 16px;
    font-size: 16px;
    border: none;
  }
  
  /* The container <div> - needed to position the dropdown content */
  .dropdown {
    position: relative;
    display: inline-block;
  }
  .table_img{
    display: flex;
    margin-left: 40px;
    align-items: center;
  }
  .table_img>img{
    width: 30px;
    height: 30px;
    border-radius: 8px;
  }
  /* Dropdown Content (Hidden by Default) */
  .dropdown-content {
    display: none;
    margin-left: -150px;
    position: absolute;
    background-color: #ffffff;
    min-width: 160px;
    box-shadow: 0px 4px 8px rgba(16, 24, 64, 0.16);
    border-radius: 8px;
    z-index: 1;
  }
  
  /* Links inside the dropdown */
  .dropdown-content a {
    color: #474d66;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
  }

  /* Change color of dropdown links on hover */
  .dropdown-content a:hover {
    background-color: #f9e0d7;
    color: lightgray;
    border-left: 3px solid gray;
  }
  
  /* Show the dropdown menu on hover */
  .dropdown:hover .dropdown-content {
    display: block;
  }
  
  /* Change the background color of the dropdown button when the dropdown content is shown */
  .dropdown:hover .dropbtn {
    background-color: #fafbff;
   
  } 
  /* spacing */

table {
    table-layout: fixed;
    width: 100%;
    border-collapse: collapse;
  
  }

  
  th,
  td {
    padding: 10px;
  }  
  td {
    text-align: center;
  }
  .table_top{
    justify-content: space-between;
    display: flex;
    padding: 5px;
  }
  .last{
    display: flex;
    align-items: center;
  }
  .table{
    margin: 20px;
 border-radius: 8px;
    box-shadow: rgba(0, 0, 0, 0.02) 0px 1px 3px 0px, rgba(27, 31, 35, 0.15) 0px 0px 0px 1px;
  }
  button{
    cursor: pointer;
    background-color: blue;
    color: white;
  }
  .table_top>p{
    font-weight: bolder;
    font-size: 16px;
  }
</style>