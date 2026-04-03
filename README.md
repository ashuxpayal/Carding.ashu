<!DOCTYPE html>
<html>
<head>
    <title>ASHU C4RDER</title>

    <style>
        body {
            background: BLACK;
            color: WHITE;
            text-align: center;
            font-family: Arial;
            margin: 0;
        }

        header {
            background: BLACK;
            padding: 15px;
            font-size: 22px;
            border-bottom: 1px solid RED;
        }

        nav {
            margin-top: 10px;
        }

        .btn {
            display: inline-block;
            margin: 10px;
            padding: 10px 20px;
            border: 2px solid RED;
            color: RED;
            text-decoration: none;
            border-radius: 10px;
            cursor: pointer;
        }

        .btn:hover {
            background: RED;
            color: BLACK;
        }

        section {
            display: none;
            padding: 20px;
        }

        #home {
            display: block;
        }

        .glow {
            color: RED;
            font-size: 35px;
            text-shadow: 0 0 10px RED, 0 0 20px RED;
        }

        .box {
            border: 1px solid RED;
            margin: 20px;
            padding: 20px;
            border-radius: 10px;
        }

        img {
            width: 250px;
            margin-top: 10px;
            border-radius: 10px;
        }

        footer {
            margin-top: 30px;
            padding: 10px;
            border-top: 1px solid RED;
        }
    </style>
</head>

<body>

<header>
    💳 ASHU C4RDER
</header>

<nav>
    <span class="btn" onclick="showSection('home')">HOME</span>
    <span class="btn" onclick="showSection('services')">SERVICES</span>
    <span class="btn" onclick="showSection('about')">ABOUT</span>
    <span class="btn" onclick="showSection('contact')">CONTACT</span>
    <span class="btn" onclick="showSection('careers')">STAFF</span>
</nav>

<!-- HOME -->
<section id="home">
    <h1>Premium c4rding Solutions</h1>
    <div class="glow">Welcome to ASHU C4RDER™</div>
    <p>Hello my name is Ashu or I am a carder and I am also doing IG Banning and free fire top-up 50% off If you are interested then contact me   </p>
</section>

<!-- SERVICES -->
<section id="services">
    <h1>Our Services</h1>

    <div class="box">
        <p onclick="showService('web')">💳 C4ARDING </p>
        <p onclick="showService('hack')">💻 INSTA BANNING </p>
        <p onclick="showService('data')">?</p>
    </div>

    <!-- Service Details -->
    <div id="serviceBox" style="display:none;">
        <h2 id="title"></h2>
        <img id="image">
        <p id="desc"></p>
    </div>
</section>

<!-- ABOUT -->
<section id="about">
    <h1>About Us</h1>
    <p>👉 We will give you the best service. Note :- No scam</p>
</section>

<!-- CONTACT -->
<section id="contact">
    <h1>Contact Us</h1>
    <p>📞 whatsapp:- 9919667539</p>
    <p>📧 Email: ashutosh.8887.my@email.com</p>
</section>

<!-- CAREERS -->
<section id="careers">
    <h1>Careers</h1>
    <p>👉  Staff Need:- If you want to work with us then message us on 
WhatsApp:- 9919667539</p>
</section>

<footer>
    © 2026 ASHU C4RDER
</footer>

<script>
function showSection(id) {
    let sections = document.querySelectorAll("section");
    sections.forEach(sec => sec.style.display = "none");

    document.getElementById(id).style.display = "block";
}

function showService(type) {
    document.getElementById("serviceBox").style.display = "block";

    if(type === 'web') {
        title.innerText = "50% OFF";
        image.src = "https://i.imgur.com/2DhmtJ4.jpg";
        desc.innerText = "I PROVIDE YOU BEST CARD.";
    }

    if(type === 'hack') {
        title.innerText = "INSTAGRAM ID BANNER";
        image.src = "https://i.imgur.com/Z6X9Z0F.jpg";
        desc.innerText = "PER ID BAN $15.";
    }

    if(type === 'data') {
        title.innerText = "?";
        image.src = "https://i.imgur.com/2DhmtJ4.jpg";
        desc.innerText = "?.";
    }
}
</script>

</body>
</html>
