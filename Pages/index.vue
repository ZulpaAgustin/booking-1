<template>
  <div class="badan">
    <div class="login-container">
        <h2>Login</h2>
        <form id="loginForm">
            <div class="input-group">
                <input type="email" id="email" name="email" placeholder="Email" required>
                <i class="fas fa-envelope"></i>
            </div>

            <div class="input-group">
                <input type="password" id="password" name="password" placeholder="Password" required>
                <i class="fas fa-lock"></i>
            </div>
            <!-- <div class="col-md-4">
                <select aria-label="state"class="form-control form-control-lg form-select rounded-5 mb-2">
                  <option value="">Hak Akses</option>
                  <option value="admin">Admin</option>
                  <option value="user">User</option>
                </select>
              </div> -->
            <NuxtLink to="http://localhost:3000/bookings">
                <button type="submit">Login</button>
            </NuxtLink>
          </form>
            <p id="message"></p>
            <p class="daftar-link">Apakah Anda belum memiliki akun? <NuxtLink to="http://localhost:3000/akun">Daftar di sini</NuxtLink>
            </p>
        
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

.login-container {
    background-color: #8a4848;
    padding: 20px;
    border-radius: 20px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
    width: 300px;
}

h2 {
    text-align: center;
    color: #fff;
}

form {
    display: flex;
    flex-direction: column;
}

.input-group {
    position: relative;
    margin-bottom: 10px;
}

.input-group i {
    position: absolute;
    top: 50%;
    left: 10px;
    transform: translateY(-50%);
    color: #000000;
}

input {
    padding: 10px 10px 10px 30px; 
    border: 1px solid #ccc;
    border-radius: 20px;
    width: 100%;
    box-sizing: border-box; 
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
    color: red;
    text-align: center;
    margin-top: 10px;
}

.daftar-link {
    text-align: center;
    margin-top: 10px;
    color: #fff;
}

.daftar-link a {
    color: #4a0404;
    text-decoration: none;
}

.daftar-link a:hover {
    text-decoration: underline;
}

</style>
<script setup>
definePageMeta({
  layout: 'layoutBooking'
})

// import { ref } from "vue";

// let email = ref("")
// let password = ref("")

// const supabase = useSupabaseClient();

// const form = ref({
//     hakakses: ""
// });

// const kirimData = async () => {
//   // console.log(form.value);
//   const { error } = await supabase.from("login").insert([form.value]);
//   if (!error) navigateTo("/login");
// };
</script>