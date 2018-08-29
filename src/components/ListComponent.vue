<template>
  <div>
    <p v-for="(item, index) in myList" :key="item.id">
      {{ index }}. {{ item }}
    </p>
    <p v-for="(item, key, index) in myObject" :key="item.id">
      {{ index }}. {{ key }} {{ item }}
    </p>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      myList: ["fluffykins", "billy", "steven", "george"],
      myObject: {
        firstName: "John",
        lastName: "Doe",
        age: 30
      }
    };
  }
};
</script>
