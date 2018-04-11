<template>
  <div>
      <form @submit.prevent="addTodo()">
          <label for="newTodo">New Todo</label>
          <input type="test" name="newTodo" id="newTodo">
          <button type="submit" name="button">Add Todo</button>
      </form> 
      <ul>
          <li v-for="todo in todos" :key="todo">{{todo}}</li>
      </ul>      
  </div>
</template>

<script>
export default {
    data() {
        return {
            newTodo: '',
            todos: [],
            todoToAdd: '',
        }
    },
      methods: {
          addTodo(){
              this.todos.push(this.todoToAdd)
              console.log(this.todos)
          }
      }
}
</script>

<style>
