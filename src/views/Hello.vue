<template>
  <div>
    <h1>Hello World! This is a new route</h1>
    <MyFirstComponent v-if="showFirst"/>
    <ButtonComponent v-else />
    <p>{{ message }}</p>
    <p>{{ reversedMessage }}</p>
    <ListComponent />
  </div>
</template>

<script>
import MyFirstComponent from "@/components/MyFirstComponent";
import ButtonComponent from "@/components/ButtonComponent";
import ListComponent from "@/components/ListComponent";

export default {
  name: "Hello",
  data: function() {
    return {
      count: 0,
      message: "lets learn vue",
      showFirst: false
    };
  },
  components: {
    MyFirstComponent,
    ButtonComponent,
    ListComponent
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
