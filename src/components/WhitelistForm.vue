<script setup lang="ts">
import { ref } from 'vue'

const email = ref('')
const showPopup = ref(false)

const submitForm = () => {
  // Simulate sending email to backend
  console.log('Submitted email:', email.value)
  
  // Simulate sending notification email
  console.log('Sending notification to backtechuk@gmail.com')
  console.log('New subscriber:', email.value)

  showPopup.value = true
  email.value = ''

  // Hide popup after 3 seconds
  setTimeout(() => {
    showPopup.value = false
  }, 3000)
}
</script>

<template>
  <div class="whitelist-form">
    <h3>Join Our Whitelist</h3>
    <p>Subscribe to get a free pass for our inauguration and stay updated!</p>
    <form @submit.prevent="submitForm">
      <input 
        type="email" 
        v-model="email" 
        placeholder="Enter your email" 
        required
      >
      <button type="submit">Subscribe</button>
    </form>
    <div v-if="showPopup" class="popup">
      <p>Thank you for subscribing!</p>
    </div>
  </div>
</template>

<style scoped>
.whitelist-form {
  background-color: #f9f9f9;
  padding: 40px;
  text-align: center;
  margin: 40px 0;
  position: relative;
}

form {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

input[type="email"] {
  padding: 10px;
  width: 300px;
  border: 1px solid #ddd;
}

button {
  padding: 10px 20px;
  background-color: #4CAF50;
  color: white;
  border: none;
  cursor: pointer;
}

.popup {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-color: #4CAF50;
  color: white;
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
  z-index: 1000;
}
</style>