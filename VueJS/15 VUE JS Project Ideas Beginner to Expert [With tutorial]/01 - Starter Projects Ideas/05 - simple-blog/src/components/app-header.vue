<template>
  <header>
    <slot></slot>
  </header>
</template>

<style lan="scss" scoped>
header {
  position: relative;
  height: 250px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url(../assets/header-bg.jpg);
  background-size: cover;
}

header::before {
  content: "";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;

  opacity: 0.95;
  background: -webkit-linear-gradient(
    -45deg,
    #330033 0%,
    #333366 100%
  ); /* Chrome10-25,Safari5.1-6 */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#330033', endColorstr='#333366',GradientType=1 ); /* IE6-9 fallback on horizontal gradient */
}

h1 {
  position: relative;
  margin: 0;
  color: #fff;
  font-weight: 300;
  font-size: 60px;
}
.back-button{
    color: #fff;
    text-decoration: none;
    position: absolute;
    top: 20px;
    left: 20px;
    background-color: rgba(255,255,255,0.1);
    border-radius: 5px;
    padding: 7px 15px;
    line-height: 1;
    
  }
  .back-button:hover{
      background-color: rgba(255,255,255,0.2);
    }
</style>

<script>
export default {};
</script>
