<template>
  <view class="container">
    <Button rounded dark :title="message" :on-press="handleBtnPress" />
    <todo-manager />
  </view>
</template>

<script>
import TodoManager from "./src/todoManager";
import { Container, Header, Content, Button, Text } from 'native-base';
export default {
  components: { TodoManager },
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
