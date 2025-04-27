<template>
  <div class="home-page">
    <header class="header">
      <div class="container header-content">
        <div class="logo">
          <img src="../assets/logo.svg" alt="Golden Connect" />
          <span>Golden Connect</span>
        </div>
        <div class="search-bar">
          <div class="search-icon">
            <img src="../assets/search-icon.svg" alt="Search" />
          </div>
          <input type="text" placeholder="Search" />
        </div>
        <div class="user-actions">
          <button class="logout-btn" @click="goToLogin">Logout</button>
          <div class="profile-icon">
            <img src="https://images.unsplash.com/photo-1559087867-ce4c91325525?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Profile" />
          </div>
        </div>
      </div>
    </header>

    <main class="main-content container">
      <div class="profile-sidebar">
        <div class="profile-header">
          <div class="profile-bg">
            <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?q=80&w=2073&auto=format&fit=crop" alt="Background" />
          </div>
          <div class="profile-avatar">
            <img src="https://images.unsplash.com/photo-1559087867-ce4c91325525?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Robert Fox" />
          </div>
          <div class="profile-info">
            <h2>Robert Fox</h2>
            <p class="username">User id: @Robert_1958</p>
            <p class="bio">I love to get connected with people.... because you've gotta make use of life ...</p>
          </div>
        </div>
        
        <nav class="profile-nav">
          <ul>
            <li class="active"><router-link to="/home"><img src="../assets/home-icon.svg" alt="Home" /> Home</router-link></li>
            <li><img src="../assets/profile-icon.svg" alt="Profile" /> Profile</li>
            <li><router-link to="/messages"><img src="../assets/messages-icon.svg" alt="Messages" /> Messages</router-link></li>
            <li><img src="../assets/notifications-icon.svg" alt="Notifications" /> Notifications</li>
          </ul>
        </nav>
      </div>
      
      <div class="feed">
        <div class="feed-tabs">
          <button class="tab active">My Posts</button>
          <button class="tab">Saved Posts</button>
          <button class="tab">Settings</button>
        </div>
        
        <div class="stats">
          <div class="stat-box">
            <span class="stat-number">12</span>
            <span class="stat-label">Posts</span>
          </div>
          <div class="stat-box">
            <span class="stat-number">207</span>
            <span class="stat-label">Followers</span>
          </div>
          <div class="stat-box">
            <span class="stat-number">64</span>
            <span class="stat-label">Following</span>
          </div>
        </div>
        
        <div class="post">
          <div class="post-header">
            <img src="https://images.unsplash.com/photo-1566616213894-2d4e1baee5d8?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Bessie Cooper" class="post-avatar" />
            <div class="post-info">
              <h3>Bessie Cooper</h3>
              <p class="post-username">@Bessiecooper1960</p>
            </div>
            <div class="post-time">7 hours ago</div>
            <div class="post-actions">...</div>
          </div>
          <div class="post-content">
            <p>Now I am very happy that I can meet my grandchildren after a long time.</p>
          </div>
          <div class="post-actions">
            <button class="action-btn"><img src="../assets/comment-icon.svg" alt="Comment" /> Comment</button>
            <button class="action-btn"><img src="../assets/like-icon.svg" alt="Like" /></button>
          </div>
        </div>
        
        <div class="post">
          <div class="post-header">
            <img src="https://images.unsplash.com/photo-1522075469751-3a6694fb2f61?q=80&w=2080&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Jonathan Jones" class="post-avatar" />
            <div class="post-info">
              <h3>Jonathan Jones</h3>
              <p class="post-username">@Jonathanj1950</p>
            </div>
            <div class="post-time">1 day ago</div>
            <div class="post-actions">...</div>
          </div>
          <div class="post-content">
            <p>I had a wonderful picnic with my family!!</p>
            <div class="post-image">
              <img src="https://images.unsplash.com/photo-1529333166437-7750a6dd5a70?q=80&w=2069&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Family picnic" />
            </div>
          </div>
          <div class="post-actions">
            <button class="action-btn"><img src="../assets/comment-icon.svg" alt="Comment" /> Comment</button>
            <button class="action-btn"><img src="../assets/like-icon.svg" alt="Like" /></button>
          </div>
        </div>
      </div>
      
      <div class="suggestions">
        <h3>Suggested Friends</h3>
        <div class="friend-suggestion">
          <img src="https://images.unsplash.com/photo-1531746020798-e6953c6e8e04?q=80&w=2000&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Olivia Anderson" class="suggestion-avatar" />
          <div class="suggestion-info">
            <h4>Olivia Anderson</h4>
            <p>@Olivia1945</p>
          </div>
          <button class="add-friend-btn">+</button>
        </div>
        
        <div class="friend-suggestion">
          <img src="https://images.unsplash.com/photo-1546456073-92b9f0a8d413?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Thomas Baker" class="suggestion-avatar" />
          <div class="suggestion-info">
            <h4>Thomas Baker</h4>
            <p>@Thomasbaker1949</p>
          </div>
          <button class="add-friend-btn">+</button>
        </div>
        
        <div class="friend-suggestion">
          <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=1888&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Lily Lee" class="suggestion-avatar" />
          <div class="suggestion-info">
            <h4>Lily Lee</h4>
            <p>@Lily1960</p>
          </div>
          <button class="add-friend-btn">+</button>
        </div>
        
        <div class="friend-suggestion">
          <img src="https://images.unsplash.com/photo-1582289545259-253ae3b93a84?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Andrew Harris" class="suggestion-avatar" />
          <div class="suggestion-info">
            <h4>Andrew Harris</h4>
            <p>@Andrew1939</p>
          </div>
          <button class="add-friend-btn">+</button>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  methods: {
    goToLogin() {
      this.$router.push('/')
    }
  }
}
</script>

