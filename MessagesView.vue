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
            <li><router-link to="/home"><img src="../assets/home-icon.svg" alt="Home" /> Home</router-link></li>
            <li><img src="../assets/profile-icon.svg" alt="Profile" /> Profile</li>
            <li class="active"><router-link to="/messages"><img src="../assets/messages-icon.svg" alt="Messages" /> Messages</router-link></li>
            <li><img src="../assets/notifications-icon.svg" alt="Notifications" /> Notifications</li>
          </ul>
        </nav>
      </div>
      
      <div class="messages-container">
        <div class="messages-header">
          <h2>Messages</h2>
          <button class="new-message-btn">New Message</button>
        </div>
        
        <div class="messages-list">
          <div class="message-contact active">
            <img src="https://images.unsplash.com/photo-1566616213894-2d4e1baee5d8?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Bessie Cooper" class="contact-avatar" />
            <div class="contact-info">
              <div class="contact-name-time">
                <h3>Bessie Cooper</h3>
                <span class="message-time">11:42 AM</span>
              </div>
              <p class="message-preview">I'd love to see them again too! How about...</p>
            </div>
          </div>
          
          <div class="message-contact">
            <img src="https://images.unsplash.com/photo-1522075469751-3a6694fb2f61?q=80&w=2080&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Jonathan Jones" class="contact-avatar" />
            <div class="contact-info">
              <div class="contact-name-time">
                <h3>Jonathan Jones</h3>
                <span class="message-time">Yesterday</span>
              </div>
              <p class="message-preview">The picnic was wonderful! Thanks for asking...</p>
            </div>
          </div>
          
          <div class="message-contact">
            <img src="https://images.unsplash.com/photo-1531746020798-e6953c6e8e04?q=80&w=2000&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Olivia Anderson" class="contact-avatar" />
            <div class="contact-info">
              <div class="contact-name-time">
                <h3>Olivia Anderson</h3>
                <span class="message-time">Monday</span>
              </div>
              <p class="message-preview">Would you like to join our book club? We meet...</p>
            </div>
          </div>
          
          <div class="message-contact">
            <img src="https://images.unsplash.com/photo-1546456073-92b9f0a8d413?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Thomas Baker" class="contact-avatar" />
            <div class="contact-info">
              <div class="contact-name-time">
                <h3>Thomas Baker</h3>
                <span class="message-time">Last Week</span>
              </div>
              <p class="message-preview">Hello Robert, I've been meaning to ask you about...</p>
            </div>
          </div>
        </div>
        
        <div class="message-chat">
          <div class="chat-header">
            <img src="https://images.unsplash.com/photo-1566616213894-2d4e1baee5d8?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Bessie Cooper" class="contact-avatar" />
            <div>
              <h3>Bessie Cooper</h3>
              <p>Online</p>
            </div>
          </div>
          
          <div class="chat-messages">
            <div class="message-date">Today</div>
            
            <div class="message-bubble received">
              <p>Hi Robert! How are your grandchildren doing? I remember you mentioned they were coming to visit.</p>
              <span class="message-time">10:30 AM</span>
            </div>
            
            <div class="message-bubble sent">
              <p>Hello Bessie! They're wonderful, thanks for asking. We had such a great time together. I hadn't seen them in almost a year!</p>
              <span class="message-time">10:45 AM</span>
            </div>
            
            <div class="message-bubble received">
              <p>That's so wonderful to hear! I miss my grandkids too. They grow up so fast, don't they?</p>
              <span class="message-time">11:02 AM</span>
            </div>
            
            <div class="message-bubble sent">
              <p>They really do! Little Tommy is already 8 and talking about computers all day. I can barely keep up!</p>
              <span class="message-time">11:15 AM</span>
            </div>
            
            <div class="message-bubble received">
              <p>Haha, that's how it goes these days. My grandchildren are teaching me how to use all these new apps. I'd love to see them again too! How about we plan a day at the park with all the grandkids?</p>
              <span class="message-time">11:42 AM</span>
            </div>
          </div>
          
          <div class="chat-input">
            <input type="text" placeholder="Type a message..." />
            <button class="send-btn">Send</button>
          </div>
        </div>
      </div>
      
      <div class="online-friends">
        <h3>Online Friends</h3>
        <div class="online-friend">
          <div class="online-indicator"></div>
          <img src="https://images.unsplash.com/photo-1566616213894-2d4e1baee5d8?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Bessie Cooper" class="friend-avatar" />
          <p>Bessie C.</p>
        </div>
        
        <div class="online-friend">
          <div class="online-indicator"></div>
          <img src="https://images.unsplash.com/photo-1531746020798-e6953c6e8e04?q=80&w=2000&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Olivia Anderson" class="friend-avatar" />
          <p>Olivia A.</p>
        </div>
        
        <div class="online-friend">
          <div class="online-indicator offline"></div>
          <img src="https://images.unsplash.com/photo-1522075469751-3a6694fb2f61?q=80&w=2080&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Jonathan Jones" class="friend-avatar" />
          <p>Jonathan J.</p>
        </div>
        
        <div class="online-friend">
          <div class="online-indicator offline"></div>
          <img src="https://images.unsplash.com/photo-1546456073-92b9f0a8d413?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Thomas Baker" class="friend-avatar" />
          <p>Thomas B.</p>
        </div>
        
        <div class="online-friend">
          <div class="online-indicator"></div>
          <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=1888&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Lily Lee" class="friend-avatar" />
          <p>Lily L.</p>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'MessagesView',
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

