# SiriShapllo
<!DOCTYPE html>
<html lang="sq">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gjimnazi Siri Shapllo</title>
    <style>
        /* Stilet e përgjithshme */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            background-color: #f0f4f8;
            color: #333;
            transition: background-color 0.5s ease;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Stilet e Header */
        header {
            background-color: #2c3e50;
            padding: 15px 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
            transition: all 0.3s ease;
        }

        header.scrolled {
            padding: 10px 0;
            background-color: rgba(44, 62, 80, 0.95);
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo img {
            height: 50px;
            margin-right: 10px;
            border-radius: 50%;
        }

        .logo h1 {
            color: #fff;
            font-size: 1.5rem;
            font-weight: bold;
            font-family: 'Georgia', serif;
        }

        nav ul {
            display: flex;
            list-style: none;
            justify-content: center;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 600;
            letter-spacing: 1px;
            position: relative;
            padding: 5px 0;
            font-size: 1.1rem;
            transition: all 0.3s ease;
        }

        nav ul li a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background-color: #e74c3c;
            transition: width 0.3s ease;
        }

        nav ul li a:hover::after {
            width: 100%;
        }

        nav ul li a:hover {
            color: #e74c3c;
        }

        .active {
            color: #e74c3c !important;
        }

        .active::after {
            width: 100%;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .menu-toggle {
            display: none;
            flex-direction: column;
            cursor: pointer;
        }

        .menu-toggle span {
            display: block;
            width: 25px;
            height: 3px;
            background-color: #fff;
            margin: 3px 0;
            transition: all 0.3s ease;
        }

        /* ... (Rest of your CSS styles) ... */
        /* Stilet e Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(135deg, #3498db, #9b59b6);
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: #fff;
            position: relative;
            overflow: hidden;
            margin-top: 80px;
        }

        /* ... (Rest of your CSS styles) ... */

        /* Contact Section Styles */
        .contact {
            padding: 80px 0;
            background-color: #ffffff;
        }

        .contact-content {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
        }

        .contact-info {
            flex: 1;
            margin-right: 40px;
        }

        .contact-form {
            flex: 1;
        }

        .contact-info h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #2c3e50;
        }

        .contact-info p {
            margin-bottom: 10px;
        }

        .contact-form h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #2c3e50;
        }

        .contact-form form {
            display: flex;
            flex-direction: column;
        }

        .contact-form label {
            margin-bottom: 5px;
            font-weight: bold;
        }

        .contact-form input,
        .contact-form textarea {
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        .contact-form textarea {
            resize: vertical;
        }

        .contact-form button {
            padding: 10px 20px;
            background-color: #e74c3c;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .contact-form button:hover {
            background-color: #c0392b;
        }
    </style>
</head>

<body>
    <header>
        <div class="header-container">
            <div class="logo">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRHzYs5PSTnZOv6r8VvJ0grNsya4_tKsBrv4w&s" alt="Gjimnazi Siri Shapllo Logo">
                <h1>Gjimnazi Siri Shapllo</h1>
            </div>
            <div class="menu-toggle">
                <span></span>
                <span></span>
                <span></span>
            </div>
            <nav>
                <ul>
                    <li><a href="#" class="active">Kryefaqja</a></li>
                    <li><a href="#about">Rreth Nesh</a></li>
                    <li><a href="#features">Programet</a></li>
                    <li><a href="#testimonials">Studentët</a></li>
                    <li><a href="#contact">Kontakt</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Mirësevini në Gjimnazin Siri Shapllo</h1>
            <p>Një hapësirë ku dija, kreativiteti dhe vlerat njerëzore bashkohen për të formuar brezin e ri të liderëve të së ardhmes.</p>
            <a href="#about" class="btn">Zbulo më shumë</a>
        </div>
    </section>

    <section id="about" class="about">
        <div class="container">
            <div class="about-content">
                <div class="about-image">
                    <img src="" alt="Gjimnazi Siri Shapllo">
                </div>
                <div class="about-text">
                    <h2 class="section-title">Rreth Nesh</h2>
                    <p>Gjimnazi "Siri Shapllo" është një nga institucionet më të rëndësishme arsimore në vend, me një histori të pasur dhe traditë në arsim. Prej vitesh, ne kemi përgatitur studentë të suksesshëm të cilët kanë vazhduar studimet në universitetet më prestigjioze në
                        vend dhe jashtë.</p>
                    <p>Misioni ynë është të edukojmë dhe të frymëzojmë brezin e ri me vlera dhe njohuri të dobishme, duke i përgatitur ata për sfidat e së ardhmes. Ne besojmë në potencialin e çdo studenti dhe angazhohemi të zhvillojmë talentet e tyre unike.</p>
                    <p>Me një staf të kualifikuar dhe me përvojë, ne ofrojmë një mjedis të sigurt dhe stimulues për të mësuar, ku kreativiteti dhe mendimi kritik inkurajohen dhe vlerësohen.</p>
                    <a href="#features" class="btn">Programet tona</a>
                </div>
            </div>
        </div>
    </section>

    <div class="container">
        <div class="slideshow">
            <div class="slideshow-item active">
                <img src="/api/placeholder/1200/400" alt="Gjimnazi Siri Shapllo">
                <div class="slideshow-caption">
                    <h3>Ambientet moderne të mësimit</h3>
                    <p>Klasa të pajisura me teknologjinë më të fundit</p>
                </div>
            </div>
            <div class="slideshow-item">
                <img src="/api/placeholder/1200/400" alt="Laboratori i Kimisë">
                <div class="slideshow-caption">
                    <h3>Laboratorët e shkencave</h3>
                    <p>Pajisje moderne për eksperimente praktike</p>
                </div>
            </div>
            <div class="slideshow-item">
                <img src="/api/placeholder/1200/400" alt="Aktivitetet sportive">
                <div class="slideshow-caption">
                    <h3>Aktivitetet sportive</h3>
                    <p>Mundësi të shumta për zhvillimin fizik të nxënësve</p>
                </div>
            </div>
            <div class="slideshow-nav">
                <button class="prev">&#10094;</button>
                <button class="next">&#10095;</button>
            </div>
        </div>
    </div>

    <section id="contact" class="contact">
        <div class="container">
            <div class="contact-content">
                <div class="contact-info">
                    <h2>Na Kontaktoni</h2>
                    <p>Për çdo pyetje apo informacion shtesë, ju lutemi të na kontaktoni.</p>
                    <p><b>Adresa:</b> 18 Shtatori, Gjirokaster</p>
                    <p><b>Tel:</b> +355</p>
                    <p><b>Email:</b> info@gjimnazisirishapllo.edu.al</p>
                </div>
                <div class="contact-form">
                    <h2>Na Dërgoni një Mesazh</h2>
                    <form>
                        <label for="name">Emri:</label>
                        <input type="text" id="name" name="name" required>

                        <label for="email">Email:</label>
                        <input type="email" id="email" name="email" required>

                        <label for="message">Mesazhi:</label>
                        <textarea id="message" name="message" rows="5" required></textarea>

                        <button type="submit">Dërgo Mesazhin</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <script src="https://kit.fontawesome.com/your-fontawesome-kit.js" crossorigin="anonymous"></script>
    <script>
        // Header scroll effect
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            header.classList.toggle('scrolled', window.scrollY > 50);
        });

        // Mobile menu toggle
        const menuToggle = document.querySelector('.menu-toggle');
        const nav = document.querySelector('nav ul');

        menuToggle.addEventListener('click', () => {
            nav.classList.toggle('active');
            menuToggle.classList.toggle('active');
        });

        // Slideshow functionality
        const slideshowItems = document.querySelectorAll('.slideshow-item');
        const prevButton = document.querySelector('.prev');
        const nextButton = document.querySelector('.next');
        let currentSlide = 0;

        function showSlide(index) {
            slideshowItems.forEach(item => item.classList.remove('active'));
            slideshowItems[index].classList.add('active');
        }

        function nextSlide() {
            currentSlide = (currentSlide + 1) % slideshowItems.length;
            showSlide(currentSlide);
        }

        function prevSlide() {
            currentSlide = (currentSlide - 1 + slideshowItems.length) % slideshowItems.length;
            showSlide(currentSlide);
        }

        nextButton.addEventListener('click', nextSlide);
        prevButton.addEventListener('click', prevSlide);

        setInterval(nextSlide, 5000); // Auto slide every 5 seconds
    </script>
</body>

</html>
