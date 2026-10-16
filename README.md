
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>For My Khadusman ❤️</title>

<style>
* { box-sizing: border-box; }

body {
  margin: 0;
  background: #210810;
  color: #fff0e9;
  font-family: Georgia, serif;
  text-align: center;
  overflow-x: hidden;
}

section {
  padding: 55px 18px;
  position: relative;
}

.hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background:
    radial-gradient(ellipse at top, #84304b, transparent 65%),
    linear-gradient(150deg, #3b101f, #18060d);
}

.eyebrow {
  letter-spacing: 4px;
  font: 12px Arial, sans-serif;
  color: #f3c58d;
}

h1 {
  font-size: clamp(39px, 10vw, 62px);
  line-height: 1.12;
  color: #ffb5c5;
  margin: 22px 0;
  text-shadow: 0 0 25px #e64b7955;
}

h2 {
  color: #ffd3a0;
  font-size: 30px;
}

p {
  line-height: 1.8;
  font-size: 17px;
}

button, .upload-label {
  border: 1px solid #ffd4a7;
  border-radius: 40px;
  background: linear-gradient(135deg, #e84972, #a51e48);
  color: white;
  padding: 14px 23px;
  font-size: 16px;
  cursor: pointer;
  font-family: Arial, sans-serif;
  display: inline-block;
  margin: 8px 4px;
}

button:active { transform: scale(.97); }

.secondary {
  background: #471626;
}

.gift {
  font-size: 85px;
  margin: 18px;
  animation: pulse 1.5s infinite;
}

@keyframes pulse {
  50% { transform: scale(1.1); }
}

.panel {
  max-width: 520px;
  margin: 20px auto;
  padding: 25px 20px;
  border: 1px solid #a95769;
  border-radius: 22px;
  background: #441523;
  box-shadow: 0 12px 35px #0004;
}

.hidden { display: none !important; }

.gallery {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
  max-width: 520px;
  margin: 25px auto;
}

.photo {
  min-height: 150px;
  border: 1px solid #a95769;
  border-radius: 15px;
  overflow: hidden;
  background: #572033;
  display: grid;
  place-items: center;
  color: #ffd5dc;
  padding: 8px;
}

.photo img {
  width: 100%;
  height: 190px;
  object-fit: cover;
  display: block;
}

input[type=file] {
  width: 100%;
  max-width: 320px;
  margin: 12px auto;
  color: #ffe2e8;
}

.letter {
  white-space: pre-line;
  text-align: left;
  font-size: 17px;
}

footer {
  padding: 30px 15px;
  color: #eeb5c3;
  font-size: 14px;
}

.heart {
  position: fixed;
  bottom: -30px;
  z-index: 5;
  pointer-events: none;
  animation: floatUp 6s linear forwards;
}

@keyframes floatUp {
  to {
    transform: translateY(-110vh) rotate(25deg);
    opacity: 0;
  }
}

.glow { color: #ffb5c5; }

#finalMessage {
  font-size: 24px;
  color: #ffd0a2;
}
</style>
</head>

<body>

<!-- OPENING PAGE -->
<section class="hero" id="opening">
  <div class="eyebrow">A LITTLE SURPRISE FOR MY FAVOURITE PERSON</div>
  <div class="gift">🎁</div>
  <p>To my one and only...</p>
  <h1>Happy Birthday,<br>My Khadusman! 😘</h1>
  <p>One special day. One special person.<br>A million little feelings. ❤️</p>
  <button onclick="openGift()">Open Your Gift 🎁</button>
  <p style="font-size:13px;color:#f3c58d">Made with love, just for you.</p>
</section>

<!-- MAIN SURPRISE -->
<div id="surprise" class="hidden">

  <section>
    <div class="eyebrow">CHAPTER ONE</div>
    <h2>Hey, Birthday Boy! ❤️</h2>
    <p>
      Welcome to your little corner of my world.
      No matter how much of a khadus you are,
      you have a special place in my heart. 😁💕
    </p>
    <div class="panel">
      <div style="font-size:48px">🌹</div>
      <p>Today, this little website is all yours.</p>
      <p class="glow">Scroll down, my favourite troublemaker!</p>
    </div>
  </section>

  <!-- PHOTO GALLERY -->
  <section>
    <div class="eyebrow">CHAPTER TWO</div>
    <h2>Our Little Memories 📸</h2>
    <p>Every picture holds a little piece of our story.</p>

    <div class="panel">
      <p>Select your couple photos from your phone:</p>
      <input id="photoPicker" type="file"
        accept="image/*" multiple>
      <p style="font-size:13px">
        Choose multiple photos. They'll appear below.
      </p>
    </div>

    <div id="gallery" class="gallery">
      <div class="photo">❤️<br>Our first memory</div>
      <div class="photo">🌹<br>Our favourite moment</div>
    </div>
  </section>

  <!-- SECRET LETTER -->
  <section>
    <div class="eyebrow">CHAPTER THREE</div>
    <h2>A Secret Letter For You 💌</h2>
    <p>There are things I want you to read from my heart.</p>
    <div style="font-size:55px">💌</div>
    <button onclick="openLetter()">Open My Secret Letter</button>

    <div id="letter" class="panel hidden">
      <h2>My Dear Khadusman, ❤️</h2>
      <div class="letter">Happy Birthday, my favourite human! 😘

I may tease you, annoy you, and call you khadusman, but you are genuinely so special to me.

Thank you for the little moments, the laughs, the conversations, and all the memories that make our story ours.

On your birthday, I wish you happiness, courage, success, good health, and the strength to chase every dream in your heart.

Keep smiling, keep growing, and never forget how much you matter.

And yes, Mr. Khadusman, you still have to tolerate me! 😂❤️

With all my love,
Your Terrorist 😁💋</div>
      <p style="text-align:center">Forever sending you hugs and happiness. 💗</p>
    </div>
  </section>

  <!-- OPTIONAL MUSIC -->
  <section>
    <div class="eyebrow">CHAPTER FOUR</div>
    <h2>Our Little Love Song 🎶</h2>
    <p>Choose a song from your phone to play while you explore.</p>
    <div class="panel">
      <input id="musicPicker" type="file" accept="audio/*">
      <br>
      <button onclick="toggleMusic()" id="musicButton">
        ▶ Play Our Song
      </button>
      <audio id="song" loop></audio>
      <p id="musicStatus" style="font-size:13px">
        Music is optional. Choose a song first.
      </p>
    </div>
  </section>

  <!-- FINAL SURPRISE -->
  <section>
    <div class="eyebrow">THE FINAL SURPRISE</div>
    <h2>One Last Little Thing... 💝</h2>
    <div class="gift">🎂</div>
    <p>Ready, birthday boy?</p>
    <button onclick="showFinal()">Reveal Your Final Surprise ✨</button>

    <div id="final" class="panel hidden">
      <div style="font-size:65px">❤️🎂❤️</div>
      <p id="finalMessage">
        Happy Birthday, Khadusman! 😘
      </p>
      <p>
        May this year bring you closer to every dream
        you've ever wished for.
      </p>
      <p>
        Thank you for being you. Keep smiling,
        keep shining, and keep being my favourite
        troublemaker. 🥹❤️
      </p>
      <h2>Lots of love,</h2>
      <h1 style="font-size:40px">Your Terrorist 😁💋</h1>
      <p>End of surprise... but never the love. 💌</p>
    </div>
  </section>

  <footer>
    Created with ❤️ by Terrorist 😁<br>
    Especially for Khadusman 😘
  </footer>
</div>

<script>
function openGift() {
  document.getElementById("surprise").classList.remove("hidden");
  document.getElementById("opening").style.display = "none";
  window.scrollTo(0, 0);
  hearts();
}

function openLetter() {
  document.getElementById("letter").classList.remove("hidden");
}

function showFinal() {
  document.getElementById("final").classList.remove("hidden");
  hearts();
  document.getElementById("final").scrollIntoView({
    behavior: "smooth",
    block: "center"
  });
}

function hearts() {
  for (let i = 0; i < 18; i++) {
    setTimeout(() => {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.textContent = ["❤️", "💕", "💗", "✨"][Math.floor(Math.random() * 4)];
      heart.style.left = Math.random() * 95 + "vw";
      heart.style.fontSize = (18 + Math.random() * 18) + "px";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }, i * 180);
  }
}

// Add photos selected from the phone.
const photoPicker = document.getElementById("photoPicker");
photoPicker.addEventListener("change", function() {
  const gallery = document.getElementById("gallery");
  gallery.innerHTML = "";

  Array.from(this.files).forEach(file => {
    if (!file.type.startsWith("image/")) return;

    const reader = new FileReader();
    reader.onload = function(e) {
      const frame = document.createElement("div");
      frame.className = "photo";

      const img = document.createElement("img");
      img.src = e.target.result;
      img.alt = "Our memory";

      frame.appendChild(img);
      gallery.appendChild(frame);
    };
    reader.readAsDataURL(file);
  });
});

// Select and play a song from the phone.
const song = document.getElementById("song");
const musicPicker = document.getElementById("musicPicker");
const musicButton = document.getElementById("musicButton");
const musicStatus = document.getElementById("musicStatus");

musicPicker.addEventListener("change", function() {
  const file = this.files[0];
  if (!file) return;

  song.src = URL.createObjectURL(file);
  musicStatus.textContent = "Your song is ready! Press play.";
  musicButton.textContent = "▶ Play Our Song";
});

async function toggleMusic() {
  if (!song.src) {
    musicStatus.textContent = "Choose a song from your phone first.";
    musicPicker.click();
    return;
  }

  if (song.paused) {
    try {
      await song.play();
      musicButton.textContent = "⏸ Pause Our Song";
      musicStatus.textContent = "Playing your special song ❤️";
    } catch (e) {
      musicStatus.textContent = "Tap play again to start your song.";
    }
  } else {
    song.pause();
    musicButton.textContent = "▶ Play Our Song";
    musicStatus.textContent = "Song paused.";
  }
}

song.addEventListener("ended", function() {
  musicButton.textContent = "▶ Play Our Song";
});
</script>

</body>
</html>

