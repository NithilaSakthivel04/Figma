# Ex09 Event Registration Web Application
## Date:20/05/2025
## Name:Nithila S
## Register Number:212224040224

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Art Contest Registration</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      text-align: center;
    }

    .screen {
      padding: 30px;
      min-height: 100vh;
      display: none;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background-size: cover;
      background-position: center;
    }

    .active {
      display: flex;
    }

    .home {
      background: url('https://i.imgur.com/VRNYfg6.jpg') no-repeat center center;
      background-size: cover;
      color: white;
    }

    .logo {
      width: 100px;
      margin-bottom: 20px;
    }

    .tagline {
      font-style: italic;
      margin-bottom: 20px;
    }

    .events {
      background: linear-gradient(to bottom, #d0eaff, #ffc0cb);
    }

    .events h2 {
      margin-bottom: 20px;
    }

    .events ol {
      text-align: left;
      font-size: 18px;
    }

    .form {
      background: url('https://i.imgur.com/WqfZ6Dr.jpg') no-repeat center center;
      background-size: cover;
    }

    .form h2 {
      margin-bottom: 20px;
      color: #000;
    }

    form input, form button {
      display: block;
      margin: 10px auto;
      padding: 10px;
      width: 80%;
      max-width: 300px;
      font-size: 16px;
      border-radius: 5px;
      border: none;
    }

    form button {
      background-color: black;
      color: white;
      cursor: pointer;
    }

    .thankyou {
      background: linear-gradient(to bottom, #5a189a, #b5179e);
      color: white;
      flex-direction: column;
    }

    .thankyou h2 {
      font-size: 28px;
      margin-bottom: 10px;
    }

    .thankyou p {
      font-size: 18px;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      margin-top: 20px;
      border: none;
      border-radius: 5px;
      background: #5a189a;
      color: white;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <!-- Screen 1: Home -->
  <section class="screen home active" id="home">
    <img src="https://i.imgur.com/C5xkYNR.png" alt="College Logo" class="logo" />
    <h1>Art Contest</h1>
    <p class="tagline">Shine your light & showcase your artwork!</p>
    <button onclick="showScreen('events')">Register</button>
  </section>

  <!-- Screen 2: Events -->
  <section class="screen events" id="events">
    <h2>EVENTS</h2>
    <ol>
      <li>Dream Doodles</li>
      <li>Sketchbox</li>
      <li>Craft Canvas</li>
      <li>Color Lab</li>
      <li>Inked Echoes</li>
      <li>Paint Perspectives</li>
    </ol>
    <button onclick="showScreen('form')">Next</button>
  </section>

  <!-- Screen 3: Form -->
  <section class="screen form" id="form">
    <h2>Event Registration Form</h2>
    <form onsubmit="submitForm(event)">
      <input type="text" placeholder="Full Name" required />
      <input type="number" placeholder="Age" required />
      <input type="text" placeholder="Gender" required />
      <input type="text" placeholder="Register Number" required />
      <input type="tel" placeholder="Mobile Number" required />
      <input type="text" placeholder="Department" required />
      <button type="submit">Register</button>
    </form>
  </section>

  <!-- Screen 4: Thank You -->
  <section class="screen thankyou" id="thankyou">
    <h2>Thank you for registering!</h2>
    <p>We are all eagerly waiting for your artwork!</p>
  </section>

  <script>
    function showScreen(screenId) {
      document.querySelectorAll(".screen").forEach(screen => {
        screen.classList.remove("active");
      });
      document.getElementById(screenId).classList.add("active");
    }

    function submitForm(event) {
      event.preventDefault();
      showScreen("thankyou");
    }
  </script>
</body>
</html>


## OUTPUT:

![alt text](image.png)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
