# Ex.07 Restaurant Website
## Date:16-10-2025

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
home.html
```
<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Courgette&family=Merienda:wght@300..900&display=swap" rel="stylesheet">
    <title>VIZZ RESTAURANT</title>
    <style>
        body {
            margin: 0;
            font-family: 'Merienda', cursive;
            background: url('backgroundrest.jpg') no-repeat center center fixed;
            background-size: cover;
            color: rgb(234, 245, 16);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        header {
            text-align: center;
            padding: 50px 20px;
            background: rgba(0, 0, 0, 0.5);
            border-bottom: 2px solid goldenrod;
        }

        header h1 {
            font-size: 80px;
            letter-spacing: 10px;
            margin: 0;
            text-shadow: 2px 2px 8px black;
        }

        nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(0, 0, 0, 0.7); 
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.5);
            z-index: 1000;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 10px 20px;
            display: flex;
            justify-content: center;
        }

        nav li {
            margin: 0 20px;
        }

        nav a {
            text-decoration: none;
            color:azure;
            font-size: 18px;
            font-weight: 600;
            padding: 10px 20px;
            border-radius: 5px;
        }

        

        main {
            flex: 1;
            padding: 40px;
            text-align: center;
            background: rgba(255, 255, 255, 0.1); 
            margin: 20px auto;
            max-width: 900px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.7);
            animation: fadeInUp 1.5s ease-in-out;
        }

        main p {
            font-size: 24px;
            font-weight: 400;
            line-height: 1.5;
            color:rgb(244, 244, 247);
            text-shadow: 1px 1px 3px black;
        }

        footer {
            background: rgba(0, 0, 0, 0.8); 
            color: white;
            text-align: center;
            padding: 20px 0;
            border-top: 2px solid greenyellow;
            box-shadow: 0 -4px 6px rgba(0, 0, 0, 0.5);
        }

        footer p {
            margin: 5px 0;
            font-size: 16px;
        }

        footer a {
            color: goldenrod;
            text-decoration: none;
            margin: 0 10px;
            font-size: 18px;
            transition: color 0.3s ease-in-out;
        }

        footer a:hover {
            color: #d4af37;
        }

       
    </style>
</head>
<body>
    <header>
        <h1>ANIME RESTAURANT!!!!!</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#" title="Home">Home</a></li>
            <li><a href="menu.html" title="menu">menu</a></li>
            <li><a href="admin.html" title="admin">Administration</a></li>
            <li><a href="contact.html" title="Contact Us">Contact Us</a></li>
        </ul>
    </nav>
    <main>
        <p>...Welcome to anime Restaurant... </p>
        <p>This the place for party</p>
    </main>
    <footer>
        <p>&copy; 2025 anime Restaurant | Designed by: <b>SANTHOSH and FAMILY</p>
        <p>
            <a href="#" title="Facebook">Facebook</a> |
            <a href="#" title="Twitter">Twitter</a> |
            <a href="#" title="Instagram">Instagram</a>
        </p>
    </footer>
</body>
</html>
```
menu.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu Arena</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg,yellow, #e0e0e0);
            color: #333;
        }
        header {
            background-color:crimson;
            color: white;
            padding: 20px 0;
            text-align: center;
            box-shadow: rgba(0, 0, 0, 0.3);
        }
        header h1 {
            margin: 0;
            font-size: 48px;
        }
        header p {
            font-size: 18px;
            margin-top: 5px;
            font-weight: lighter;
        }
        .menu-section {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }
        .menu-section h2 {
            text-align: center;
            margin-bottom: 20px;
            font-size: 32px;
            color: #2a008b;
            border-bottom: 3px solid #ddd;
            display: inline-block;
            padding-bottom: 5px;
        }
        .menu-grid {
            display: flex;
            gap: 30px;
        }
        .menu-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .menu-item:hover {
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }
        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .menu-item h3 {
            margin: 15px 0 10px;
            font-size: 18px;
            color: #333;
        }
        .menu-item p {
            color: #555;
            font-size: 12px;
            margin: 0 10px 15px;
        }
        .menu-item .price {
            font-weight: bold;
            font-size: 15px;
            color: #33008b;
            margin-bottom: 15px;
        }
        footer {
            text-align: center;
            padding: 15px 0;
            background-color: #333;
            color: white;
            margin-top: 40px;
        }
    </style>
