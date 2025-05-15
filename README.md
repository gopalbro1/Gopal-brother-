<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Gopal Brothers</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Enter Screen -->
  <div class="enter-screen" id="enterScreen">
    <img src="enter-background.jpg" alt="Welcome Background" class="background" />
    <div class="enter-content">
      <h1>Welcome to Gopal Brothers</h1>
      <button onclick="enterSite()">Enter Site</button>
    </div>
  </div>

  <!-- Main Content -->
  <div id="mainContent" class="hidden">

    <header>
      <h1>Gopal Brothers</h1>
    </header>

    <section class="section-header">Anime Videos</section>
    <div class="videos-row">
      <div class="video-box">
        <video controls poster="attack-on-titan.jpg" width="350">
          <source src="attack-on-titan.mp4" type="video/mp4" />
          Your browser does not support the video tag.
        </video>
      </div>
      <div class="video-thumbs">
        <img src="my-hero-academia.jpg" alt="My Hero Academia" />
        <img src="demon-slayer.jpg" alt="Demon Slayer" />
        <img src="fate-apocrypha.jpg" alt="Fate Apocrypha" />
      </div>
    </div>

    <div class="section-row">
      <div>
        <h2>Anime Images</h2>
        <img src="mikasa.jpg" alt="Anime Image" class="section-image" />
      </div>

      <div>
        <h2>Animations</h2>
        <div class="animated-box">Hover Me!</div>
      </div>
    </div>

  </div>

  <script>
    function enterSite() {
      document.getElementById('enterScreen').style.display = 'none';
      document.getElementById('mainContent').classList.remove('hidden');
    }
  </script>
</body>
</html>* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Arial', sans-serif;
}

body {
  background-color: #fff0e6;
  color: #e7601b;
}

.hidden {
  display: none;
}

/* Enter Screen */
.enter-screen {
  position: fixed;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.background {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
  filter: brightness(0.6);
  z-index: -1;
}

.enter-content h1 {
  font-size: 3rem;
  font-weight: 700;
  color: white;
  text-align: center;
  margin-bottom: 20px;
  text-shadow: 2px 2px 8px #000;
}

.enter-content button {
  background-color: #f37021;
  border: none;
  color: white;
  padding: 14px 36px;
  font-size: 1.3rem;
  font-weight: 700;
  border-radius: 30px;
  cursor: pointer;
  box-shadow: 0 3px 6px rgba(243, 112, 33, 0.7);
  transition: background-color 0.3s ease;
}

.enter-content button:hover {
  background-color: #c95317;
}

/* Main content header */
header h1 {
  text-align: center;
  font-weight: 700;
  font-size: 2.2rem;
  margin: 40px 0 20px;
}

/* Section Header */
.section-header {
  text-align: center;
  font-weight: 700;
  font-size: 1.8rem;
  margin-bottom: 20px;
}

/* Videos row */
.videos-row {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
  padding: 0 20px 40px;
}

/* Video Box */
.video-box video {
  border-radius: 15px;
  box-shadow: 0 0 20px #e7601b;
}

/* Thumbnails */
.video-thumbs {
  display: flex;
  gap: 10px;
  align-items: center;
}

.video-thumbs img {
  width: 110px;
  height: 160px;
  object-fit: cover;
  border-radius: 15px;
  box-shadow: 0 0 10px #e7601b;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.video-thumbs img:hover {
  transform: scale(1.05);
}

/* Section Row: Images + Animations */
.section-row {
  display: flex;
  justify-content: center;
  gap: 60px;
  padding: 0 20px 60px;
  flex-wrap: wrap;
}

/* Section Image */
.section-image {
  width: 260px;
  height: 350px;
  border-radius: 15px;
  box-shadow: 0 0 20px #e7601b;
  object-fit: cover;
  display: block;
  margin-top: 15px;
}

/* Animations Box */
.animated-box {
  background-color: #ffc75f;
  width: 260px;
  height: 350px;
  border-radius: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: 700;
  font-size: 2.5rem;
  color: #e7601b;
  cursor: pointer;
  box-shadow: 0 0 20px #e7601b;
  transition: transform 0.3s ease, background-color 0.3s ease;
}

.animated-box:hover {
  transform: scale(1.1);
  background-color: #f9b839;
}* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Arial', sans-serif;
}

body {
  background-color: #fff0e6;
  color: #e7601b;
}

.hidden {
  display: none;
}

/* Enter Screen */
.enter-screen {
  position: fixed;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.background {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
  filter: brightness(0.6);
  z-index: -1;
}

.enter-content h1 {
  font-size: 3rem;
  font-weight: 700;
  color: white;
  text-align: center;
  margin-bottom: 20px;
  text-shadow: 2px 2px 8px #000;
}

.enter-content button {
  background-color: #f37021;
  border: none;
  color: white;
  padding: 14px 36px;
  font-size: 1.3rem;
  font-weight: 700;
  border-radius: 30px;
  cursor: pointer;
  box-shadow: 0 3px 6px rgba(243, 112, 33, 0.7);
  transition: background-color 0.3s ease;
}

.enter-content button:hover {
  background-color: #c95317;
}

/* Main content header */
header h1 {
  text-align: center;
  font-weight: 700;
  font-size: 2.2rem;
  margin: 40px 0 20px;
}

/* Section Header */
.section-header {
  text-align: center;
  font-weight: 700;
  font-size: 1.8rem;
  margin-bottom: 20px;
}

/* Videos row */
.videos-row {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
  padding: 0 20px 40px;
}

/* Video Box */
.video-box video {
  border-radius: 15px;
  box-shadow: 0 0 20px #e7601b;
}

/* Thumbnails */
.video-thumbs {
  display: flex;
  gap: 10px;
  align-items: center;
}

.video-thumbs img {
  width: 110px;
  height: 160px;
  object-fit: cover;
  border-radius: 15px;
  box-shadow: 0 0 10px #e7601b;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.video-thumbs img:hover {
  transform: scale(1.05);
}

/* Section Row: Images + Animations */
.section-row {
  display: flex;
  justify-content: center;
  gap: 60px;
  padding: 0 20px 60px;
  flex-wrap: wrap;
}

/* Section Image */
.section-image {
  width: 260px;
  height: 350px;
  border-radius: 15px;
  box-shadow: 0 0 20px #e7601b;
  object-fit: cover;
  display: block;
  margin-top: 15px;
}

/* Animations Box */
.animated-box {
  background-color: #ffc75f;
  width: 260px;
  height: 350px;
  border-radius: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: 700;
  font-size: 2.5rem;
  color: #e7601b;
  cursor: pointer;
  box-shadow: 0 0 20px #e7601b;
  transition: transform 0.3s ease, background-color 0.3s ease;
}

.animated-box:hover {
  transform: scale(1.1);
  background-color: #f9b839;
}
