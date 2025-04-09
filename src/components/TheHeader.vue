<template>
  <div class="ui vertical masthead center aligned" id="header">
    <div id="header-content">
      <img src="../assets/img/logo.png" alt="/">
      <p>{{ subHeader }}</p>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'TheHeader',
  setup() {
    const { header, subHeader } = window.__PRE_CONFIG__;
    return {
      header, subHeader
    };
  }
});
</script>
<style>
#header {
  height: 25rem;
  position: relative;
  /*Replace your header image at this place!*/
  /* background: url("../assets/img/cover.jpg") no-repeat center; */
  /* background-size: cover; */
}

#header::after {
  content: 'マジカルミライ 2025';
  position: absolute;
  right: 15px;
  bottom: 0;
  z-index: 2;
  color: #05f4fc;
  text-shadow: 1px 1px 1px #666;
}

#header-content {
  position: absolute;
  z-index: 3;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-shadow: 2px 2px 2px #666;
  text-align: center;
}

#header h1 {
  font-size: 3.57rem;
  white-space: nowrap;
}

#header p {
  font-size: 1.5rem;
  color: aliceblue;
}

img {
  width: 450px;
}

@media screen and (max-width:768px) {
  img {
    width: 350px;
  }
}
</style>
