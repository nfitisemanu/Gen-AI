# Gen-AI

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Angel Reese - Influencer Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f0f2f5;
    }
    header {
      background-color: #fff;
      padding: 20px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      position: relative;
    }
    header h1 {
      margin: 0;
    }
    .basketball {
      width: 40px;
      height: 40px;
      background-image: url('https://upload.wikimedia.org/wikipedia/commons/7/7a/Basketball.png');
      background-size: cover;
      position: absolute;
      top: 10px;
      left: -50px;
      animation: bounceBall 5s linear infinite;
    }
    @keyframes bounceBall {
      0% { left: -50px; top: 10px; transform: rotate(0deg); }
      25% { top: 30px; transform: rotate(90deg); }
      50% { top: 10px; left: 50%; transform: rotate(180deg); }
      75% { top: 30px; transform: rotate(270deg); }
      100% { left: 100%; top: 10px; transform: rotate(360deg); }
    }
    .profile, .posts, .stats, .merch {
      max-width: 800px;
      margin: 20px auto;
    }
    .profile {
      background-color: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      text-align: center;
    }
    .profile img {
      width: 150px;
      border-radius: 50%;
    }
    .post, table, .merch {
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .post {
      margin-bottom: 20px;
      padding: 15px;
    }
    table {
      width: 100%;
      overflow: hidden;
      text-align: center;
    }
    table thead {
      background: #f7f7f7;
    }
    table th, table td {
      padding: 10px;
    }
    .merch {
      text-align: center;
      padding: 20px;
    }
    .merch a {
      margin: 10px;
      display: inline-block;
      text-decoration: none;
      color: black;
    }
    .merch img {
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <header>
    <div class="basketball"></div>
    <h1>Angel Reese</h1>
  </header>

  <div class="profile">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Angel_Reese_2023.jpg/220px-Angel_Reese_2023.jpg" alt="Angel Reese Profile Picture">
    <h2 id="name">@angelreese10</h2>
    <p id="bio">College Hoops Star | NCAA Champion | Fashion & Fitness Enthusiast</p>
  </div>

  <div class="posts" id="posts">
    <!-- Posts will be added here -->
  </div>

  <div class="stats">
    <h2 style="text-align:center;">Recent Game Stats</h2>
    <table>
      <thead>
        <tr>
          <th>Date</th>
          <th>Opponent</th>
          <th>Points</th>
          <th>Rebounds</th>
          <th>Assists</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>Mar 25, 2025</td><td>UConn</td><td>26</td><td>14</td><td>3</td></tr>
        <tr><td>Mar 18, 2025</td><td>South Carolina</td><td>30</td><td>17</td><td>2</td></tr>
        <tr><td>Mar 12, 2025</td><td>Georgia</td><td>22</td><td>11</td><td>5</td></tr>
      </tbody>
    </table>
  </div>

  <div class="merch">
    <h2>Shop Angel's Look</h2>
    <a href="https://example.com/shoes" target="_blank">
      <img src="https://via.placeholder.com/150x150?text=Signature+Sneakers" alt="Sneakers">
      <p>Signature Sneakers</p>
    </a>
    <a href="https://example.com/jersey" target="_blank">
      <img src="https://via.placeholder.com/150x150?text=Official+Jersey" alt="Jersey">
      <p>Official Jersey</p>
    </a>
  </div>

  <script>
    const posts = [
      {
        content: "Grateful for another day to chase greatness 🏀✨ #Blessed #GRWNATION",
      },
      {
        content: "Game day fit 💅💃 Who said athletes can't serve looks? #StyleOnAndOffCourt",
      },
      {
        content: "Big dub tonight with my girls! We locked in 🔒 #NCAA #HoopsQueen",
      }
    ];

    const postsContainer = document.getElementById('posts');

    posts.forEach(post => {
      const postDiv = document.createElement('div');
      postDiv.className = 'post';
      postDiv.textContent = post.content;
      postsContainer.appendChild(postDiv);
    });
  </script>

</body>
</html>
