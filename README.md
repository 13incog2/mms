<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kthe • Links</title>
  <link rel="icon" href="https://github.githubassets.com/favicons/favicon.svg" type="image/svg+xml">
  <style>
    :root {
      --bg: #0d0d0f;
      --card: rgba(20, 20, 30, 0.6);
      --text: #e0e0ff;
      --accent: #00ddeb;
      --accent-glow: #00ddeb33;
      --border: rgba(0, 221, 235, 0.18);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      background: var(--bg);
      color: var(--text);
      font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      background-image: 
        radial-gradient(circle at 15% 50%, #1a0033 0%, transparent 40%),
        radial-gradient(circle at 85% 30%, #001a33 0%, transparent 40%);
      background-attachment: fixed;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 2rem 1rem;
    }

    .container {
      width: 100%;
      max-width: 420px;
      text-align: center;
    }

    .avatar {
      width: 110px;
      height: 110px;
      border-radius: 50%;
      border: 3px solid var(--accent);
      box-shadow: 0 0 30px var(--accent-glow);
      margin-bottom: 1.2rem;
      object-fit: cover;
      background: #111;
    }

    h1 {
      font-size: 2.1rem;
      margin-bottom: 0.4rem;
      letter-spacing: -0.5px;
      background: linear-gradient(90deg, #a78bfa, #7dd3fc, #00ddeb);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .bio {
      font-size: 1.05rem;
      opacity: 0.85;
      margin-bottom: 2.2rem;
      line-height: 1.5;
    }

    .links {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    .btn {
      display: block;
      padding: 1.1rem 1.5rem;
      background: var(--card);
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
      border: 1px solid var(--border);
      border-radius: 16px;
      color: var(--text);
      font-size: 1.1rem;
      font-weight: 500;
      text-decoration: none;
      transition: all 0.35s ease;
      position: relative;
      overflow: hidden;
      box-shadow: 0 8px 32px rgba(0,0,0,0.35);
    }

    .btn:hover {
      transform: translateY(-4px);
      box-shadow: 0 16px 40px var(--accent-glow);
      border-color: var(--accent);
      color: white;
    }

    .btn::before {
      content: '';
      position: absolute;
      top: 0; left: -100%;
      width: 100%; height: 100%;
      background: linear-gradient(90deg, transparent, rgba(0,221,235,0.15), transparent);
      transition: 0.6s;
    }

    .btn:hover::before {
      left: 100%;
    }

    .small {
      font-size: 0.9rem;
      opacity: 0.7;
      margin-top: 3rem;
    }

    @media (max-width: 480px) {
      .container { padding: 0 1rem; }
      h1 { font-size: 1.9rem; }
    }
  </style>
</head>
<body>

  <div class="container">
    <!-- Optional: add your GitHub profile pic or any image -->
    <img 
      class="avatar" 
      src="https://github.com/kthe.png" 
      alt="Kthe" 
      onerror="this.src='https://via.placeholder.com/110/111/eee?text=K'">

    <h1>Kthe</h1>
    <p class="bio">Geelong-based dev • building stuff on GitHub • random ideas & experiments</p>

    <div class="links">
      <a href="https://github.com/kthe" class="btn" target="_blank">GitHub Profile →</a>
      <a href="https://github.com/kthe?tab=repositories" class="btn" target="_blank">My Repositories</a>
      <a href="https://github.com/kthe/kthe.github.io" class="btn" target="_blank">This Website Source</a>
      
      <!-- Add more of your cool repos / projects here -->
      <a href="https://github.com/kthe/your-cool-project-1" class="btn" target="_blank">Project Alpha – [short desc]</a>
      <a href="https://github.com/kthe/your-cool-project-2" class="btn" target="_blank">Game / Tool / Whatever</a>
      
      <!-- Optional extras -->
      <!-- <a href="https://twitter.com/yourhandle" class="btn" target="_blank">X / Twitter</a> -->
      <!-- <a href="https://linkedin.com/in/yourname" class="btn" target="_blank">LinkedIn</a> -->
    </div>

    <p class="small">Made with ❤️ using only GitHub Pages • 2026 vibes</p>
  </div>

</body>
</html>
