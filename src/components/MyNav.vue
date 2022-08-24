<template>
 <nav class="navbar navbar-light mb-5">
          <div class="container-fluid mx-5 mt-5">
            <router-link to="/" class="navbar-brand fw-bold fs-3" id="navlogo">{{logo}}</router-link>
            <div class="d-flex">
             <router-link to="/pricelist">
              <button
                class="btn rounded-pill"
                id="plist"
                type="submit"
              >
                Pricelist
              </button>
              </router-link> 
            
              <div class="container-fluid fixed-top mt-5 me-5" style="mix-blend-mode: difference; width: fit-content;">
                <div class="toggle">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>       
              </div>
            </div>
          </div>
    </nav>

        <div class="sidebar">
          <ul class="navigation">
            
          <li><router-link to="/pricelist" data-text="Pricelist">Pricelist</router-link></li>
          <li><router-link to="/photography" data-text="Photography">Photography</router-link></li>
          <li><router-link to="/editing" data-text="Editing">Editing</router-link></li>
          <li><router-link to="/design" data-text="Design">Design</router-link></li>
          <li><router-link to="/printing" data-text="Printing">Printing</router-link></li>
          <div class="navfooter">
            <hr>
            <li class="navmail"><a href="#"><u>View Email</u> </a></li>
            <li class="navnum"><a href="#">+62 831 3483-1328</a></li>
          </div>

          </ul>
         
        </div>
</template>

<script>
export default {
  name: 'MyNav',
  props: {
    logo: String,
  },
  mounted(){
      let menutoggle = document.querySelector(".toggle");
      let navigation = document.querySelector(".navigation");
      let sidebar = document.querySelector(".sidebar");
      let navlogo = document.querySelector("#navlogo");
      let plist = document.querySelector("#plist");

    menutoggle.onclick = function () {
    menutoggle.classList.toggle("active");
    navigation.classList.toggle("active");
    sidebar.classList.toggle("active");
    navlogo.classList.toggle("active");
    plist.classList.toggle("active");
    }
  } 
}

</script>

<style>

@keyframes fadein {
  0%,50% { opacity: 0 }
  100% { opacity: 1 }
}

#navlogo {
transition: 0.5s;
}

#navlogo.active {
animation: fadein 0.5s linear;
z-index: 20000;

position: fixed;
}

#plist{
  padding: 10px 17px;
  margin-right: 70px; 
  z-index: 1; 
  color:var(--main); 
  background: var(--bgprice);
  transition: 0.5s; 

}

#plist:hover{
  color: var(--white); 
  background: var(--main); 
}

#plist.active{
  opacity: 0;
  transition: 0s;
}

.toggle {

    margin-top: 12px;
    position: relative;
    float: right;
    width: 40px;
    height: 40px;
    justify-content: center;
    align-items: center;
    display: flex;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.02);
    background: transparent;
    cursor: pointer;
    overflow: hidden;
    z-index: 20000;
  }
  
.toggle span {
    position: absolute;
    width: 30px;
    height: 2.4px;
    background: var(--white);
    border-radius: 3px;
    transition: 0.5s;
  }
  
.toggle span:nth-child(1) {
    transform: translateY(-9px);
    width: 15px;
    left: 5px;
}
  
.toggle.active span:nth-child(1) {
    width: 25px;
    transform: translateY(0px) rotate(45deg);
    transition-delay: 0.125s;
}
  
.toggle span:nth-child(2) {
    transform: translateY(9px);
    width: 15px;
    left: 5px;
}
  
.toggle.active span:nth-child(2) {
    width: 25px;
    transform: translateY(0px) rotate(315deg);
    transition-delay: 0.25s;
}
  
.toggle.active span:nth-child(3) {
    transform: translateX(60px);
}

.navigation {
    position: fixed;
    top: 0;
    padding-left: 5%;
    right: -100%;
    width: 30%;
    height: 100%;
    display: flex;
    background: var(--white);
    justify-content: center;
    align-items: left;
    flex-direction: column;
    z-index: 4;
    transition: 1s;
    visibility: hidden;
    cursor: pointer;
    min-width: 300px;
   
}

  
.navigation.active {
    
    visibility: visible;
    right: 0%;

}

.sidebar.active{
    position: fixed;
    top: 0;
    width: 100%;
    height: 100%;
    background: var(--bgnavigation);
    z-index: 2;
    animation: fadein 0.5s linear;
    
}
  

.navigation li {
    list-style: none;
}
  
.navigation li a {
    position: relative;
    display: block;
    margin: 5px 0;
    font-size: 2em;
    text-decoration: none;
    color: transparent;
    padding: 5px 20px;
    border-radius: 40px;
    -webkit-text-stroke: 0.9px var(--black);
    font-weight: bolder;
    letter-spacing: 2px;
    line-height: 1.2em;
}
  
.navigation li a:before {
    content: attr(data-text);
    position: absolute;
    transition: 0.5s;
}
  
.navigation li a:after {
    top: 0;
    left: 23px;
    content: attr(data-text);
    position: absolute;
    transition: 0.5s;
    visibility: hidden;
    transition: none;
}
  
.navigation li a:hover {
    color: var(--white);
    -webkit-text-stroke: 00.9px var(--black);
    transition: 0.5s;
}
  
.navigation li a:hover:before {
    color: red;
    -webkit-text-stroke: 00.9px var(--black);
    z-index: 5;
    transform: translate(3px, -3px);
}
  
.navigation li a:hover:after {
    color: cyan;
    -webkit-text-stroke: 00.9px var(--black);
    z-index: 6;
    transform: translate(3px, -3px);
    visibility: visible;
    transition: 0.5s;
}

.navigation .navfooter li a {
    font-size: 16px;
    -webkit-text-stroke: 0;
    letter-spacing: 1px;
}

.navigation .navfooter .navnum a {
    color: var(--main);
}

.navigation .navfooter .navmail a {
    color: red;
}

.navigation .navfooter .navmail a:hover {
    color: var(--main);
}

#numtext{
    color: var(--main);
}

#mailtext{
    color:var(--secondary);
}
</style>