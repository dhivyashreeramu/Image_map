# Ex04 Places Around Me
# Date:26.09.2025
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

# CODE
```
map.html
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
````
```
temple.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Sri Arulmigu Karumari Amman Temple</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap');

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: #fff8f0;
      color: #4a2c0f;
      line-height: 1.7;
      scroll-behavior: smooth;
    }

    header {
      background: linear-gradient(90deg, #fbb034, #ffdd00);
      padding: 25px 0;
      text-align: center;
      box-shadow: 0 4px 15px rgba(0,0,0,0.15);
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    header h1 {
      font-size: 3rem;
      color: #6b3e0a;
      letter-spacing: 3px;
      text-shadow: 1.5px 1.5px 5px #b37400;
      transition: color 0.3s ease;
    }

    header h1:hover {
      color: #ff6700;
    }

    nav {
      margin-top: 15px;
    }

    nav a {
      color: #6b3e0a;
      margin: 0 20px;
      text-decoration: none;
      font-weight: 600;
      font-size: 1.15rem;
      padding: 8px 12px;
      border-radius: 6px;
      transition: background-color 0.3s ease, color 0.3s ease;
    }

    nav a:hover {
      background-color: #ffbb00;
      color: #4a2c0f;
      box-shadow: 0 0 8px #ffbb00;
    }

    .hero {
      background: url('https://upload.wikimedia.org/wikipedia/commons/3/3a/Karumari_Amman_temple_entrance.jpg') center/cover no-repeat;
      height: 450px;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      text-shadow: 3px 3px 10px #4a2c0f;
      animation: fadeInHero 2s ease forwards;
    }

    @keyframes fadeInHero {
      from {
        opacity: 0;
        transform: translateY(40px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .hero h2 {
      font-size: 3.5rem;
      background: rgba(255, 221, 0, 0.85);
      padding: 25px 50px;
      border-radius: 15px;
      font-weight: 700;
      box-shadow: 0 5px 15px rgba(181, 117, 0, 0.5);
      letter-spacing: 2px;
      max-width: 90%;
      text-align: center;
    }

    section {
      max-width: 900px;
      margin: 50px auto;
      padding: 0 25px;
      background: #fff5d6;
      border-radius: 20px;
      box-shadow: 0 8px 25px rgba(181, 117, 0, 0.15);
      animation: fadeInSection 1.5s ease forwards;
    }

    @keyframes fadeInSection {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    h3 {
      color: #b35e00;
      font-size: 2.4rem;
      margin-bottom: 25px;
      border-bottom: 4px solid #ffbb00;
      display: inline-block;
      padding-bottom: 8px;
      letter-spacing: 1.5px;
    }

    p {
      font-size: 1.18rem;
      margin-bottom: 25px;
      text-align: justify;
      color: #5a3d0a;
      line-height: 1.8;
    }

    footer {
      background: #6b3e0a;
      color: #fff;
      text-align: center;
      padding: 20px 10px;
      font-size: 1rem;
      margin-top: 60px;
      box-shadow: inset 0 5px 20px rgba(0,0,0,0.25);
    }

    /* Contact form */
    .contact-form {
      background: #fff3db;
      padding: 35px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(181, 117, 0, 0.25);
      max-width: 600px;
      margin: 0 auto 60px;
      transition: box-shadow 0.3s ease;
    }

    .contact-form:hover {
      box-shadow: 0 14px 40px rgba(255, 187, 0, 0.4);
    }

    .contact-form label {
      display: block;
      font-weight: 700;
      margin-bottom: 12px;
      color: #6b3e0a;
      font-size: 1.1rem;
      letter-spacing: 0.03em;
    }

    .contact-form input,
    .contact-form textarea {
      width: 100%;
      padding: 15px 18px;
      margin-bottom: 28px;
      border: 2.5px solid #ffbb00;
      border-radius: 12px;
      font-size: 1.1rem;
      font-family: 'Poppins', sans-serif;
      resize: vertical;
      color: #4a2c0f;
      transition: border-color 0.3s ease;
    }

    .contact-form input:focus,
    .contact-form textarea:focus {
      border-color: #fbb034;
      outline: none;
      box-shadow: 0 0 8px #fbb034;
    }

    .contact-form button {
      background: #ffbb00;
      border: none;
      padding: 18px 40px;
      font-size: 1.25rem;
      font-weight: 700;
      border-radius: 14px;
      cursor: pointer;
      color: #6b3e0a;
      box-shadow: 0 5px 15px rgba(255, 187, 0, 0.5);
      transition: background 0.4s ease, box-shadow 0.4s ease;
    }

    .contact-form button:hover {
      background: #fbb034;
      box-shadow: 0 8px 20px rgba(255, 170, 0, 0.8);
    }

    /* Responsive */
    @media (max-width: 600px) {
      header h1 {
        font-size: 2.2rem;
      }

      nav a {
        margin: 0 10px;
        font-size: 1rem;
      }

      .hero h2 {
        font-size: 2rem;
        padding: 15px 25px;
      }

      section {
        margin: 30px 15px;
        padding: 20px 15px;
      }

      h3 {
        font-size: 1.8rem;
      }

      .contact-form {
        padding: 25px 20px;
      }
    }
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
    <p>
      Sri Arulmigu Karumari Amman Temple is a revered place of worship dedicated to Goddess Karumari Amman,
      known for her compassion and protection. The temple stands as a beacon of spiritual strength and cultural heritage, attracting devotees from across the region.
    </p>
    <div style="text-align:center; margin-top: 30px;">
      <img src="temple.jpeg"
        alt="Sri Arulmigu Karumari Amman Temple Entrance" 
        style="max-width: 100%; height: auto; border-radius: 15px; box-shadow: 0 8px 25px rgba(181, 117, 0, 0.3);" 
      />
    </div>
  </section>

  <section id="about">
    <h3>About the Temple</h3>
    <p>
      Sri Arulmigu Karumari Amman Temple is a revered place of worship dedicated to Goddess Karumari Amman,
      known for her compassion and protection. The temple stands as a beacon of spiritual strength and cultural heritage, attracting devotees from across the region.
    </p>
  </section>

  <section id="history">
    <h3>Temple History</h3>
    <p>
      The Sri Arulmigu Karumari Amman Temple dates back over several centuries, rooted deeply in the traditions and culture of the Tamil people.
      It is believed that Goddess Karumari Amman is a fierce and benevolent deity who protects her devotees from evil and grants prosperity.
    </p>
    <p>
      The temple architecture is a beautiful example of Dravidian style, featuring intricate carvings and vibrant statues that depict various mythological stories.
      Every year, the temple attracts thousands of pilgrims, especially during the annual festival seasons such as Panguni Uthiram and Navaratri, when the deity is adorned with exquisite floral decorations and rituals are performed with great fervor.
    </p>
    <p>
      Local legends tell of miraculous events and divine interventions associated with the temple, making it a center of faith and spiritual energy.
      The temple committee actively preserves the heritage through restoration and cultural programs, maintaining the temple as a vital part of the community.
    </p>
    <p>
      Visitors to the temple often describe a serene atmosphere filled with chanting, the scent of incense, and the warm hospitality of the priests and locals.
      The temple also serves as a hub for various social and religious activities, fostering unity and devotion among people from all walks of life.
    </p>
  </section>

  <section id="contact">
    <h3>Contact Us</h3>
    <form class="contact-form" action="#" method="POST">
      <label for="name">Name</label>
      <input type="text" id="name" name="name" placeholder="Your full name" required />

      <label for="email">Email</label>
      <input type="email" id="email" name="email" placeholder="Your email address" required />

      <label for="message">Message</label>
      <textarea id="message" name="message" rows="5" placeholder="Write your message here..." required></textarea>

      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    &copy; 2025 Sri Arulmigu Karumari Amman Temple. All rights reserved.
  </footer>

</body>
</html>
```
```
lake.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Koladi Lake</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;700&display=swap');

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Roboto', sans-serif;
    }

    body {
      background: #e6f0ff;
      color: #003366;
      line-height: 1.6;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    header {
      background: linear-gradient(90deg, #1e40af, #3b82f6);
      padding: 30px 20px;
      text-align: center;
      box-shadow: 0 4px 15px rgba(0, 60, 130, 0.4);
      color: #fff;
    }

    header h1 {
      font-size: 3rem;
      letter-spacing: 2px;
      text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.3);
    }

    main {
      flex-grow: 1;
      max-width: 900px;
      margin: 40px auto;
      background: #ffffffcc;
      border-radius: 20px;
      padding: 30px 40px;
      box-shadow: 0 8px 30px rgba(59, 130, 246, 0.3);
      animation: fadeIn 1.5s ease forwards;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    h2 {
      color: #1e3a8a;
      font-size: 2.8rem;
      margin-bottom: 25px;
      border-bottom: 3px solid #3b82f6;
      padding-bottom: 10px;
      letter-spacing: 1.2px;
    }

    p {
      font-size: 1.15rem;
      color: #1e3a8a;
      margin-bottom: 28px;
      text-align: justify;
      line-height: 1.8;
    }

    .image-container {
      text-align: center;
      margin-bottom: 35px;
    }

    .image-container img {
      width: 100%;
      max-width: 700px;
      height: auto;
      border-radius: 15px;
      box-shadow: 0 10px 25px rgba(59, 130, 246, 0.4);
      transition: transform 0.4s ease;
      cursor: pointer;
    }

    .image-container img:hover {
      transform: scale(1.05);
      box-shadow: 0 14px 40px rgba(59, 130, 246, 0.7);
    }

    footer {
      background: #1e40af;
      color: #fff;
      text-align: center;
      padding: 18px 15px;
      font-size: 1rem;
      margin-top: auto;
      letter-spacing: 0.05em;
      box-shadow: inset 0 4px 15px rgba(0, 0, 80, 0.7);
    }

    /* Responsive */
    @media (max-width: 600px) {
      header h1 {
        font-size: 2.2rem;
      }

      main {
        margin: 30px 15px;
        padding: 25px 20px;
      }

      h2 {
        font-size: 2rem;
      }

      p {
        font-size: 1rem;
      }
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
```
garden.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>RMK Cholan Garden</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;700&display=swap');

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Montserrat', sans-serif;
    }

    body {
      background: #e6f4ea;
      color: #1b3a2d;
      line-height: 1.7;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    header {
      background: linear-gradient(90deg, #2a7a3d, #7ed56f);
      padding: 30px 20px;
      text-align: center;
      box-shadow: 0 4px 20px rgba(42, 122, 61, 0.5);
      color: #ffffff;
    }

    header h1 {
      font-size: 3rem;
      letter-spacing: 3px;
      text-shadow: 1.5px 1.5px 5px rgba(0,0,0,0.3);
    }

    main {
      flex-grow: 1;
      max-width: 900px;
      margin: 40px auto;
      background: #f7fff9cc;
      border-radius: 20px;
      padding: 30px 40px;
      box-shadow: 0 10px 30px rgba(46, 125, 50, 0.25);
      animation: fadeIn 1.5s ease forwards;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(25px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    h2 {
      color: #2a7a3d;
      font-size: 2.8rem;
      margin-bottom: 25px;
      border-bottom: 3px solid #7ed56f;
      padding-bottom: 10px;
      letter-spacing: 1.5px;
    }

    p {
      font-size: 1.15rem;
      color: #1b3a2d;
      margin-bottom: 28px;
      text-align: justify;
      line-height: 1.8;
    }

    .image-container {
      text-align: center;
      margin-bottom: 35px;
    }

    .image-container img {
      width: 100%;
      max-width: 700px;
      height: auto;
      border-radius: 15px;
      box-shadow: 0 10px 25px rgba(46, 125, 50, 0.35);
      transition: transform 0.4s ease;
      cursor: pointer;
    }

    .image-container img:hover {
      transform: scale(1.05);
      box-shadow: 0 14px 40px rgba(126, 213, 111, 0.7);
    }

    footer {
      background: #2a7a3d;
      color: #fff;
      text-align: center;
      padding: 18px 15px;
      font-size: 1rem;
      margin-top: auto;
      letter-spacing: 0.05em;
      box-shadow: inset 0 4px 15px rgba(0, 60, 0, 0.7);
    }

    /* Responsive */
    @media (max-width: 600px) {
      header h1 {
        font-size: 2.2rem;
      }

      main {
        margin: 30px 15px;
        padding: 25px 20px;
      }

      h2 {
        font-size: 2rem;
      }

      p {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>RMK Cholan Garden</h1>
  </header>

  <main>
    <div class="image-container">
      <img 
        src="garden.jpg"
        alt="RMK Cholan Garden" 
        loading="lazy"
      />
    </div>

    <h2>History of RMK Cholan Garden</h2>
    <p>
      RMK Cholan Garden is a beautifully maintained garden located within the RMK Engineering College campus. Established to provide a peaceful green space for students and visitors, the garden serves as a natural retreat where one can enjoy the calming effects of nature amid academic life.
    </p>
    <p>
      The garden features a variety of native and exotic plants, carefully arranged walkways, and serene seating areas. It reflects the institution’s commitment to environmental sustainability and the well-being of its community.
    </p>
    <p>
      Over the years, RMK Cholan Garden has become a popular spot for recreational activities, nature studies, and cultural events. It symbolizes harmony between education and nature, encouraging visitors to connect with the environment while nurturing their minds.
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
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@300;700&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Merriweather', serif;
    }

    body {
      background: linear-gradient(135deg, #283e51, #485563);
      color: #f0f0f0;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      line-height: 1.7;
    }

    body::before {
      content: "";
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      background: url('https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/Statue_of_Dr_Babasaheb_Ambedkar_at_Bhim_Gaatha_Park%2C_Bengaluru_02.JPG/1280px-Statue_of_Dr_Babasaheb_Ambedkar_at_Bhim_Gaatha_Park%2C_Bengaluru_02.JPG') no-repeat center center/cover;
      opacity: 0.12;
      z-index: -1;
      filter: grayscale(40%) brightness(70%);
    }

    header {
      background: rgba(40, 62, 81, 0.85);
      padding: 30px 20px;
      text-align: center;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);
    }

    header h1 {
      font-size: 3rem;
      letter-spacing: 3px;
      color: #ffde59;
      text-shadow: 2px 2px 6px #000000aa;
    }

    main {
      max-width: 900px;
      margin: 40px auto;
      background: rgba(40, 62, 81, 0.9);
      border-radius: 20px;
      padding: 30px 40px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.8);
      animation: fadeIn 1.5s ease forwards;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(25px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    h2 {
      color: #ffd54f;
      font-size: 2.8rem;
      margin-bottom: 25px;
      border-bottom: 3px solid #ffde59;
      padding-bottom: 12px;
      letter-spacing: 1.5px;
    }

    p {
      font-size: 1.2rem;
      margin-bottom: 28px;
      text-align: justify;
      color: #f0f0f0cc;
    }

    .image-container {
      text-align: center;
      margin-bottom: 35px;
    }

    .image-container img {
      width: 100%;
      max-width: 700px;
      height: auto;
      border-radius: 15px;
      box-shadow: 0 12px 30px #ffde59aa;
      transition: transform 0.3s ease;
      cursor: pointer;
      border: 4px solid #ffd54f;
    }

    .image-container img:hover {
      transform: scale(1.05);
      box-shadow: 0 16px 40px #ffde59ff;
    }

    footer {
      background: #1c2b38;
      color: #ffde59;
      text-align: center;
      padding: 18px 15px;
      font-size: 1rem;
      letter-spacing: 0.1em;
      box-shadow: inset 0 4px 15px #000000cc;
      margin-top: auto;
    }

    /* Responsive */
    @media (max-width: 600px) {
      header h1 {
        font-size: 2rem;
      }

      main {
        margin: 30px 15px;
        padding: 25px 20px;
      }

      h2 {
        font-size: 2rem;
      }

      p {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Dr. B.R. Ambedkar Statue - Thiruverkadu</h1>
  </header>

  <main>
    <div class="image-container">
      <img 
        src="dr.ambedhkar.jpeg"
        alt="Dr. B.R. Ambedkar Statue in Thiruverkadu" 
        loading="lazy"
      />
    </div>

    <h2>History of the Statue</h2>
    <p>
      The Dr. B.R. Ambedkar Statue in Thiruverkadu stands as a powerful symbol of social justice and equality, honoring one of India’s most influential leaders and social reformers. Dr. Bhimrao Ramji Ambedkar, often called the Father of the Indian Constitution, was a visionary who fought tirelessly against social discrimination and worked to uplift marginalized communities.
    </p>
    <p>
      This statue commemorates Dr. Ambedkar’s enduring legacy and his profound contributions to the Indian society, particularly in championing the rights of Dalits and advocating for universal education and legal reform. Located in Thiruverkadu, the statue serves not only as a memorial but also as an inspiration for generations to come.
    </p>
    <p>
      The site has become a place of gathering for social and cultural events, where people reflect on the values of equality, justice, and liberty that Dr. Ambedkar stood for. The statue's artistic design reflects his dignity and strength, making it a notable landmark in the region.
    </p>
  </main>

  <footer>
    &copy; 2025 Dr. B.R. Ambedkar Statue, Thiruverkadu. All rights reserved.
  </footer>

</body>
</html>
```

# OUTPUT
**mycity map**

<img width="1920" height="1021" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/38cbf28e-03c7-4c54-a122-56975e0c46af" />

**temple output**

<img width="1911" height="988" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/ea117a06-5226-44ea-aa43-0863c4089078" />
<img width="1920" height="1031" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/d358e2be-a971-487e-a454-39ccbb212def" />

**lake output**

<img width="1915" height="1024" alt="Screenshot (20)" src="https://github.com/user-attachments/assets/df7f2808-3f31-4088-a1a5-6e21e940f5b8" />

**garden output**

<img width="1920" height="1017" alt="Screenshot (21)" src="https://github.com/user-attachments/assets/e809eadb-18f8-4808-8323-43c96d429058" />

**statue output**


<img width="1920" height="1028" alt="Screenshot (22)" src="https://github.com/user-attachments/assets/62c23025-5ef4-4c77-9c18-3036ca1231af" />



# RESULT
The program for implementing image maps using HTML is executed successfully.
