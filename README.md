# Ex.07 Restaurant Website
## Date:

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
HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Burger Restaurant</title>
    <link rel="stylesheet" href="STYLE.CSS">
</head>
<body>
    <header>
        <div class="logo">
            <h1>Burger Haven</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="hero-content">
            <h2>Welcome to Burger Haven!</h2>
            <p>The best burgers in town, made with fresh ingredients and a secret sauce!</p>
        </div>
    </section>

    <section id="menu" class="menu">
        <h2>Our Menu</h2>
        <div class="menu-items">
            <div class="menu-item">
                <img src="burger1.jpg" alt="Classic Burger">
                <h3>Classic Burger</h3>
                <p>A delicious beef patty with lettuce, tomato, and cheese.</p>
                <p class="price">$8.99</p>
            </div>
            <div class="menu-item">
                <img src="burger2.jpg" alt="Cheese Burger">
                <h3>Cheese Burger</h3>
                <p>Beef patty topped with cheddar cheese, pickles, and onions.</p>
                <p class="price">$9.49</p>
            </div>
            <div class="menu-item">
                <img src="burger3.jpg" alt="Veggie Burger">
                <h3>Veggie Burger</h3>
                <p>A healthy veggie patty with avocado, lettuce, and tomato.</p>
                <p class="price">$7.99</p>
            </div>
        </div>
    </section>

    <section id="about" class="about">
        <h2>About Us</h2>
        <p>At Burger Haven, we take pride in serving high-quality, fresh, and delicious burgers. We source our ingredients locally and make everything with love. Come taste the difference!</p>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Have any questions? Feel free to reach out!</p>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Burger Haven. All rights reserved.</p>
    </footer>
</body>
</html>

```
CSS
```

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #33dd2d;
    color: #333;
}

h1, h2, h3 {
    font-family: 'Arial', sans-serif;
}


header {
    background-color: #333;
    color: #fff;
    padding: 1rem 0;
    text-align: center;
    position: sticky;
    top: 0;
    z-index: 1000;
}

header .logo h1 {
    font-size: 2.5rem;
    letter-spacing: 2px;
}

header nav ul {
    list-style-type: none;
    padding: 0;
    margin: 1rem 0;
}

header nav ul li {
    display: inline;
    margin: 0 15px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    text-transform: uppercase;
}

.hero {
    background: url('hero-image.jpg') no-repeat center center/cover;
    height: 60vh;
    color: rgb(174, 15, 15);
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.hero h2 {
    font-size: 3rem;
}

.hero p {
    font-size: 1.2rem;
    max-width: 600px;
    margin: 0 auto;
}

.menu {
    padding: 4rem 2rem;
    text-align: center;
    background-color: #fff;
}

.menu h2 {
    font-size: 2.5rem;
    margin-bottom: 2rem;
}

.menu-items {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}

.menu-item {
    background-color: #f9f9f9;
    padding: 20px;
    margin: 15px;
    text-align: center;
    border-radius: 8px;
    width: 30%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.menu-item img {
    width: 100%;
    height: auto;
    border-radius: 8px;
}

.menu-item h3 {
    font-size: 1.8rem;
    margin-top: 1rem;
}

.menu-item p {
    font-size: 1rem;
    margin-top: 0.5rem;
}

.price {
    font-size: 1.2rem;
    font-weight: bold;
    color: #e67e22;
    margin-top: 0.5rem;
}


.about {
    padding: 3rem 2rem;
    text-align: center;
    background-color: #ececec;
}

.about h2 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.contact {
    padding: 4rem 2rem;
    background-color: #fff;
    text-align: center;
}

.contact form {
    max-width: 500px;
    margin: 0 auto;
    text-align: left;
}

.contact label {
    font-size: 1.2rem;
    display: block;
    margin: 10px 0 5px;
}

.contact input,
.contact textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.contact button {
    padding: 10px 20px;
    background-color: #333;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

.contact button:hover {
    background-color: #555;
}

footer {
    background-color: #333;
    color: white;
    padding: 1rem 0;
    text-align: center;
}

@media (max-width: 768px) {
    .menu-items {
        flex-direction: column;
        align-items: center;
    }

    .menu-item {
        width: 80%;
    }

    .hero h2 {
        font-size: 2rem;
    }

    .hero p {
        font-size: 1rem;
    }
}

```


## OUTPUT:
![Screenshot 2024-11-12 131425](https://github.com/user-attachments/assets/6d00dd59-bf26-4e96-b5f5-843de7631595)
![Screenshot 2024-11-12 131433](https://github.com/user-attachments/assets/b7c38f3d-daff-423b-a7db-7591d008ccf0)
![Screenshot 2024-11-12 131442](https://github.com/user-attachments/assets/40120e33-c1ba-4ff5-a9c2-e6f34c7a601a)




## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
