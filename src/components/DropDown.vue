<template>
  <dropdown
    title="Simple Filter"
    text="Click to filter"
    :items="[
    {text: 'Item 1'},
    {text: 'Item 2'}
  ]"
  ></dropdown>
</template>

<script>
export default {
  name: "DropDown",
  props: ["title", "items"]
};
</script>

<style>
nav .menu-item svg {
  width: 10px;
  margin-left: 10px;
}

nav .menu-item .sub-menu {
  position: absolute;
  background-color: #222;
  top: calc(100%+ 18px);
  left: 50%;
  transform: translateX(-50%);
  width: max-content;
  border-radius: 0px 0px 16px 16px;
}
</style>