<template>
  <div class="home">
    <div class="flex flex-col justify-center items-center h-home">
      <h1 class="text-center text-9xl font-black text-black">
        VALENTIN<br>ENGELHARD
      </h1>
      <h2 class="text-center text-5xl font-bold text-gray-900">Développeur Web Fullstack Junior</h2>
    </div>
    <div class="h-32">

    </div>
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.h-home {
  height: 80vh;
}

body {
  background-color: #111;
}

.arrow {
  transform: rotate(90deg);
  cursor: pointer;
  height: 120px;
  left: 50%;
  position: absolute;
  top: 50%;
  transform: translateX(-50%) translateY(-50%);
  transition: transform .1s;
  width: 80px;
  
  $transition-time: .15s;
  
  &-top,
  &-bottom {
    background-color: #666;
    height: 4px;
    left: -5px;
    top: 50%;
    width: 100%;
    
    &:after {
      background-color: #fff;
      content: '';
      height: 100%;
      position: absolute;
      top: 0;
      transition: all $transition-time;
    }
  }
  
  &-top {
    transform: rotate(135deg);
    transform-origin: bottom right;
    
    &:after {
      left: 100%;
      right: 0;
      transition-delay: 0s;
    }
  }
  
  &-bottom {
    transform: rotate(45deg);
    transform-origin: top right;
    
    &:after {
      left: 0;
      right: 100%;
      transition-delay: $transition-time;
    }
  }
  
  &:hover & {
    
    &-top:after {
      left: 0;
      transition-delay: $transition-time;
    }

    &-bottom:after {
      right: 0;
      transition-delay: 0s;
    }
  }
  
  &:active {
    transform: translateX(-50%) translateY(-50%) scale(0.9);
  }
}
</style>
