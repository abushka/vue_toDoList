<template>
  <form @submit.prevent="onSubmit">
    <input id="input" type="text" v-model="title" placeholder="Enter your plans">
    <button type="submit">Create</button>
  </form>
</template>

<script>
export default {
  data() {
    return {
      title: ''
    }
  },
  methods: {
    onSubmit() {
      if (this.title.trim()) {
        const newTodo = {
          id: Date.now(),
          title: this.title,
          completed:false
        }
        this.$emit('add-todo', newTodo)
        this.title = ''
      }
    }
  }
}
</script>

<style scoped>
  form {
    /*display: flex;*/
    /*flex-direction: row;*/
    /*justify-content: center;*/
    position: relative;
    padding-top: 0.6rem;
  }
  input {
    width: 400px;
    height: 20px;
    margin-right: 2px;
  }
  button {
    height: 26px;
    width: 80px;
    color: #000;
    background: aquamarine;
    border: none;
    border-radius: 4px;
    outline: none;
    cursor: pointer;

  }
  button:hover {
    background: aqua;
    transform: translateY(-1px);
  }
  button:active {
    transform: translateY(0);
  }

</style>