<template>
  <router-view/>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

*{
    margin: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
    
}

:root{
  --black:black;
  --white:white;

  --bgnavigation: rgba(0, 29, 102, 0.2);

  --main:rgb(0, 29, 102);
  --secondary:rgba(102, 0, 0, 1);

  --bgprice: rgba(0, 29, 102, 0.48);
  --bgbtn: rgba(193, 0, 0, 0.3);
    
}

  #rtext{
    color: var(--main);
  }

  #btext{
    color:var(--main);
  }

#app {
  font-family: Poppins, sans-serif;

}

#ntext{
text-align: center;
width: 34px;
height: 32px;
border: 1.5px solid #001D66;
border-radius: 6px;
}

</style>