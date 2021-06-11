<template>
    <!-- need to have .prevent because there is no serve to post a callback-->
    <form @submit.prevent="onSubmit">
        <label for="new-todo-input">
            What needs to be done?
        </label>
        <input
            type="text"
            id="new-todo-input"
            name="new-todo"
            autocomplete="off"
        />
        <button type="submit">
            Add
        </button>
    </form>
</template>

<script>
  export default {
      methods: {
          onSubmit() {
              console.log('form submitted')
          }
      }
  };
</script>