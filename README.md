<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EarlyBird - Join Waitlist</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        }

        body {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #f5f7fa 0%, #e4e9f2 100%);
        }

        .container {
            width: 100%;
            max-width: 480px;
            padding: 2rem;
            text-align: center;
            background: white;
            border-radius: 16px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            margin: 1rem;
        }

        .logo {
            width: 48px;
            height: 48px;
            margin-bottom: 1.5rem;
        }

        .sparkle-icon {
            width: 48px;
            height: 48px;
            margin: 1rem 0;
            color: #3b82f6;
        }

        h1 {
            font-size: 2rem;
            color: #1f2937;
            margin-bottom: 0.5rem;
        }

        .product-name {
            color: #10b981;
            font-weight: 600;
        }

        .subtitle {
            color: #6b7280;
            margin-bottom: 2rem;
        }

        input {
            width: 100%;
            padding: 0.75rem 1rem;
            margin-bottom: 1rem;
            border: 1px solid #e5e7eb;
            border-radius: 8px;
            font-size: 1rem;
            outline: none;
            transition: border-color 0.2s;
        }

        input:focus {
            border-color: #10b981;
        }

        button {
            width: 100%;
            padding: 0.75rem;
            background-color: #111827;
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 500;
            cursor: pointer;
            transition: background-color 0.2s;
        }

        button:hover {
            background-color: #374151;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
        }

        .social-links a {
            color: #6b7280;
            text-decoration: none;
            transition: color 0.2s;
        }

        .social-links a:hover {
            color: #374151;
        }

        .nav-buttons {
            position: absolute;
            top: 1rem;
            right: 1rem;
            display: flex;
            gap: 0.5rem;
        }

        .nav-button {
            background: none;
            border: none;
            padding: 0.5rem;
            cursor: pointer;
            color: #6b7280;
        }

        .nav-button:hover {
            color: #374151;
            background: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="nav-buttons">
            <button class="nav-button">←</button>
            <button class="nav-button">→</button>
            <button class="nav-button">⋮</button>
            <button class="nav-button">✕</button>
        </div>
        
        <img src="/api/placeholder/48/48" alt="Logo" class="logo">
        
        <svg class="sparkle-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <path d="M12 2L15 9L22 9L16 14L18 21L12 17L6 21L8 14L2 9L9 9L12 2Z" />
        </svg>

        <h1>Join the waitlist for<br><span class="product-name">DataMind</span></h1>
        <p class="subtitle">Stay informed about our latest updates</p>

        <form id="waitlistForm">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <button type="submit">Join the waitlist</button>
        </form>

        <div class="social-links">
            <a href="#" aria-label="Twitter">𝕏</a>
            <a href="#" aria-label="Facebook">f</a>
            <a href="#" aria-label="Instagram">📷</a>
            <a href="#" aria-label="LinkedIn">in</a>
            <a href="#" aria-label="YouTube">▶</a>
        </div>
    </div>

    <script>
        document.getElementById('waitlistForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for joining the waitlist!');
        });
    </script>
</body>