<style scoped>
.home-page {
  min-height: 100vh;
  background-color: #f5f5f5;
}

.header {
  background-color: #1D7C40;
  padding: 15px 0;
  color: white;
}

.header-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  display: flex;
  align-items: center;
  font-weight: bold;
  font-size: 18px;
}

.logo img {
  width: 30px;
  height: 30px;
  margin-right: 10px;
}

.search-bar {
  display: flex;
  align-items: center;
  background-color: rgba(255, 255, 255, 0.2);
  border-radius: 20px;
  padding: 5px 15px;
  width: 300px;
}

.search-icon {
  margin-right: 10px;
}

.search-bar input {
  background: transparent;
  border: none;
  color: white;
  width: 100%;
  outline: none;
}

.search-bar input::placeholder {
  color: rgba(255, 255, 255, 0.8);
}

.user-actions {
  display: flex;
  align-items: center;
}

.logout-btn {
  background: none;
  border: none;
  color: white;
  cursor: pointer;
  margin-right: 15px;
}

.profile-icon img {
  width: 35px;
  height: 35px;
  border-radius: 50%;
  object-fit: cover;
}

.main-content {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  gap: 20px;
  padding-top: 20px;
}

.profile-sidebar, .feed, .suggestions {
  background-color: white;
  border-radius: 10px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

.profile-header {
  position: relative;
  padding-bottom: 15px;
}

.profile-bg {
  height: 100px;
  overflow: hidden;
}

.profile-bg img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.profile-avatar {
  position: absolute;
  left: 20px;
  top: 50px;
  border: 4px solid white;
  border-radius: 50%;
  overflow: hidden;
  width: 80px;
  height: 80px;
}

.profile-avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.profile-info {
  padding: 40px 20px 10px;
}

.profile-info h2 {
  font-size: 18px;
  margin-bottom: 5px;
}

.username {
  color: #666;
  font-size: 14px;
  margin-bottom: 10px;
}

.bio {
  font-size: 14px;
  line-height: 1.4;
  color: #444;
}

.profile-nav {
  border-top: 1px solid #eee;
}

.profile-nav ul {
  list-style: none;
}

.profile-nav li {
  padding: 15px 20px;
  display: flex;
  align-items: center;
  font-weight: 500;
  cursor: pointer;
}

.profile-nav li a {
  display: flex;
  align-items: center;
  color: inherit;
  text-decoration: none;
  width: 100%;
}

.profile-nav li.active {
  background-color: #f0f7f3;
  color: #1D7C40;
  border-left: 3px solid #1D7C40;
}

.profile-nav li img {
  width: 20px;
  margin-right: 10px;
}

.feed-tabs {
  display: flex;
  border-bottom: 1px solid #eee;
}

.tab {
  padding: 15px 20px;
  background: none;
  border: none;
  cursor: pointer;
  font-weight: 500;
  color: #666;
}

.tab.active {
  color: #1D7C40;
  border-bottom: 2px solid #1D7C40;
}

.stats {
  display: flex;
  justify-content: space-around;
  padding: 20px;
  text-align: center;
  border-bottom: 1px solid #eee;
}

.stat-number {
  display: block;
  font-size: 24px;
  font-weight: bold;
  color: #1D7C40;
}

.stat-label {
  font-size: 14px;
  color: #666;
}

.post {
  padding: 20px;
  border-bottom: 1px solid #eee;
}

.post-header {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
}

.post-avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  margin-right: 10px;
}

.post-info {
  flex: 1;
}

.post-info h3 {
  font-size: 16px;
  margin-bottom: 2px;
}

.post-username, .post-time {
  font-size: 14px;
  color: #666;
}

.post-actions {
  display: flex;
  justify-content: flex-start;
  padding-top: 15px;
}

.action-btn {
  display: flex;
  align-items: center;
  background: none;
  border: none;
  color: #666;
  margin-right: 20px;
  cursor: pointer;
}

.action-btn img {
  margin-right: 5px;
  width: 20px;
}

.post-content {
  font-size: 15px;
  line-height: 1.5;
  margin-bottom: 15px;
}

.post-image {
  border-radius: 10px;
  overflow: hidden;
  margin: 15px 0;
}

.post-image img {
  width: 100%;
}

.suggestions {
  padding: 20px;
}

.suggestions h3 {
  margin-bottom: 15px;
  font-size: 18px;
}

.friend-suggestion {
  display: flex;
  align-items: center;
  padding: 10px 0;
  border-bottom: 1px solid #eee;
}

.suggestion-avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  margin-right: 10px;
}

.suggestion-info {
  flex: 1;
}

.suggestion-info h4 {
  font-size: 16px;
  margin-bottom: 2px;
}

.suggestion-info p {
  font-size: 14px;
  color: #666;
}

.add-friend-btn {
  width: 30px;
  height: 30px;
  border-radius: 50%;
  background-color: #1D7C40;
  color: white;
  border: none;
  font-size: 20px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}

@media (max-width: 1024px) {
  .main-content {
    grid-template-columns: 1fr 2fr;
  }
  
  .suggestions {
    display: none;
  }
}

@media (max-width: 768px) {
  .main-content {
    grid-template-columns: 1fr;
  }
  
  .profile-sidebar {
    display: none;
  }
}
</style> 