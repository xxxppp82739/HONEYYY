<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For Honey 💖</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: #ffb6c1;
      font-family: 'Courier New', monospace;
      overflow: hidden;
    }.message {
  text-align: center;
  font-size: 24px;
  color: #00bfff;
  animation: glowShift 4s infinite alternate;
  max-width: 80%;
  line-height: 1.6;
  white-space: pre-wrap;
}

@keyframes glowShift {
  0% {
    text-shadow:
      0 0 5px #00bfff,
      0 0 10px #1e90ff,
      0 0 20px #1e90ff,
      0 0 40px #00bfff;
  }
  100% {
    text-shadow:
      0 0 5px #ff69b4,
      0 0 10px #ff1493,
      0 0 20px #ff1493,
      0 0 40px #ff69b4;
  }
}

.cursor {
  display: inline-block;
  width: 10px;
  background: #00bfff;
  margin-left: 5px;
  animation: blink 1s infinite;
}

@keyframes blink {
  0%, 50%, 100% { opacity: 1; }
  25%, 75% { opacity: 0; }
}

  </style>
</head>
<body>  <div class="message" id="text"></div><div class="cursor"></div>  <script>
    const lines = [
      "I REALLY APPRECIATE WHAT WE HAVE,",
      "I LIKE BEING YOU'RE FRIEND,",
      "I HOPE WE CAN STAY FRIENDS FOREVER AND NEVER LOSE YOU",
      "",
      "- sincerely yours Angelo"
    ];

    const textElement = document.getElementById("text");
    let lineIndex = 0;
    let charIndex = 0;

    function typeLine() {
      if (lineIndex < lines.length) {
        if (charIndex < lines[lineIndex].length) {
          textElement.textContent += lines[lineIndex].charAt(charIndex);
          charIndex++;
          setTimeout(typeLine, 25); // faster typing
        } else {
          textElement.textContent += "\n";
          lineIndex++;
          charIndex = 0;
          setTimeout(typeLine, 700); // dramatic pause between lines
        }
      }
    }

    typeLine();
  </script></body>
</html># HONEYYY