</head>
<body>

<header>
    <h1>Delicious food</h1>
    <p>Your favorite spot for authentic Indian non-veg meals</p>
</header>

<div class="menu-section">
    <h2>Chicken</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="biriyani.jpg" alt="biriyani">
            <h3>biriyani</h3>
            <p>Fragrant rice cooked with chicken, spices, and herbs.</p>
            <div class="price">₹150</div>
        </div>
        <div class="menu-item">
            <img src="chicken stick.jpg" alt="chicken stick">
            <h3>chicken stick</h3>
            <p>Slow-cooked mutton with aromatic</p>
            <div class="price">₹350</div>
        </div>
        <div class="menu-item">
            <img src="chiili chicken.jpg" alt="chicken 65">
            <h3>chicken 65</h3>
            <p>slow cook and moisture</p>
            <div class="price">₹300</div>
        </div>
        <div class="menu-item">
            <img src="tahnduri.jpg" alt="thanduri">
            <h3>thanduri</h3>
            <p>full chicken boiled slowly in fire</p>
            <div class="price">₹250</div>
        </div>
        <div class="menu-item">
            <img src="muuton .jpg" alt="mutton">
            <h3>mutton</h3>
            <p>A simple, aromatic  dish cooked in fire.</p>
            <div class="price">₹100</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Veg</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="dosa.jpg" alt="Crispy dosa">
            <h3>Crispy Dosa</h3>
            <p>Rostted in brownish color</p>
            <div class="price">₹180</div>
        </div>
        <div class="menu-item">
            <img src="idly.jpg" alt="idli">
            <h3>idli</h3>
            <p>So soft</p>
            <div class="price">₹50</div>
        </div>
        <div class="menu-item">
            <img src="meals.jpg" alt="meals">
            <h3>meals</h3>
            <p>Delicious and type of food</p>
            <div class="price">₹280</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Desert and sweets</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="desert.jpg" alt="Desert">
            <h3>Desert</h3>
            <p>Must Finish with Desert.</p>
            <div class="price">₹220</div>
        </div>
        
        
        <div class="menu-item">
            <img src="juice.jpg" alt="juice">
            <h3>juice</h3>
            <p>Different type of juice</p>
            <div class="price">₹70</div>
        </div>
    </div>
</div>

<footer>
    <p>&copy; 2025 Delicious Indian Bites. All rights reserved.</p>
</footer>

