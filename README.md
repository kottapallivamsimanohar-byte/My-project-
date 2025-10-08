<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Movie Ticket Booking - MyShow</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f4f4f4;
    }
    header {
      background-color: #d81f26;
      color: white;
      padding: 15px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    header .logo {
      font-size: 1.8em;
      font-weight: bold;
      letter-spacing: 2px;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-weight: 600;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .container {
      max-width: 1100px;
      margin: 30px auto;
      padding: 0 20px;
    }
    h1 {
      color: #222;
      text-align: center;
      margin-bottom: 40px;
    }
    .movies {
      display: flex;
      gap: 30px;
      justify-content: center;
      flex-wrap: wrap;
    }
    .movie-card {
      background: white;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      width: 300px;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      transition: transform 0.2s ease;
    }
    .movie-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 15px rgba(216, 31, 38, 0.5);
    }
    .movie-poster img {
      width: 100%;
      height: 400px;
      object-fit: cover;
    }
    .movie-info {
      padding: 20px;
      flex-grow: 1;
      display: flex;
      flex-direction: column;
    }
    .movie-title {
      font-size: 1.3em;
      margin: 0 0 10px 0;
      font-weight: bold;
    }
    .movie-desc {
      font-size: 0.9em;
      color: #555;
      flex-grow: 1;
      margin-bottom: 15px;
    }
    .theatres {
      font-size: 0.9em;
      color: #333;
      margin-bottom: 15px;
    }
    .theatres strong {
      color: #d81f26;
    }
    .book-btn {
      background-color: #d81f26;
      border: none;
      color: white;
      padding: 12px 0;
      border-radius: 5px;
      font-size: 1em;
      font-weight: bold;
      cursor: pointer;
      transition: background-color 0.3s ease;
      width: 100%;
    }
    .book-btn:hover {
      background-color: #a5171f;
    }
    footer {
      background-color: #222;
      color: #ddd;
      text-align: center;
      padding: 15px 20px;
      margin-top: 50px;
    }
    @media (max-width: 700px) {
      .movies {
        flex-direction: column;
        align-items: center;
      }
      .movie-card {
        width: 90%;
        margin-bottom: 30px;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">MyShow</div>
    <nav>
      <a href="#">Home</a>
      <a href="#">Movies</a>
      <a href="#">Contact</a>
    </nav>
  </header>
  <div class="container">
    <h1>Book Your Movie Tickets</h1>
    <div class="movies">

      <!-- Movie 1: They Call Him OG -->
      <div class="movie-card">
        <div class="movie-poster">
          <img src="https://upload.wikimedia.org/wikipedia/en/c/cd/They_Call_Him_Og_Poster.jpg" alt="They Call Him OG Poster" />
        </div>
        <div class="movie-info">
          <div class="movie-title">They Call Him OG</div>
          <div class="movie-desc">
            A gripping thriller exploring identity and justice. Experience the captivating story in theaters near you.
          </div>
          <div class="theatres">
            Available at theatres in Madanapalle:
            <ul>
              <li><strong>Ravi Theatre</strong></li>
              <li><strong>Sri Krishna Cinema Hall</strong></li>
              <li><strong>Siddartha Theatre</strong></li>
            </ul>
          </div>
          <button class="book-btn" onclick="alert('Booking for They Call Him OG coming soon!')">Book Now</button>
        </div>
      </div>

      <!-- Movie 2: Mirai Kantara -->
      <div class="movie-card">
        <div class="movie-poster">
          <img src="https://upload.wikimedia.org/wikipedia/en/9/9a/Mirai_kantara_poster.jpg" alt="Mirai Kantara Poster" />
        </div>
        <div class="movie-info">
          <div class="movie-title">Mirai Kantara</div>
          <div class="movie-desc">
            A heartwarming tale of hope, dreams, and the beauty of the future. Coming soon to your city.
          </div>
          <div class="theatres">
            Available at theatres in Madanapalle:
            <ul>
              <li><strong>Ravi Theatre</strong></li>
              <li><strong>Sri Krishna Cinema Hall</strong></li>
              <li><strong>Siddartha Theatre</strong></li>
            </ul>
          </div>
          <button class="book-btn" onclick="alert('Booking for Mirai Kantara coming soon!')">Book Now</button>
        </div>
      </div>

    </div>
  </div>
  <footer>
    &copy; 2025 MyShow - Movie Ticket Booking Platform
  </footer>
</body>
</html>
