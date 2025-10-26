<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Smart URL Shortener</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f5f6fa;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .box {
      background: #fff;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      text-align: center;
      width: 90%;
      max-width: 400px;
    }
    input {
      width: 100%;
      padding: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
      margin-bottom: 10px;
    }
    button {
      padding: 10px 20px;
      border: none;
      background: #0066ff;
      color: white;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }
    .result {
      margin-top: 15px;
      font-weight: bold;
      color: #333;
    }
  </style>
</head>
<body>
  <div class="box">
    <h2>🔗 URL Shortener</h2>
    <input type="text" id="longUrl" placeholder="Enter your long URL..." />
    <button onclick="shortenUrl()">Shorten</button>
    <div class="result" id="result"></div>
  </div>

  <script>
    const FIREBASE_URL = "https://urlshortener-d1814-default-rtdb.asia-southeast1.firebasedatabase.app/";

    // Random short ID তৈরি
    function generateID(length = 5) {
      const chars = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789";
      return Array.from({length}, () => chars[Math.floor(Math.random() * chars.length)]).join('');
    }

    async function shortenUrl() {
      const longUrl = document.getElementById("longUrl").value.trim();
      if (!longUrl) {
        alert("Please enter a valid URL!");
        return;
      }

      const shortCode = generateID();
      const data = { longUrl, created: new Date().toISOString() };

      // Firebase এ সেভ করা
      await fetch(`${FIREBASE_URL}/links/${shortCode}.json`, {
        method: "PUT",
        headers: {"Content-Type": "application/json"},
        body: JSON.stringify(data)
      });

      const shortUrl = `${window.location.origin}${window.location.pathname.replace("index.html","")}redirect.html?c=${shortCode}`;
      document.getElementById("result").innerHTML = `✅ Short URL: <a href="${shortUrl}" target="_blank">${shortUrl}</a>`;
    }
  </script>
</body>
</html>
