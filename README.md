# Ex04 Places Around Me
# Date:30.09,2025
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE:
my city 
```
<html>
<head>
<title>My City</title>
</head>
<body>
<h1 align="center">
<font color="red"><b>Gingee</b></font>
</h1>
<h3 align="center">
<font color="blue"><b>DHIVYASHREE .R (25016639)</b></font>
</h3>
<center>
<img src="map (2).png" usemap="my city" height="610" width="1450"                                   
<map name="MyCity">
<area shape="rect" coords="700,250,850,400," href="home.html" title="My Home Town">
<area shape="circle"coords="570,230,45" href="temple.html" tittle="sri arulmigu karumari amman temple">
<area shape="circle"coords="640,200,30"href="lake.html" tittle="koladi lake">
<area shape="circle"coords="1120,360,25" href="garden.html"tittle="rmk chola garden">
<area shape="rect"coords="950,120,1100,140" href="stone.html"tittle="DR.B.R ambedkarstatue">
</map>
</center>
</body>
</html>
```
temple .html
```
temple.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Sri Arulmigu Karumari Amman Temple</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Poppins', sans-serif; scroll-behavior: smooth; }
    body { background: #fff8f0; color: #4a2c0f; }
    header { background: linear-gradient(90deg, #fbb034, #ffdd00); padding: 20px 0; text-align: center; position: sticky; top: 0; z-index: 1000; box-shadow: 0 4px 10px rgba(0,0,0,0.1); }
    header h1 { font-size: 2.5rem; color: #6b3e0a; text-shadow: 1px 1px 3px #b37400; }
    nav a { margin: 0 15px; text-decoration: none; color: #6b3e0a; font-weight: 600; }
    nav a:hover { color: #ff6700; }

    .hero { background: url('https://upload.wikimedia.org/wikipedia/commons/3/3a/Karumari_Amman_temple_entrance.jpg') center/cover no-repeat; height: 400px; display: flex; justify-content: center; align-items: center; color: #fff; text-shadow: 2px 2px 6px #4a2c0f; }
    .hero h2 { background: rgba(255, 221, 0, 0.8); padding: 20px 40px; border-radius: 10px; font-size: 2.5rem; }

    section { max-width: 800px; margin: 40px auto; padding: 20px; background: #fff5d6; border-radius: 15px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); }
    h3 { font-size: 2rem; color: #b35e00; margin-bottom: 15px; }
    p { font-size: 1.1rem; color: #5a3d0a; margin-bottom: 15px; line-height: 1.7; text-align: justify; }

    .contact-form { background: #fff3db; padding: 25px; border-radius: 15px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); }
    .contact-form input, .contact-form textarea { width: 100%; padding: 12px; margin-bottom: 15px; border: 2px solid #ffbb00; border-radius: 10px; font-size: 1rem; }
    .contact-form button { background: #ffbb00; padding: 12px 30px; border: none; border-radius: 10px; font-weight: bold; color: #6b3e0a; cursor: pointer; }
    .contact-form button:hover { background: #fbb034; }

    footer { text-align: center; background: #6b3e0a; color: white; padding: 15px; font-size: 0.95rem; margin-top: 40px; }
  </style>
</head>
<body>

  <header>
    <h1>Sri Arulmigu Karumari Amman Temple</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#history">History</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <h2>Divine Blessings & Eternal Peace</h2>
  </section>

  <section id="about">
    <h3>About the Temple</h3>
    <p>Sri Arulmigu Karumari Amman Temple is dedicated to the Goddess Karumari Amman, known for her compassion and divine protection. It's a symbol of devotion and spiritual energy in the region.</p>
    <div style="text-align:center;">
      <img src="temple.jpeg" alt="Temple Image" style="max-width: 100%; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1);" />
    </div>
  </section>

  <section id="history">
    <h3>Temple History</h3>
    <p>The temple dates back centuries and features beautiful Dravidian architecture. It's a hub of cultural festivals and religious unity, especially during events like Panguni Uthiram and Navaratri.</p>
    <p>Legends tell of divine miracles and blessings here. Locals and visitors alike speak of peace, devotion, and community spirit surrounding the temple.</p>
  </section>

  <section id="contact">
    <h3>Contact Us</h3>
    <form class="contact-form" action="#" method="POST">
      <input type="text" name="name" placeholder="Your full name" required />
      <input type="email" name="email" placeholder="Your email address" required />
      <textarea name="message" rows="4" placeholder="Your message..." required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    &copy; 2025 Sri Arulmigu Karumari Amman Temple. All rights reserved.
  </footer>

</body>
</html>
```
lake.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Koladi Lake</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;700&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Roboto', sans-serif; }
    body {
      background: #e6f0ff; color: #003366; line-height: 1.6;
      min-height: 100vh; display: flex; flex-direction: column;
    }
    header, footer {
      background: #1e40af; color: #fff; text-align: center;
      padding: 20px; box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }
    header h1 { font-size: 2.5rem; }
    main {
      flex: 1; max-width: 800px; margin: 30px auto;
      background: #fff; padding: 25px; border-radius: 15px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
    }
    h2 {
      font-size: 2rem; margin-bottom: 20px;
      color: #1e3a8a; border-bottom: 2px solid #3b82f6;
      padding-bottom: 10px;
    }
    p {
      margin-bottom: 20px; font-size: 1.1rem;
      text-align: justify; color: #1e3a8a;
    }
    .image-container {
      text-align: center; margin-bottom: 25px;
    }
    img {
      max-width: 100%; border-radius: 10px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
      transition: transform 0.3s ease;
    }
    img:hover { transform: scale(1.03); }
    footer { font-size: 0.9rem; }
    @media (max-width: 600px) {
      header h1 { font-size: 1.8rem; }
      h2 { font-size: 1.5rem; }
      p { font-size: 1rem; }
    }
  </style>
