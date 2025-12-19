# Ex.07 Restaurant Website
## Date:19-12-2025
## Ref no:25012095

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
~~~
home.html

<!DOCTYPE html>
<html>
<head>
    <title>Rooftop Restaurant</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<header>
    <h1>Rooftop Restaurant</h1>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section>
    <h2>Welcome to Rooftop Restaurant</h2>
    <p>Fresh vegetarian flavors, modern dining experience, and cozy vibes.</p>
</section>

</body>
</html>

menu.html

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Leafora Veg - Menu</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<header>
    <h1>Rooftop Restaurant</h1>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
     <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section>
    <h2>Our Menu</h2>
    <div class="menu-grid">
        <div class="card"><img src="idly.jpg"><p>Idly - ₹20</p></div>
        <div class="card"><img src="ice.jpg"><p>Ice cream - ₹15</p></div>
        <div class="card"><img src="chicken65-f.webp"><p>Chicken 65 - ₹180</p></div>
        <div class="card"><img src="chapathi.jpg"><p>Chapathi - ₹15</p></div>
        <div class="card"><img src="paneer.jpg"><p>Paneer Tikka - ₹200</p></div>
        <div class="card"><img src="veg-fried-rice.jpg"><p>Fried Rice - ₹170</p></div>
    </div>
</section>

</body>
</html>

admin.html

<!DOCTYPE html>
<html>
<head>
    <title>Rooftop Restaurant - Administration</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<header>
    <h1> Rooftop Restaurant  </h1> Restaurant</h1>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section>
    <h2>Meet Our Team</h2>
    <div class="team-grid">
        <div class="card"><img src="chef.jpg"><p>Person 1 - Head Chef</p></div>
        <div class="card"><img src="manager.jpg"><p>Person 2 - Manager</p></div>
    </div>
</section>

</body>
</html>

contact.html

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Rooftop Restaurant - Contact Us</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<header>
    <h1>Rooftop Restaurant</h1>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section>
    <div class="contact-container">
        <h2>Contact Us</h2>
        <p><b>Address:</b> 123 Blue street,Chennai, Tamil Nadu 600201</p>
        <p><b>Phone:</b> +91 9876543210</p>
        <p><b>Email:</b> contact@leafora.com</p>
        <p><b>Opening Hours:</b> Mon-Sun: 10:00 AM - 11:00 PM</p>
    </div>
</section>
</body>
</html>

index.css

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    background-color: #F2F8FF; /* light blue background */
    color: #0A2540; /* deep navy text */
}

/* Header */
header {
    background: linear-gradient(
        90deg,
        #d7f708,   /* dark yellow */
        #eaf077,   /* medium yellow*/
        #e0ee8d    /* light yellow */
    ); 
    color: #1a0101;
    padding: 22px;
    text-align: center;
    letter-spacing: 1px;
}

/* Navigation */
nav {
    background-color: #020b21; 
    text-align: center;
}

nav a {
    color: #ffffff;
    text-decoration: none;
    margin: 0 18px;
    padding: 10px;
    display: inline-block;
    font-weight: 600;
    transition: 0.3s ease;
}

nav a:hover {
    background-color: #4DA3FF; /* sky blue hover */
    color: #0A2540;
    border-radius: 6px;
}

/* Section */
section {
    padding: 40px;
    text-align: center;
}

/* Headings */
h2 {
    font-family: 'Courgette', cursive;
    color: #163A5F; /* rich blue */
    font-weight: 700;
    letter-spacing: 0.5px;
}

/* Grid Layout */
.menu-grid, .team-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
    max-width: 1000px;
    margin: 30px auto;
    text-align: center;
}

/* Cards */
.card {
    background-color: #f1f6f8;
    padding: 18px;
    border-radius: 14px;
    box-shadow: 0 9px 17px rgba(173, 5, 228, 0.12);
    color: #030357;
    font-weight: 600;
    border: 4px solid #1a32c7fc; 
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-6px);
}

/* Images */
.card img {
    width: 90px;
    height: 110px;
    object-fit: cover;
    border-radius: 18px;
}

/* Footer */
footer {
    background-color: #0A2540;
    color: #ffffff;
    text-align: center;
    padding: 18px;
    font-size: 14px;
    letter-spacing: 0.5px;
}

/* Contact Section */
.contact-container {
    max-width: 800px;
    margin: 0 auto;
    text-align: left;
    padding: 25px;
    background-color: #ffffff;
    border-radius: 14px;
    box-shadow: 0 8px 18px rgba(0,0,0,0.12);
    border: 6px dashed #a50bd8; 
}


.contact-container h2 {
    text-align: center;
    color: #0A2540;
}

.contact-container p {
    font-size: 18px;
    margin: 12px 0;
    color: #163A5F;
}

.contact-container b {
    color: #0A2540;
}
.logo {
  border: 3px solid #0a0a0a00;
  padding: 15px;
  border-radius: 15px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}
~~~




## OUTPUT:
<img width="1919" height="1067" alt="Screenshot 2025-12-19 114805" src="https://github.com/user-attachments/assets/13820c52-51bd-4380-9eba-29e61f7a43d5" />
<img width="1919" height="1079" alt="Screenshot 2025-12-19 114349" src="https://github.com/user-attachments/assets/24bcf355-5f8a-4324-97d5-551fdc57e205" />
<img width="1919" height="1079" alt="Screenshot 2025-12-19 114701" src="https://github.com/user-attachments/assets/08064ecf-41ed-48e9-b119-b090929fee78" />
<img width="1919" height="1079" alt="Screenshot 2025-12-19 114719" src="https://github.com/user-attachments/assets/bc54b4fe-d0dc-403e-bc88-1b29df7aff89" />
<img width="1919" height="1079" alt="Screenshot 2025-12-19 114728" src="https://github.com/user-attachments/assets/30094cb3-275a-4ab2-a552-0739f24672ff" />


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
