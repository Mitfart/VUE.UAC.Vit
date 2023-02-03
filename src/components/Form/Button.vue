<template>
  <a href="#" class="btn"> Создать </a>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Button",
  props: {
    ['text']
  },

}
</script>

<style scoped lang="scss">

.btn {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;

  background-color: $c-primal-c;
  color: $c-primal;

  padding: .75rem 1.5rem;
  border-radius: 1000rem;

  cursor: pointer;
  &:hover {
    background-color: $c-primal;
    color: $c-base;
  }

  &_active {
    background-color: $c-primal-c;
    color: $c-primal;
  }
}
</style>