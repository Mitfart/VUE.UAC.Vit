<template>
  <label class="header__search search">
    <input type="text" class="search__field" placeholder="Найти пост или пользователя...">

    <button class="search__btn" type="button">
      <svg class="icon icon_loupe" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
      </svg>
    </button>
  </label>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Search"
}
</script>

<style scoped lang="scss">
  .search {
    background-color: $c-base-c;

    display: flex;
    justify-content: space-between;

    border: .125rem solid transparent;
    border-radius: 1000rem;
    overflow: hidden;

    opacity: 50%;


    &__field,
    &__btn {
      padding: .5rem 1rem;
      border: none;
    }

    &__field {
      width: 100%;
    }
    &__btn {
      display: flex;
      align-items: center;
      gap: 1rem;

      &:hover > .icon {
        color: $c-primal;
      }
    }


    &:hover,
    &:focus-within {
      border-color: $c-primal;
      background-color: $c-base;
      opacity: 100%;
    }
  }
</style>