<script setup>
import { ref } from 'vue';

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count += 2">count is {{ count }}</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p>
    Install
    <a href="https://github.com/johnsoncodehk/volar" target="_blank">Volar</a>
    in your IDE for a better DX
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>

<style scoped type="text/css">
.wrapper {
  background: #fff;
  .footer {
    color: #666;
    text-align: center;
    margin-top: 150px;
    width: 100%;
    span {
      color: #1e90ff;
      cursor: pointer;
    }
  }

  .login {
    .top {
      margin: 20% 0 0 8%;
      font-size: 26px;
      span {
        margin-left: 20px;
        position: relative;
        bottom: 5px;
        color: #666;
      }
    }

    .form {
      margin: 10% 8% 0 8%;
      input {
        font-family: 'Microsoft Yahei';
        width: 100%;
        &.btn {
          line-height: 32px;
          background: #1e90ff;
          color: white;
          margin-top: 50px;
        }
      }
      a {
        margin-top: 20px;
        color: #1e90ff;
      }
      ::-webkit-input-placeholder,
      ::-moz-placeholder,
      ::-moz-placeholder,
      ::-ms-input-placeholder {
        color: #333;
      }
    }
  }
}
</style>
