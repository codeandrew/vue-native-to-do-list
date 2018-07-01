<template>
  <view class="container">
    <Button :title="message" :on-press="handleBtnPress" />
  </view>
</template>

<script>
export default {
  data : function(){
    return {
      message :  "Vue Native Button"
    }
  },

  methods: {
    handleBtnPress : function() {
      alert('Btn Press');
    }
  }
}
</script>

<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: blue;
}
</style>
