<template>
  <div class="login-container">
    <div class="login-form">
      <div class="login-logo">
        <img src="../assets/logo.svg" alt="Golden Connect" />
        <h1>Golden Connect</h1>
      </div>
      
      <div class="elderly-image">
        <img src="https://images.unsplash.com/photo-1524601500432-1e1a4c71d33d?q=80&w=3174&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Happy seniors enjoying life" />
      </div>
      
      <h2>WELCOME BACK!</h2>
      <p class="subtitle">Please enter your login details.</p>
      
      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" placeholder="Enter your email" class="input-field">
      </div>
      
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" placeholder="••••••••••" class="input-field">
      </div>
      
      <div class="remember-forgot">
        <div class="remember">
          <input type="checkbox" id="remember" />
          <label for="remember">Remember me</label>
        </div>
        <a href="#" class="link">Forgot password?</a>
      </div>
      
      <button class="btn" @click="goToHome">Sign in</button>
      
      <div class="google-signin">
        <button class="google-btn">
          <img src="../assets/google.svg" alt="Google" />
          Sign in with Google
        </button>
      </div>
      
      <div class="login-link">
        <p>Don't have an account? <router-link to="/" class="link">Sign up</router-link></p>
      </div>
    </div>
    
    <div class="login-image">
      <img src="https://images.unsplash.com/photo-1575267685965-20e1354939e7?q=80&w=3270&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Happy seniors connecting" />
      <div class="logo-overlay">
        <img src="../assets/logo.svg" alt="Golden Connect" />
        <span>Golden Connect</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SignInView',
  methods: {
    goToHome() {
      this.$router.push('/home')
    }
  }
}
</script>

<style scoped>
.login-container {
  display: flex;
  height: 100vh;
}

.login-form {
  flex: 1;
  padding: 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  max-width: 500px;
  margin: 0 auto;
}

.login-logo {
  display: none;
}

.elderly-image {
  margin-bottom: 30px;
  border-radius: 10px;
  overflow: hidden;
  display: block;
}

.elderly-image img {
  width: 100%;
  border-radius: 10px;
}

h2 {
  font-size: 32px;
  margin-bottom: 10px;
  color: #1D7C40;
}

.subtitle {
  color: #666;
  margin-bottom: 30px;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  margin-bottom: 8px;
  font-weight: bold;
}

.remember-forgot {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

.remember {
  display: flex;
  align-items: center;
}

.remember input {
  margin-right: 8px;
}

.remember label {
  margin-bottom: 0;
  font-weight: normal;
}

.google-signin {
  margin-top: 20px;
}

.google-btn {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 5px;
  background-color: white;
  cursor: pointer;
}

.google-btn img {
  width: 20px;
  margin-right: 10px;
}

.login-link {
  margin-top: 20px;
  text-align: center;
}

.login-image {
  flex: 1;
  position: relative;
  display: none;
}

.login-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.logo-overlay {
  position: absolute;
  top: 20px;
  right: 20px;
  display: flex;
  align-items: center;
  color: white;
  font-weight: bold;
  font-size: 18px;
}

.logo-overlay img {
  width: 30px;
  height: 30px;
  margin-right: 10px;
}

@media (min-width: 768px) {
  .login-image {
    display: block;
  }
  
  .elderly-image {
    display: none;
  }
}

@media (max-width: 767px) {
  .elderly-image {
    display: block;
  }
}
</style> 