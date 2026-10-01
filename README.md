<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vandal_Heartz</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;1,400;1,500&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg: #0b0a0d;
            --bg-alt: #16131a;
            --text: #e8e3e6;
            --muted: #948b93;
            --accent: #8c2f45;
            --accent-soft: #b3475f;
            --line: #2a242c;
        }

        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            background-color: var(--bg);
            background-image:
                linear-gradient(rgba(11, 10, 13, 0.88), rgba(11, 10, 13, 0.93)),
                url("hero.png");
            background-size: cover;
            background-position: center top;
            background-attachment: fixed;
            background-repeat: no-repeat;
            color: var(--text);
            font-family: "Inter", sans-serif;
            font-weight: 300;
            line-height: 1.7;
        }

        .hero {
            position: relative;
            min-height: 60vh;
            display: flex;
            align-items: flex-end;
        }

        .hero-overlay {
            position: relative;
            max-width: 640px;
            margin: 0 auto;
            padding: 24px 24px 64px;
            width: 100%;
        }

        .hero h1 {
            font-family: "Cormorant Garamond", serif;
            font-style: italic;
            font-weight: 500;
            font-size: 3.4rem;
            margin: 0;
            color: var(--text);
            text-shadow: 0 2px 20px rgba(0, 0, 0, 0.5);
        }

        .tagline {
            color: var(--muted);
            margin: 8px 0 32px;
            font-size: 1rem;
        }

        nav {
            display: flex;
            gap: 28px;
            border-top: 1px solid var(--line);
            padding-top: 20px;
        }

        nav a {
            color: var(--muted);
            text-decoration: none;
            font-size: 0.95rem;
            letter-spacing: 0.02em;
            transition: color 0.2s ease;
        }

        nav a:hover,
        nav a:focus-visible {
            color: var(--accent-soft);
        }

        main {
            max-width: 640px;
            margin: 0 auto;
            padding: 0 24px;
        }

        section {
            padding: 32px;
            margin: 32px 0;
            border: 1px solid var(--line);
            border-radius: 10px;
            background-color: rgba(17, 14, 20, 0.6);
            backdrop-filter: blur(4px);
        }

        section h2 {
            font-family: "Cormorant Garamond", serif;
            font-style: italic;
            font-weight: 500;
            font-size: 1.8rem;
            color: var(--accent-soft);
            margin: 0 0 20px;
        }

        section p {
            color: var(--text);
            max-width: 56ch;
        }

        .contact-line {
            color: var(--muted);
            font-size: 0.95rem;
            margin-top: 24px;
        }

        .contact-line a {
            color: var(--accent-soft);
            text-decoration: none;
            border-bottom: 1px solid var(--accent);
        }

        .contact-line a:hover,
        .contact-line a:focus-visible {
            color: var(--text);
        }

        .social-list {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            flex-direction: column;
            gap: 14px;
        }

        .social-list li {
            color: var(--muted);
        }

        .social-list a {
            color: var(--accent-soft);
            text-decoration: none;
            border-bottom: 1px solid var(--accent);
        }

        .social-list a:hover,
        .social-list a:focus-visible {
            color: var(--text);
        }

        .facts-list {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            flex-direction: column;
            gap: 14px;
        }

        .facts-list li {
            position: relative;
            padding-left: 22px;
        }

        .facts-list li::before {
            content: "—";
            position: absolute;
            left: 0;
            color: var(--accent);
        }

        footer {
            max-width: 640px;
            margin: 0 auto;
            padding: 40px 24px 80px;
            border-top: 1px solid var(--line);
            color: var(--muted);
            font-size: 0.85rem;
        }

        @media (max-width: 480px) {
            .hero {
                min-height: 50vh;
            }

            .hero-overlay {
                padding: 20px 20px 44px;
            }

            .hero h1 {
                font-size: 2.3rem;
            }

            body {
                background-attachment: scroll;
            }
        }
    </style>
</head>
<body>
    <header class="hero">
        <div class="hero-overlay">
            <h1>Vandal_Heartz</h1>
            <p class="tagline">a quiet corner of the internet</p>
            <nav>
                <a href="#about">about</a>
                <a href="#facts">fun facts</a>
                <a href="#find-me">find me</a>
            </nav>
        </div>
    </header>

    <main>
        <section id="about">
            <h2>About Me</h2>
            <p>
                I'm Vandal_Heartz — a 9th grade student, into mechanical engineering.
                Outside of school I make music and post it on Suno.
                My song <em>"Better Off Without You"</em> is the one that matters most to
                me — I wrote it about myself.
            </p>
            <p>
                This site's just for fun. If I'm being honest, I want to get out of my
                country someday. People here love to talk about its heritage and
                "unity in diversity" — but look past the talk and it's a different story.
            </p>
        </section>

        <section id="facts">
            <h2>Fun Facts</h2>
            <ul class="facts-list">
                <li>Best goalkeeper in my school — still managed to end up friendless.</li>
                <li>I notice tiny details other people miss.</li>
                <li>Oddly drawn to people who try to annoy and irritate me.</li>
                <li>Making music, listening to it non-stop, and researching how to get out of my country.</li>
                <li>Favorite song: "Oxygen" by Johnny Huynh.</li>
                <li>Favorite movie: honestly, I don't watch many.</li>
                <li>Favorite book: <em>Haunting Adeline</em> (don't ask).</li>
                <li>What I actually want: some peace, and real friends who don't just try to get under my skin.</li>
            </ul>
        </section>

        <section id="find-me">
            <h2>Find Me</h2>
            <ul class="social-list">
                <li>Suno: Vandal_heartz</li>
                <li>
                    Instagram:
                    <a href="https://instagram.com/ghostvoidnyk" target="_blank" rel="noopener">
                        @ghostvoidnyk
                    </a>
                </li>
                <li>Discord: ghostvoidnyk</li>
            </ul>
        </section>
    </main>

    <footer>
        <p>&copy; <span id="year"></span> Vandal_Heartz</p>
    </footer>

    <script>
        document.getElementById("year").textContent = new Date().getFullYear();
    </script>
</body>
</html>
