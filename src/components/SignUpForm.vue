<template>
  <form action="">
    <label for="email">Email</label>
    <input type="email" v-model="email" required>

    <label for="password">Password</label>
    <input type="password" v-model="password" required>

    <label for="role">Role</label>
    <select name="" id="" v-model="role" required>
        <option value="developer">Web developer</option>
        <option value="designer">Web designer</option>
    </select>

    <input type="checkbox" v-model="terms" required>
    <label for="terms">I accept the terms and conditions</label>
  </form>
  <p>Email: {{email}}</p>
  <p>Password: {{password}}</p>
  <p>Role: {{role}}</p>
  <p>Terms: {{terms}}</p>
</template>

<script>
export default {
    data(){
        return{
            email:'',
            password:'',
            role:'',
            terms:false
        }
    }
}
</script>

<style>

</style>