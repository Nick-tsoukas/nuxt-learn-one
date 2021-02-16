<template>
  <div class="container">
    {{ message }}
    <div>
      <label for="goals">Goals</label>
      <input type="text" v-model="enteredValue">
      <button v-on:click="addGoal">Add Goals</button>
    </div>
    <ul>
      <li v-for="goal in goals" v-bind:key="goal">{{goal}}</li>
    </ul>
  </div>
</template>

<script>
export default {
   data() {
      return {
        goals: [],
        enteredValue: '',
        message: 'hello this is a message'
      }
    },
     medthods: {
      addGoal() {
        this.goals.push(enteredValue) 
      }
    }
   
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

</style>