</head>
<body>

  <header>
    <h1>Koladi Lake</h1>
  </header>

  <main>
    <div class="image-container">
      <img 
        src="lake.jpg"
        alt="Koladi Lake" 
        loading="lazy"
      />
    </div>

    <h2>History of Koladi Lake</h2>
    <p>
      Koladi Lake, located on the outskirts of Mumbai, India, is a serene and picturesque water body surrounded by lush greenery and hills. Historically, it served as an important water source for the local communities and played a vital role in sustaining the ecology of the region. Over the years, the lake has become a popular spot for nature lovers and trekkers looking for a peaceful escape from the bustling city.
    </p>
    <p>
      The lake's natural beauty is complemented by the surrounding Sahyadri hills, which provide breathtaking views and a rich habitat for various species of flora and fauna. Efforts have been made in recent years to preserve the lake’s pristine environment, balancing tourism with ecological conservation. Visitors are drawn not only by the calm waters but also by the hiking trails and picnic spots nearby.
    </p>
    <p>
      Koladi Lake holds cultural significance as well, with occasional local festivals celebrating the natural bounty of the area. The lake remains a symbol of Mumbai's harmonious coexistence of urban life and nature’s tranquility.
    </p>
  </main>

  <footer>
    &copy; 2025 Koladi Lake. All rights reserved.
  </footer>

