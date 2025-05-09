<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Welcome to our Hotel</title>

  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&display=swap" rel="stylesheet" />
  <style>
    /* Base styles */
    body {
      display: flex;
      flex-direction: column;
      justify-content: flex-start; /* Align items at the top */
      align-items: center;
      margin: 0;
      padding: 0;
      height: 100vh; /* Full height of the viewport */
      background: linear-gradient(-45deg, black, #02bbf8, white);
      font-family: 'Playfair Display', serif;
      padding-left: 5vw; /* Horizontal padding */
      padding-right: 5vw; /* Horizontal padding */
    }

    .welcome-text {
      font-size: 6vw; /* Responsive font size based on viewport width */
      font-weight: 700;
      color: white;
      margin-top: 5vh; /* Margin at the top to give some space from the top of the screen */
      margin-bottom: 2vh; /* Space between the text and the image */
      text-align: center;
      text-shadow: 4px -4px 4px rgba(0, 0, 0, 0.5); /* Increased text shadow */
    }

    .image-container {
      background-color: antiquewhite;
      width: 80vw; /* Spans most of the screen width */
      height: 80vw; /* Make it square to maintain circular shape */
      border-radius: 50%; /* Circular container */
      overflow: hidden;
      position: relative;
      margin-bottom: 10vh; /* Margin to push it down from the next section */
      border: 2px solid white;
      box-shadow: 10px -20px 5px rgba(0, 0, 0, 0.5); /* Enhanced shadow */
    }

    .image-container img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      position: absolute;
      top: 0;
      left: 0;
    }

    /* Media Queries for Responsiveness */
    @media (max-width: 768px) {
      .welcome-text {
        font-size: 8vw; /* Larger text on smaller screens */
      }

      .image-container {
        width: 90vw; /* Full width for tablets */
        height: 90vw; /* Maintain circular aspect ratio */
      }
    }

    @media (max-width: 480px) {
      .welcome-text {
        font-size: 10vw; /* Larger text for very small devices */
      }

      .image-container {
        width: 95vw; /* Nearly full width on small screens */
        height: 95vw; /* Adjust height for very small devices */
      }
    }
  </style>
</head>
<body>

  <div id="curved-text" class="welcome-text">Welcome to our Hotel</div>
  <div class="image-container">
    <img src="https://raw.githubusercontent.com/abelbrhanegebreslasie/Frends/main/image/sss.jpg" alt="Hotel Image" />
  </div>

  <!-- CircleType.js for curved text -->
  <script src="https://cdn.jsdelivr.net/npm/circletype@2.3.0/dist/circletype.min.js"></script>
  <script>
    new CircleType(document.getElementById('curved-text')).radius(500);

    setTimeout(function() {
      window.location.href = 'https://abelbrhanegebreslasie.github.io/Frends/';
    }, 500000);
  </script>

</body>
</html>
