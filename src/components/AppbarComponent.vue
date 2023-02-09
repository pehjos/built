<template >
    <div class="appbar">
        <div class="appbar_brand">
        <h3>Dashboard</h3>
        </div>
        <div class="appbar_initials">
            <div class="appbar_search">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
                    <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
                  </svg>
                  <input type="text" placeholder="Search here..."/>
            </div>
            <div class="appbar_profile">
                <div class="appbar_notification">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-bell" viewBox="0 0 16 16">
                        <path d="M8 16a2 2 0 0 0 2-2H6a2 2 0 0 0 2 2zM8 1.918l-.797.161A4.002 4.002 0 0 0 4 6c0 .628-.134 2.197-.459 3.742-.16.767-.376 1.566-.663 2.258h10.244c-.287-.692-.502-1.49-.663-2.258C12.134 8.197 12 6.628 12 6a4.002 4.002 0 0 0-3.203-3.92L8 1.917zM14.22 12c.223.447.481.801.78 1H1c.299-.199.557-.553.78-1C2.68 10.2 3 6.88 3 6c0-2.42 1.72-4.44 4.005-4.901a1 1 0 1 1 1.99 0A5.002 5.002 0 0 1 13 6c0 .88.32 4.2 1.22 6z"/>
                      </svg>
        <p></p>
                </div>
                <div class="appbar_profile_img">
                    <div class="appbar_name">
        <h6>Alex Mora</h6>
        <p>Super Admin</p>
                    </div>
                    <img src="https://media.licdn.com/dms/image/C5603AQHXO62dyzbdTw/profile-displayphoto-shrink_800_800/0/1618510493844?e=2147483647&v=beta&t=VzX1Mx9gpNMwOypUVag9V-H7EyZTRYxkCTEYXHut_vM" alt="profile image"/>
                </div>
            </div>
        </div>  
    </div>
</template>
<script setup lang="ts">

</script>
<style scoped>
 .appbar{
    display: flex;
    align-items: center;
   flex: 1;
   width: 100%;
 
   justify-content: space-between;
   height: 80px;
   box-shadow: rgba(0, 0, 0, 0.1) 0px 1px 0px 0px;
 }   
 .appbar_profile_img>img{
width: 30px;
border-radius: 50%;
height: 30px;
 }
 .appbar_initials{
    display: flex;
    align-items: center;
 }
 .appbar_profile{
    display: flex;
    justify-content: space-between;
    margin-right: 10px;
 }
 .appbar_profile_img{
    display: flex;
    align-items: center;
 }
 .appbar_notification{
    display: flex;
    align-items: center;
    margin-right: 30px;
    padding: 3px;
    justify-content: center;
    width: 40px;
    height: 40px;
    border: 1px solid lightgrey;
    border-radius: 50%;
    margin-top: 15px;
 }
 .appbar_search{
    display: flex;
width: 500px;
align-items: center;
height: 40px;
background-color: rgba(241, 237, 237, 0.863);
margin-right: 20px;
border-radius: 30px;
padding: 3px;
 }
 .appbar_search>svg{
   margin-left: 10px;
 }
 .appbar_search>input{
width: 420px;
background-color: rgba(241, 237, 237, 0.863);
padding: 2px;
outline-width: 0;
border: none;
height: 20px;
margin-left: 10px;

 }
.appbar_notification>p{
width: 5px;
border-radius: 50%;
background-color: rgb(223, 175, 87);
height: 5px;
margin-left: -5px;

 }
 .appbar_name>p{
margin-top: -20px;
margin-right: 20px;
font-size: 10px;
 }
 .appbar_name>h6{
font-weight: bolder;
color:black;
  }
 .appbar_brand{
    flex: 0.4;
 }
 .appbar_initials{
    flex: 0.6;
 }
 .appbar_initials{
   display: flex;
   align-items: center;

 }
 .appbar_brand{
   margin: 10px;
 }

</style>