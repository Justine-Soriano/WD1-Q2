<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>News Feed Page</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f4f4f9;
      color: #333;
    }

    /* Navbar */
    header {
      position: sticky;
      top: 0;
      background: #4267B2;
      color: #fff;
      padding: 10px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 1000;
    }

    .navbar-left {
      font-weight: bold;
      font-size: 20px;
    }

    .navbar-center a {
      color: white;
      margin: 0 10px;
      text-decoration: none;
      font-weight: bold;
    }

    .navbar-right {
      position: relative;
    }

    .dropdown {
      display: none;
      position: absolute;
      right: 0;
      background: white;
      color: black;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
      border-radius: 5px;
      overflow: hidden;
    }

    .dropdown a {
      display: block;
      padding: 10px;
      text-decoration: none;
      color: black;
    }

    .dropdown a:hover {
      background: #f0f0f0;
    }

    .navbar-right:hover .dropdown {
      display: block;
    }

    /* Layout */
    main {
      display: flex;
      padding: 20px;
    }

    aside {
      width: 20%;
      padding: 10px;
    }

    .feed {
      width: 80%;
      padding: 10px;
    }

    /* Profile */
    .profile, .friends {
      background: white;
      padding: 15px;
      border-radius: 10px;
      margin-bottom: 20px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .profile img, .friends img {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      margin-right: 10px;
    }

    .friend {
      display: flex;
      align-items: center;
      margin: 10px 0;
    }

    /* Post cards */
    .post {
      background: white;
      border-radius: 10px;
      padding: 15px;
      margin-bottom: 20px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .post img {
      width: 100%;
      border-radius: 10px;
      margin-top: 10px;
    }

    .post .actions {
      display: flex;
      justify-content: space-between;
      margin-top: 10px;
      font-size: 14px;
      color: #555;
    }

    footer {
      text-align: center;
      padding: 15px;
      background: #4267B2;
      color: white;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <!-- Header -->
  <header>
    <div class="navbar-left">AppName</div>
    <div class="navbar-center">
      <a href="#">Home</a>
      <a href="#">Chats</a>
      <a href="#">Marketplace</a>
    </div>
    <div class="navbar-right">
      ⚙️ Settings
      <div class="dropdown">
        <a href="#">Profile</a>
        <a href="#">Log out</a>
      </div>
    </div>
  </header>

  <!-- Main Content -->
  <main>
    <!-- Aside -->
    <aside>
      <div class="profile">
        <img src="https://via.placeholder.com/50" alt="Profile">
        <h3>John Doe</h3>
        <p>@johndoe</p>
        <p> Address: City, Country</p>
        <p> Birthday: Jan 1, 2000</p>
        <p> Joined: 2022</p>
      </div>

      <div class="friends">
        <h4>Friends</h4>
        <div class="friend">
          <img src="https://via.placeholder.com/50" alt="">
          <p>Alice @alice</p>
        </div>
        <div class="friend">
          <img src="https://via.placeholder.com/50" alt="">
          <p>Bob @bob</p>
        </div>
        <div class="friend">
          <img src="https://via.placeholder.com/50" alt="">
          <p>Charlie @charlie</p>
        </div>
        <div class="friend">
          <img src="https://via.placeholder.com/50" alt="">
          <p>Diana @diana</p>
        </div>
        <div class="friend">
          <img src="https://via.placeholder.com/50" alt="">
          <p>Edward @edward</p>
        </div>
      </div>
    </aside>

    <!-- Feed -->
    <div class="feed">
      <!-- Post 1 -->
      <div class="post">
        <h4>Mike @mike • 6h</h4>
        <p>Guy with fear of heights gets the courage to climb a cliffside!</p>
        <img src="https://via.placeholder.com/600x300" alt="Post Image">
        <div class="actions">
          <span> 87</span>
          <span> 16</span>
          <span> 36</span>
        </div>
      </div>

      <!-- Post 2 -->
      <div class="post">
        <h4>Sarah @sarah • 5h</h4>
        <p>Film starting out normal but gradually becoming freakish?</p>
        <div class="actions">
          <span> 2.2K</span>
          <span> 198</span>
          <span> 45</span>
        </div>
      </div>

      <!-- Post 3 -->
      <div class="post">
        <h4>Anna @anna • 4h</h4>
        <p>Check out this modern house design!</p>
        <img src="https://via.placeholder.com/600x300" alt="House">
        <div class="actions">
          <span> 12</span>
          <span> 25</span>
          <span> 187</span>
        </div>
      </div>

      <!-- Post 4 -->
