<template>
  <div class="register hero">
    <div class="field">
      <label class="label is-pulled-left">Name</label>
      <div class="control">
        <input class="input" type="text" placeholder="Enter your name">
      </div>
    </div>
    <div class="field">
      <label class="label is-pulled-left">Username</label>
      <div class="control has-icons-left">
        <span class="icon is-small is-left">
          <i class="fas fa-user"></i>
        </span>
        <input class="input" type="text" placeholder="Enter Username">
      </div>
    </div>
    <div class="field">
      <label class="label is-pulled-left">E-Mail</label>
      <div class="control has-icons-left">
        <span class="icon is-small is-left">
          <i class="fas fa-envelope"></i>
        </span>
        <input class="input" type="email" placeholder="Enter a valid E-Mail">
      </div>
    </div>

    <div class="field">
      <label class="label is-pulled-left">Password</label>
      <div class="control has-icons-left">
        <span class="icon is-small is-left">
          <i class="fas fa-lock"></i>
        </span>
        <input class="input" type="password" :value="password" placeholder="Enter Password">
      </div>
    </div>
    <div class="field is-grouped">
      <div class="control">
        <label class="checkbox">
          <input type="checkbox">
          I agree to the
          <a href="#">terms and conditions</a>
        </label>
      </div>
      <div class="control">
        <button class="button is-link">Register</button>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({})
export default class Register extends Vue {
  name: string = "";
  username: string = "";
  email: string = "";
  password: string = "";
}
</script>

<style lang="css" scoped></style>
