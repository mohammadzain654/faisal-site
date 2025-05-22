# faisal-site
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Lovely Faisal</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      text-align: center;
      background: linear-gradient(to right, #c9d6ff, #e2e2e2);
      min-height: 100vh;
      padding: 60px 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
    }

    h1 {
      font-size: 2.5rem;
      color: #2c3e50;
      margin-bottom: 30px;
    }

    button, .whatsapp-button {
      padding: 12px 28px;
      font-size: 18px;
      background: #ad0a8a;
      color: #fff;
      border: none;
      border-radius: 30px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
      cursor: pointer;
      transition: background 0.3s ease, transform 0.2s;
      text-decoration: none;
      margin: 10px 0;
      display: inline-block;
    }

    button:hover, .whatsapp-button:hover {
      background: #b01080;
      transform: scale(1.05);
    }

    #myImage {
      opacity: 0;
      display: none;
      margin-top: 30px;
      width: 320px;
      max-width: 90%;
      border-radius: 16px;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
      transition: opacity 1s ease-in;
    }

    #myImage.show {
      display: block;
      opacity: 1;
    }
  </style>
</head>
<body>

  <h1>Click the Button to See a Sweet Guy</h1>
  <button onclick="showImage()">Show Tommy</button>

  <!-- WhatsApp Button -->
  <a href="https://wa.me/923452132818" target="_blank" class="whatsapp-button">
    Message on WhatsApp
  </a>

  <img
    id="myImage"
    src="https://i.postimg.cc/j50GS3JD/Ggkuqo.jpg"
    alt="Uploaded Image"
  >

  <script>
    function showImage() {
      const img = document.getElementById('myImage');
      img.style.display = 'block';
      setTimeout(() => {
        img.classList.add('show');
      }, 10);
    }
  </script>

</body>
</html>
