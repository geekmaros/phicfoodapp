<template>
<section class="masthead" role="img" aria-label="Image Description">
  <h1>
    Phic Food App
  </h1>
    <button>
      See Restaurants >
    </button>
</section>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.masthead {
  width: 100%;
  height: 80vh; 
  overflow: hidden;
  background-size: cover !important;
    padding: 40px;
  background: radial-gradient(ellipse at center, rgba(0,0,0,0) 0%, rgba(0,0,0,0) 48%, rgba(0,0,0,0.65) 100%), url('~/assets/headerimg.jpg') no-repeat center center scroll;
}

h1 {
  font-style: normal;
  font-weight: bold;
  color: #eee;
  font-size: 8vmin;
 
  letter-spacing: 0.03em;
  line-height: 1;
  text-shadow: 1px 2px 4px rgba(0, 0, 0, 0.8);
  margin-bottom: 20px;
}
    
      

    
</style>


    