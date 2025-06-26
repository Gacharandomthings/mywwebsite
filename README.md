<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Test gacha number-Trúng 999 là gay</title>
    <style>
        body {
            font-family: Courier;
            background-image: ('https://store-images.s-microsoft.com/image/apps.60323.14294656681058683.4d17bdd8-7026-429a-846f-cf7836bc9e56.a69e6905-8926-4a48-b243-14a039b97aae?mode=scale&q=90&h=1080&w=1920.jpg');;
            background-color: #a9db97
            text-align: center;
            padding: 50px;
        }
        .container {
            max-width: 500px;
            margin: 0 auto;
            padding: 20px;
            background-color: #98a5be;
            border-radius: 12px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #333;
        }
        button {
            padding: 10px 20px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 24px;
        }
        button:hover {
            background-color: #3346c9;
        }
        #result {
            margin-top: 20px;
            font-size: 18px;
            color: #f0da23;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Gacha random number</h1>
        <button onclick="generateRandomNumber()">An bo may di!</button>
        <p id="result"></p>
    </div>
    <script>
        function generateRandomNumber() {
            document.getElementById("result").innerText = "tutudangbocso...";
            setTimeout(() => {
                const randomNumber = Math.floor(Math.random() * 1000) + 1;
                document.getElementById("result").innerText = `May da trung ${randomNumber}`;
            }, 450);
        }
    </script>
</body>
</html>
    </style>
<body>
    <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <style>
    body {
      margin: 0;
      height: 100vh;
      overflow: hidden;
      background-color: #f0f0f0;
      cursor: none; 
    }

    #circle {
      position: absolute;
      width: 30px;
      height: 30px;
      background-color: #d74141;
      border-radius: 50%;
      pointer-events: none;
      transform: translate(-50%, -50%);
    }
  </style>
</head>
<body>
  <div id="circle"></div>

  <script>
    const circle = document.getElementById('circle');

    document.addEventListener('mousemove', (e) => {
      circle.style.left = e.clientX + 'px';
      circle.style.top = e.clientY + 'px';
    });
  </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <style>
    body {
      margin: 0;
      height: 100vh;
      background-color: #f9f9f9;
    }

    #clock {
      position: fixed;
      bottom: 10px;
      left: 10px;
      background-color: black;
      color: white;
      font-family: monospace;
      font-size: 20px;
      padding: 10px 15px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
      user-select: none;
    }
  </style>
</head>
<body>
  <div id="clock">--:--:--</div>

  <script>
    function updateClock() {
      const now = new Date();
      const hours = now.getHours().toString().padStart(2, '0');
      const minutes = now.getMinutes().toString().padStart(2, '0');
      const seconds = now.getSeconds().toString().padStart(2, '0');
      document.getElementById('clock').textContent = `${hours}:${minutes}:${seconds}`;
    }

    setInterval(updateClock, 0500); 
    updateClock(); 
  </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <style>
    body {
      margin: 0;
      height: 100vh;
      background-color: #f0f0f0;
      overflow: hidden;
    }

    .click-image {
      position: absolute;
      width: 80px;
      height: 80px;
      pointer-events: none;
      transform: translate(-50%, -50%);
      transition: opacity 0.3s ease;
      opacity: 1;
    }
  </style>
</head>
<body>

  <script>
    document.addEventListener('click', (e) => {
      const img = document.createElement('img');
      img.src = 'https://tse1.mm.bing.net/th?id=OIP.ibZ4hLFP9S8ICwdC7O-bggHaHa&pid=Api&P=0&h=220';
      img.className = 'click-image';
      img.style.left = `${e.clientX}px`;
      img.style.top = `${e.clientY}px`;

      document.body.appendChild(img);

      setTimeout(() => {
        img.style.opacity = '0';
        setTimeout(() => {
          img.remove();
        }, 300);
      }, 700);
    });
  </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <style>
    body {
      margin: 0;
      padding: 0;
      transition: background 0.5s ease;
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center;
    }
    #toggleButton {
      position: fixed;
      top: 20px;
      right: 20px;
      padding: 10px 20px;
      font-size: 16px;
      background-color: #1e90ff;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      z-index: 1000;
    }
  </style>
</head>
<body>

<button id="toggleButton">On</button>

<audio id="backgroundMusic" src="breezy-escape-chill-background-music-271240.mp3"></audio>

<script>
  const button = document.getElementById('toggleButton');
  const audio = document.getElementById('backgroundMusic');
  let isPlaying = false;

  button.addEventListener('click', () => {
    if (!isPlaying) {
      audio.play();
      document.body.style.backgroundImage = "url('https://tophinhanhdep.com/wp-content/uploads/2021/10/Lofi-Gif-Wallpapers.gif')";
      button.textContent = 'Off';
      isPlaying = true;
    } else {
      audio.pause();
      document.body.style.backgroundImage = '';
      button.textContent = 'On';
      isPlaying = false;
    }
  });
</script>

</body>
</html>
