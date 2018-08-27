
<template>
  <div>
    <h1>Hello World! This is a new route</h1>
    <MyFirstComponent/>
    <ButtonComponent/>
  </div>
</template>

<script>
import MyFirstComponent from "@/components/MyFirstComponent";
import ButtonComponent from "@/components/ButtonComponent";

export default {
  data: function() {
    return {
      count: 0
    };
  },
  components: {
    MyFirstComponent,
    ButtonComponent
  }
};
</script>

