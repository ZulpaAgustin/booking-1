<template>
  <div class="badan">
    <div class="container">
        <h2>Daftar Akun</h2>
        <form id="signupForm">
            <div class="input-group">
                <i class="fas fa-user"></i>
                <input type="text" id="username" name="username" placeholder="Username" required>
            </div>
            <div class="input-group">
                <i class="fas fa-envelope"></i>
                <input type="email" id="email" name="email" placeholder="Email" required>
            </div>
            <div class="input-group">
                <i class="fas fa-phone"></i>
                <input type="tel" id="phone" name="phone" placeholder="No Handphone" required>
            </div>
            <div class="input-group">
                <i class="fas fa-lock"></i>
                <input type="password" id="password" name="password" placeholder="Password" required>
            </div>
            <NuxtLink to="http://localhost:3000/bookings">
                <button type="submit">Daftar</button>
            </NuxtLink>
            
        </form>
        <p id="message"></p>
        <p class="login-link">Sudah memiliki akun? <NuxtLink to="/">Login</NuxtLink>
          <!-- <a href="login.html"></a> --></p>
      </div>
    </div>
</template>

<style scoped>
.badan {
    font-family: Georgia, 'Times New Roman', Times, serif;
    background-color: #958686;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
}

.container {
    background-color: #8a4848;
    padding: 20px;
    border-radius: 20px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    width: 300px;
}

h2 {
    text-align: center;
    color: #fff;
}

.input-group {
    position: relative;
    margin-bottom: 15px;
}

.input-group i {
    position: absolute;
    top: 10px;
    left: 10px;
    color: #000000;
}

.input-group input {
    width: 100%;
    padding: 8px 8px 8px 30px;
    box-sizing: border-box;
    border: 1px solid #ccc;
    border-radius: 20px;
}

input::placeholder {
    color: #161718c0;
}

button {
    width: 100%;
    padding: 10px;
    background-color: #7f3333;
    color: white;
    border: none;
    border-radius: 20px;
    cursor: pointer;
    font-size: 16px;
}

button:hover {
    background-color: #601717;
}

#message {
    text-align: center;
    color: red;
    margin-top: 15px;
}


.login-link {
    text-align: center;
    margin-top: 10px;
    color: #fff;
}

.login-link a {
    color: #4a0404;
    text-decoration: none;
}

.login-link a:hover {
    text-decoration: underline;
}
</style>

<script setup>
definePageMeta({
  layout: 'layoutBooking'
})
</script>