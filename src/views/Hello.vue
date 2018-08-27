
<template>
  <div>
    <h1>Hello World! This is a new route</h1>
    <MyFirstComponent/>
    <ButtonComponent/>
    <p>{{ message }}</p>
    <p>{{ reversedMessage }}</p>
  </div>
</template>

<script>
import MyFirstComponent from "@/components/MyFirstComponent";
import ButtonComponent from "@/components/ButtonComponent";

export default {
  data: function() {
    return {
      count: 0,
      message: "lets learn vue"
    };
  },
  components: {
    MyFirstComponent,
    ButtonComponent
  },
  computed: {
    reversedMessage: function() {
      return this.message
        .split("")
        .reverse()
        .join("");
    }
  }
};
</script>
