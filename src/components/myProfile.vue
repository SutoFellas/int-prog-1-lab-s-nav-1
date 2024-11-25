<template>
    <section v-if="isLoggedin">
<div style="background-color: blue; 
text-align: center; 
color: white;
font-style: italic;">
<h1>
    BlogBook
</h1>
</div>
<div style="text-align: center;">
    <img src="../assets/profile-foto.jpg" width="200px">
</div>
<div style="text-align: center;
font-style: italic;">
    <li>Süleyman Gürbüz (22)</li>
</div>

<div style="text-align: center; 
color: blue;
font-style: italic;">
    <button onclick="yeniBlog()">
        Yeni Blog Yaz+
    </button><br></div>
    <div>
    
    <v-text-field></v-text-field>
    
    
    </div>

<div style="text-align: center; 
color: blue; 
background-color: cornflowerblue;">
    <button onclick="yaz()">Yaz+</button>
</div>


</section>
<section v-else>
   <div style="background-color: blue; 
   text-align: center; 
   color: white;
   font-style:italic;">
    <h1>BlogBook</h1></div> 
    <div style="text-align: center;">
        <h2>Kullanıcı Adı</h2>
    </div>
    <div>
        <v-text-field></v-text-field>
    </div>
    <div>
        <h2 style="text-align: center;">Şifre</h2>
    </div>
    <div>
        <v-text-field></v-text-field>
    </div>
    <div style="text-align: center; color:green;">
        <button onclick="giris()">Giriş</button>
    </div>
    <div>hocam ref i false yapınca login pageye gider</div>

</section>
</template>
<script setup>
import {ref} from "vue"

var isLoggedin = ref()
var isLoggedin = ref(true)

</script>