</body>
</html>
```
admin.html
```
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chefs</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@700&family=Pacifico&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-color:yellow;
        }

        header {
            text-align: center;
            background-color: #0e6ff5;
            padding: 20px 0;
        }

        header h1 {
            font-family: "Caveat", cursive;
            font-size: 50px;
            color: white;
            margin: 0;
        }


        .chefs-container {
            display: flex;
            gap: 20px;
            padding: 40px;
            margin: auto;
        }

        .chef-card {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
        }

        .chef-card:hover {
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .chef-card img {
            width: 100%;
            object-fit: contain; 
            max-height: 300px; 
        }

        .chef-details {
            padding: 200px;
        }

        .chef-details h1 {
            font-size: 35px;
            margin-left:-200px;
            color: rgb(181, 101, 29);
           
        }

        .chef-details h2,
        .chef-details h3 {
            font-size: 20px;
            color: rgb(85, 85, 85);
            margin-left: -150px ;
        }

       
        footer {
            text-align: center;
            background-color:aliceblue;
            color:brown;
            padding: 20px 0;
            margin-top: 20px;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>

  
    <header>
        <h1>Cooking chef</h1>
    </header>

    
    <div class="chefs-container">
        <div class="chef-card">
            <img src="chef 3.jpg" alt="Chef harish">
            <div class="chef-details">
                <h1>Mr.Harish</h1>
                <h2>Designation: Sous Chef</h2>
                <h3>Experience: 6 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="chef 1.jpg" alt="Chef Venkat">
            <div class="chef-details">
                <h1>Mr. Vennkat</h1>
                <h2>Designation: Executive Chef</h2>
                <h3>Experience: 7 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="chef 2.jpg" alt="Chef koushik">
            <div class="chef-details">
                <h1>Mr. koushik</h1>
                <h2>Designation: Saucier Chef</h2>
                <h3>Experience: 2 years</h3>
            </div>
        </div>
        
        </div>

        
        
    </div>
    
   
    <footer>
        <p>&copy; 2025 Foodie's Paradise. All rights reserved.</p>
    </footer>

</body>
</html>
```
contact.html
```
<html>
    <head>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&display=swap" rel="stylesheet">
        <title>Contact Us</title>
        <style>
            #n1{
                position: relative;
                color:chartreuse;
                font-size: 60px;
                padding-left: 380px;
                left: 0px;
                top: 190px;
                letter-spacing: 5px;
            }
            body{
                background-image: url("contact.jpg");
                background-repeat: no-repeat;
                background-size: 1700px 950px;
            }
            #n2{
                position:relative;
                color: rgb(16, 5, 102);
                font-size: 80px;
                padding-left: 480px;
                top: 140px;
                letter-spacing: 3px;
                font-family: "Dancing Script", cursive;
            }
            #n3{
                position: relative;
                color: rgb(11, 203, 100);
                font-size: 35px;
                top: 255px;
                padding-left: 240px;
            }
            #n4{
                position: relative;
                color:darkmagenta;
                font-size:31px;
                top: 205px;
                padding-left: 170px;
                letter-spacing: 2px;
            }
            #n5{
                position: relative;
                color: rgb(14, 231, 17);
                font-size: 35px;
                top: 60px;
                padding-left: 680px;
            }
            #n6{
                position: relative;
                color:crimson;
                font-size:35px;
                top: 8px;
                padding-left: 505px;
            }
            #n7{
                position: relative;
                color: rgb(20, 222, 54);
                font-size: 35px;
                bottom: 135px;
                padding-left: 1155px;
            }
            #n8{
                position: relative;
                color:darksalmon;
                font-size: 31px;
                bottom: 187px;
                padding-left: 950px;
                text-align: center;
            }

           
            a {
                color:hotpink;
                text-decoration: none;
                cursor: pointer;
            }

      
            a:hover {
                text-decoration: underline;
            }
            
        </style>
    </head>
    <body>
        <h1 id="n1">With Your Love And Kindness</h1>
        <h2 id="n2">Quality and Taste</h2>
        <h5 id="n3">Phone:</h5>
        <h5 id="n4">
            <a href="tel:+918896871265">+91 8854623514</a>
        </h5>
        <h5 id="n5">Email:</h5>
        <h5 id="n6">
            <a href="mailto:animerestaurant@gmail.com"><b>animerestaurant@gmail.com</b></a>
        </h5>
        <h5 id="n7">Location:</h5>
        <h5 id="n8">
            <a href="anime restarurant"><b> anime restaurant in chennai-600 035</b></a>
        </h5>
    </body>
</html>
```

## OUTPUT:
<img width="1919" height="1013" alt="Screenshot 2025-10-16 100426" src="https://github.com/user-attachments/assets/8cd197dc-be22-4ddb-b8fd-79413bc0438a" />
<img width="1913" height="1015" alt="Screenshot 2025-10-16 100451" src="https://github.com/user-attachments/assets/34370956-ed8e-4754-bc99-a813744a4da6" />
<img width="1915" height="1011" alt="Screenshot 2025-10-16 100523" src="https://github.com/user-attachments/assets/e5fdccdb-02cc-4c36-b042-42fb2eaa9f52" />
<img width="1919" height="1007" alt="Screenshot 2025-10-16 100542" src="https://github.com/user-attachments/assets/16cc76c5-34c7-46a4-b389-c9170a240f56" />

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