.profile-sidebar, .messages-container, .online-friends {
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

/* Messages specific styles */
.messages-container {
  display: flex;
  flex-direction: column;
  height: calc(100vh - 110px);
}

.messages-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 20px;
  border-bottom: 1px solid #eee;
}

.messages-header h2 {
  font-size: 20px;
  color: #333;
}

.new-message-btn {
  background-color: #1D7C40;
  color: white;
  border: none;
  padding: 8px 16px;
  border-radius: 5px;
  cursor: pointer;
  font-weight: 500;
}

.messages-list {
  width: 35%;
  border-right: 1px solid #eee;
  overflow-y: auto;
  height: 100%;
}

.message-contact {
  display: flex;
  padding: 15px;
  border-bottom: 1px solid #eee;
  cursor: pointer;
}

.message-contact.active {
  background-color: #f0f7f3;
}

.contact-avatar {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  margin-right: 15px;
  object-fit: cover;
}

.contact-info {
  flex: 1;
}

.contact-name-time {
  display: flex;
  justify-content: space-between;
  margin-bottom: 5px;
}

.contact-name-time h3 {
  font-size: 16px;
  font-weight: 600;
}

.message-time {
  color: #777;
  font-size: 12px;
}

.message-preview {
  color: #666;
  font-size: 14px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.message-chat {
  display: flex;
  flex-direction: column;
  width: 65%;
  height: 100%;
}

.chat-header {
  display: flex;
  align-items: center;
  padding: 15px 20px;
  border-bottom: 1px solid #eee;
}

.chat-header img {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  margin-right: 15px;
  object-fit: cover;
}

.chat-header h3 {
  font-size: 16px;
  margin-bottom: 3px;
}

.chat-header p {
  color: #1D7C40;
  font-size: 12px;
}

.chat-messages {
  flex: 1;
  padding: 20px;
  overflow-y: auto;
  display: flex;
  flex-direction: column;
}

.message-date {
  text-align: center;
  margin: 10px 0;
  color: #888;
  font-size: 12px;
}

.message-bubble {
  max-width: 75%;
  padding: 12px 15px;
  border-radius: 18px;
  margin-bottom: 15px;
  position: relative;
}

.message-bubble p {
  margin: 0;
  font-size: 15px;
  line-height: 1.4;
}

.message-bubble .message-time {
  font-size: 11px;
  color: #999;
  text-align: right;
  margin-top: 5px;
}

.message-bubble.sent {
  align-self: flex-end;
  background-color: #e6f7ed;
  border-bottom-right-radius: 5px;
}

.message-bubble.received {
  align-self: flex-start;
  background-color: #f0f2f5;
  border-bottom-left-radius: 5px;
}

.chat-input {
  display: flex;
  padding: 15px;
  border-top: 1px solid #eee;
}

.chat-input input {
  flex: 1;
  padding: 12px 15px;
  border: 1px solid #ddd;
  border-radius: 25px;
  outline: none;
  font-size: 15px;
}

.send-btn {
  margin-left: 10px;
  background-color: #1D7C40;
  color: white;
  border: none;
  border-radius: 25px;
  padding: 0 20px;
  font-weight: 500;
  cursor: pointer;
}

/* Online friends sidebar */
.online-friends {
  padding: 20px;
}

.online-friends h3 {
  margin-bottom: 20px;
  font-size: 18px;
  color: #333;
}

.online-friend {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
  position: relative;
}

.online-indicator {
  width: 10px;
  height: 10px;
  background-color: #42b883;
  border-radius: 50%;
  position: absolute;
  bottom: 0;
  left: 30px;
  border: 2px solid white;
}

.online-indicator.offline {
  background-color: #ddd;
}

.friend-avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  margin-right: 10px;
  object-fit: cover;
}

.online-friend p {
  font-size: 14px;
  font-weight: 500;
}

@media (max-width: 1024px) {
  .main-content {
    grid-template-columns: 1fr 2fr;
  }
  
  .online-friends {
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
  
  .messages-container {
    height: calc(100vh - 80px);
  }
  
  .messages-list {
    width: 100%;
    border-right: none;
    height: auto;
    max-height: 40vh;
  }
  
  .message-chat {
    width: 100%;
  }
}
</style> 