</body>
</html>
```
garden.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>RMK Cholan Garden</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;700&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Montserrat', sans-serif; }
    body {
      background: #e6f4ea; color: #1b3a2d;
      display: flex; flex-direction: column; min-height: 100vh;
    }
    header, footer {
      background: #2a7a3d; color: #fff; text-align: center;
      padding: 20px; box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }
    header h1 { font-size: 2.5rem; }
    main {
      flex: 1; max-width: 800px; margin: 30px auto;
      background: #fff; padding: 25px; border-radius: 15px;
      box-shadow: 0 8px 25px rgba(0,0,0,0.1);
    }
    h2 {
      font-size: 2rem; color: #2a7a3d;
      margin-bottom: 20px; border-bottom: 2px solid #7ed56f;
      padding-bottom: 10px;
    }
    p {
      font-size: 1.1rem; margin-bottom: 20px;
      text-align: justify; color: #1b3a2d;
    }
    .image-container {
      text-align: center; margin-bottom: 25px;
    }
    img {
      max-width: 100%; border-radius: 10px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.15);
      transition: transform 0.3s ease;
    }
    img:hover { transform: scale(1.03); }
    footer { font-size: 0.9rem; }
    @media (max-width: 600px) {
      header h1 { font-size: 2rem; }
      h2 { font-size: 1.6rem; }
      p { font-size: 1rem; }
    }
  </style>
</head>
<body>

  <header>
    <h1>RMK Cholan Garden</h1>
  </header>

  <main>
    <div class="image-container">
      <img src="garden.jpg" alt="RMK Cholan Garden" loading="lazy" />
    </div>
    <h2>About the Garden</h2>
    <p>
      Located at RMK Engineering College, the Cholan Garden is a peaceful green space for students and visitors to relax and recharge.
    </p>
    <p>
      It features native plants, clean pathways, and quiet seating areas — a symbol of harmony between nature and education.
    </p>
    <p>
      The garden also hosts cultural events and outdoor activities, promoting both sustainability and student well-being.
    </p>
  </main>

  <footer>
    &copy; 2025 RMK Cholan Garden. All rights reserved.
  </footer>

</body>
</html>
```
```
statue.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Dr. B.R. Ambedkar Statue - Thiruverkadu</title>
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@300;700&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Merriweather', serif; }
    body {
      background: linear-gradient(135deg, #283e51, #485563);
      color: #f0f0f0; line-height: 1.7;
      display: flex; flex-direction: column; min-height: 100vh;
    }
    body::before {
      content: ""; position: fixed; inset: 0;
      background: url('https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/Statue_of_Dr_Babasaheb_Ambedkar_at_Bhim_Gaatha_Park%2C_Bengaluru_02.JPG/1280px-Statue_of_Dr_Babasaheb_Ambedkar_at_Bhim_Gaatha_Park%2C_Bengaluru_02.JPG') no-repeat center/cover;
      opacity: 0.12; z-index: -1; filter: grayscale(40%) brightness(70%);
    }
    header {
      background: rgba(40, 62, 81, 0.85); padding: 25px 15px;
      text-align: center; box-shadow: 0 4px 15px rgba(0,0,0,0.5);
    }
    header h1 {
      font-size: 2.5rem; color: #ffde59;
      text-shadow: 1px 1px 5px #000;
    }
    main {
      max-width: 850px; margin: 40px auto; padding: 30px;
      background: rgba(40, 62, 81, 0.9); border-radius: 15px;
      box-shadow: 0 8px 25px rgba(0,0,0,0.7);
    }
    .image-container { text-align: center; margin-bottom: 25px; }
    .image-container img {
      width: 100%; max-width: 680px;
      border-radius: 12px; border: 3px solid #ffd54f;
      box-shadow: 0 10px 25px #ffde59aa;
      transition: 0.3s; cursor: pointer;
    }
    .image-container img:hover {
      transform: scale(1.05);
      box-shadow: 0 14px 35px #ffde59;
    }
    h2 {
      color: #ffd54f; font-size: 2rem;
      border-bottom: 2px solid #ffde59;
      margin-bottom: 20px; padding-bottom: 8px;
    }
    p {
      margin-bottom: 20px; text-align: justify;
      font-size: 1.1rem; color: #f0f0f0cc;
    }
    footer {
      background: #1c2b38; color: #ffde59;
      text-align: center; padding: 15px; font-size: 0.95rem;
      margin-top: auto; box-shadow: inset 0 3px 10px #000;
    }
    @media (max-width: 600px) {
      header h1 { font-size: 1.8rem; }
      main { margin: 25px 15px; padding: 20px; }
      h2 { font-size: 1.5rem; }
      p { font-size: 1rem; }
    }
  </style>
</head>
<body>

  <header>
    <h1>Dr. B.R. Ambedkar Statue - Thiruverkadu</h1>
  </header>

  <main>
    <div class="image-container">
      <img src="dr.ambedhkar.jpeg" alt="Dr. B.R. Ambedkar Statue in Thiruverkadu" loading="lazy" />
    </div>

    <h2>History of the Statue</h2>
    <p>The statue of Dr. B.R. Ambedkar in Thiruverkadu is a powerful symbol of social justice, honoring the architect of the Indian Constitution and a tireless advocate for the rights of marginalized communities.</p>
    <p>It commemorates his legacy, values of equality, and serves as a gathering place for events and reflection. The artistic design reflects his dignity and stands as an inspiration to all.</p>
  </main>

  <footer>
    &copy; 2025 Dr. B.R. Ambedkar Statue, Thiruverkadu. All rights reserved.
  </footer>

</body>
</html>
```
gnp palace.html
````
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>GPN Palace</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #e6f0ff;
    }

    header {
      background: linear-gradient(90deg, #0a3d62, #3c6382);
      color: white;
      padding: 20px;
      text-align: center;
      font-size: 24px;
      font-weight: bold;
    }

    .card {
      background-color: white;
      max-width: 700px;
      margin: 40px auto;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
    }

    .card img {
      width: 100%;
      border-radius: 8px;
      margin-bottom: 20px;
    }

    h2 {
      color: #0a3d62;
      margin-bottom: 10px;
    }

    p {
      line-height: 1.6;
      text-align: justify;
    }

    hr {
      border: none;
      height: 1px;
      background-color: #ccc;
      margin: 15px 0;
    }
  </style>
</head>
<body>

<header>GPN Palace</header>

<div class="card">
  <img src="gpn.webp" alt="GPN Palace Image">

  <h2>About GPN Palace</h2>
  <p>
    GPN Palace is a spacious and elegant marriage hall located in Thiruverkadu, Chennai. Known for its large seating capacity and premium facilities, it’s a preferred venue for weddings, receptions, and other grand celebrations.
  </p>

  <hr>

  <h2>History</h2>
  <p>
    Established over a decade ago, GPN Palace was designed to bring together tradition and modern comfort. Over the years, it has hosted hundreds of joyful occasions and continues to be a beloved destination for families and communities across Chennai.
  </p>
</div>

</body>
</html>
```

# OUTPUT
![![temple output](<Screenshot (18).png>)]
![temple output2](<Screenshot (19).png>)
![lake output](<Screenshot (20).png>)
![garden output](<Screenshot (21).png>)
![statue output](<Screenshot (22).png>)
![gpn palace](<Screenshot (38).png>)


# RESULT
The program for implementing image maps using HTML is executed successfully.
