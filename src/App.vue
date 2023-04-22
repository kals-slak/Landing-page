<!-- <template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view/>
</template> -->
<template>
  <el-menu
    :default-active="activeIndex"
    class="el-menu-demo"
    mode="horizontal"
    :ellipsis="false"
    @select="handleSelect"
  >
  <div class="nav">

    <el-menu-item class="logo" index="0">
      <img src="../src/assets/sidepash.png">
      <h2>SIDEPASH</h2>
    </el-menu-item>
    <div class="navLinks">
      <el-menu-item index="1"><li>Home</li></el-menu-item>
      <el-menu-item index="2"><li>Services</li></el-menu-item>
      <el-menu-item index="3"><li>Culture</li></el-menu-item>
    </div>
    <div class="reachContainer">
      <button class="reach">Reach us</button>
    </div>
    <div class="burger">
      <a @click="toggle" ><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Hamburger_icon_white.svg/1024px-Hamburger_icon_white.svg.png"></a>
    </div>
  </div>
   <div class="burgerLinks">
      <el-menu-item index="1"><h4>Home</h4></el-menu-item>
      <el-menu-item index="2"><h4>Services</h4></el-menu-item>
      <el-menu-item index="3"><h4>Culture</h4></el-menu-item>
      <button class="reach">Reach us</button>
   </div>    
  </el-menu>
  <router-view/>
</template>

<script setup>
import { ref } from 'vue';
const activeIndex = ref('1');
const handleSelect = (key, keyPath) => {
  console.log(key, keyPath);
}
const toggle = ()=>{
  let burgerlinks= document.getElementsByClassName("burgerLinks")[0];
  if(burgerlinks.style.display=='block'){
    burgerlinks.style.display= 'none';
  }
  else{
    burgerlinks.style.display= 'block';
  }
}
</script>

<style lang="scss">

*{
  margin: 0;
  padding: 0;
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
} 

li,h2{
  color: white;
}
a { 
  text-decoration: none; 
}

img{
  width: 50px;
  height: 50px;
}
 
.el-menu.el-menu--horizontal {
  border-bottom: none !important;
}

.logo{
  
  display: flex;
  align-items: center;
}

.reachContainer{
  margin-right: 4%;

}

.reach {
  background-image: linear-gradient(to right, #00c6ff 0%, #0072ff  51%, #00c6ff  100%);
  margin: 10px;
  text-align: center;
  padding: 10px 15px;
  background-size: 200% auto;
  transition: 0.5s;
  color: white;            
  display: block;
  border-radius: 5px;
  border: none;
}        

.nav {
  display: flex;
  justify-content: space-between;
  background-color: #131A2C;
  
}

.navLinks{
    display: flex;
}

.burger{
  display: none;
}

.burgerLinks{
  display: none;
}

@media only screen and (max-width:600px){
  .navLinks{
    display: none;
  }
  .burger{
    display: block;
  }
  .reachContainer{
    display: none;
  }
  .el-menu-item.logo{
    padding: 0;
  }
}


</style>


