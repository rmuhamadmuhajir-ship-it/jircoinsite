```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jir Coin (JCN) - The Future of Fun Finance</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700;900&family=Rajdhani:wght@300;400;500;600;700&display=swap');
        
        :root {
            --primary-color: #8a2be2;
            --secondary-color: #00bfff;
            --accent-color: #ffd700;
            --dark-bg: #0a0a0a;
            --card-bg: rgba(20, 20, 40, 0.7);
            --text-light: #ffffff;
            --text-muted: #b8b8d1;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Rajdhani', sans-serif;
            background-color: var(--dark-bg);
            color: var(--text-light);
            overflow-x: hidden;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(10, 10, 10, 0.8);
            backdrop-filter: blur(10px);
            padding: 15px 0;
            transition: all 0.3s ease;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
            font-family: 'Orbitron', sans-serif;
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--accent-color);
            text-decoration: none;
        }
        
        .logo img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        .nav-links {
            display: flex;
            gap: 30px;
            list-style: none;
        }
        
        .nav-links a {
            color: var(--text-light);
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            position: relative;
        }
        
        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--secondary-color);
            transition: width 0.3s ease;
        }
        
        .nav-links a:hover::after {
            width: 100%;
        }
        
        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            background: linear-gradient(135deg, rgba(10, 10, 10, 0.9), rgba(30, 10, 60, 0.9)), 
                        url('https://z-cdn-media.chatglm.cn/files/385dfa27-2f11-4088-8ff7-3cc604a1b9a3_Gemini_Generated_Image_qzksjsqzksjsqzks%20%281%29.png?auth_key=1793098919-af01ad4c5d28410194758534ecc3f51f-0-ad55e01f10fc1ecbada60d6fc2bc87d2');
            background-size: cover;
            background-position: center;
            overflow: hidden;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 50% 50%, rgba(138, 43, 226, 0.2) 0%, transparent 70%);
            z-index: -1;
        }
        
        .particles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: -1;
        }
        
        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: var(--secondary-color);
            border-radius: 50%;
            opacity: 0.7;
            animation: particle-float 15s infinite linear;
        }
        
        @keyframes particle-float {
            0% {
                transform: translateY(100vh) translateX(0);
                opacity: 0;
            }
            10% {
                opacity: 0.7;
            }
            90% {
                opacity: 0.7;
            }
            100% {
                transform: translateY(-100vh) translateX(100px);
                opacity: 0;
            }
        }
        
        .hero-content {
            text-align: center;
            z-index: 2;
            padding: 20px;
        }
        
        .hero-logo {
            width: 150px;
            height: 150px;
            margin: 0 auto 30px;
            border-radius: 50%;
            box-shadow: 0 0 30px rgba(138, 43, 226, 0.7);
            animation: glow 2s ease-in-out infinite alternate;
        }
        
        @keyframes glow {
            from { box-shadow: 0 0 20px rgba(138, 43, 226, 0.7); }
            to { box-shadow: 0 0 30px rgba(138, 43, 226, 0.9), 0 0 40px rgba(0, 191, 255, 0.5); }
        }
        
        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: 3.5rem;
            font-weight: 900;
            margin-bottom: 20px;
            background: linear-gradient(90deg, var(--accent-color), var(--secondary-color));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-shadow: 0 0 20px rgba(138, 43, 226, 0.5);
        }
        
        .hero p {
            font-size: 1.5rem;
            margin-bottom: 40px;
            color: var(--text-muted);
        }
        
        .btn-group {
            display: flex;
            gap: 20px;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        .btn {
            padding: 15px 30px;
            font-family: 'Orbitron', sans-serif;
            font-weight: 600;
            font-size: 1rem;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            position: relative;
            overflow: hidden;
        }
        
        .btn-primary {
            background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
            color: white;
        }
        
        .btn-secondary {
            background: transparent;
            color: var(--text-light);
            border: 2px solid var(--secondary-color);
        }
        
        .btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(138, 43, 226, 0.4);
        }
        
        .btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s;
        }
        
        .btn:hover::before {
            left: 100%;
        }
        
        /* Section Styles */
        section {
            padding: 100px 0;
            position: relative;
        }
        
        .section-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 2.5rem;
            font-weight: 700;
            text-align: center;
            margin-bottom: 50px;
            position: relative;
            color: var(--accent-color);
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
        }
        
        /* About Section */
        .about {
            background: linear-gradient(135deg, rgba(20, 20, 40, 0.9), rgba(40, 20, 80, 0.9));
        }
        
        .about-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
            font-size: 1.2rem;
            line-height: 1.8;
            color: var(--text-muted);
        }
        
        /* Tokenomics Section */
        .tokenomics {
            background: var(--dark-bg);
        }
        
        .tokenomics-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .token-card {
            background: var(--card-bg);
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            border: 1px solid rgba(138, 43, 226, 0.3);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .token-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(138, 43, 226, 0.1) 0%, transparent 70%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .token-card:hover::before {
            opacity: 1;
        }
        
        .token-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(138, 43, 226, 0.3);
            border-color: var(--secondary-color);
        }
        
        .token-card i {
            font-size: 2.5rem;
            color: var(--secondary-color);
            margin-bottom: 20px;
        }
        
        .token-card h3 {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: var(--accent-color);
        }
        
        .token-card p {
            font-size: 1.1rem;
            color: var(--text-muted);
        }
        
        .contract-address {
            background: rgba(0, 191, 255, 0.1);
            border: 1px solid rgba(0, 191, 255, 0.3);
            border-radius: 10px;
            padding: 15px;
            margin-top: 20px;
            font-family: 'Orbitron', sans-serif;
            font-size: 0.9rem;
            word-break: break-all;
            position: relative;
        }
        
        .copy-btn {
            position: absolute;
            right: 10px;
            top: 50%;
            transform: translateY(-50%);
            background: var(--secondary-color);
            color: var(--dark-bg);
            border: none;
            border-radius: 5px;
            padding: 5px 10px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        
        .copy-btn:hover {
            background: var(--accent-color);
        }
        
        /* Roadmap Section */
        .roadmap {
            background: linear-gradient(135deg, rgba(20, 20, 40, 0.9), rgba(40, 20, 80, 0.9));
        }
        
        .roadmap-timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .roadmap-timeline::before {
            content: '';
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 2px;
            height: 100%;
            background: linear-gradient(to bottom, var(--primary-color), var(--secondary-color));
        }
        
        .roadmap-item {
            position: relative;
            margin-bottom: 50px;
            width: 100%;
        }
        
        .roadmap-item:nth-child(odd) .roadmap-content {
            margin-right: 50%;
            text-align: right;
            padding-right: 40px;
        }
        
        .roadmap-item:nth-child(even) .roadmap-content {
            margin-left: 50%;
            padding-left: 40px;
        }
        
        .roadmap-dot {
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background: var(--accent-color);
            border: 3px solid var(--dark-bg);
            z-index: 1;
        }
        
        .roadmap-content {
            background: var(--card-bg);
            border-radius: 10px;
            padding: 20px;
            border: 1px solid rgba(138, 43, 226, 0.3);
            transition: all 0.3s ease;
        }
        
        .roadmap-content:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(138, 43, 226, 0.3);
            border-color: var(--secondary-color);
        }
        
        .roadmap-content h3 {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.5rem;
            margin-bottom: 10px;
            color: var(--accent-color);
        }
        
        .roadmap-content p {
            color: var(--text-muted);
        }
        
        /* Community Section */
        .community {
            background: var(--dark-bg);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 50px;
        }
        
        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 80px;
            height: 80px;
            border-radius: 50%;
            background: var(--card-bg);
            border: 2px solid rgba(138, 43, 226, 0.3);
            color: var(--text-light);
            font-size: 2rem;
            transition: all 0.3s ease;
            text-decoration: none;
        }
        
        .social-link:hover {
            transform: translateY(-10px);
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            box-shadow: 0 15px 30px rgba(138, 43, 226, 0.4);
        }
        
        /* Chart Section */
        .chart-section {
            background: linear-gradient(135deg, rgba(20, 20, 40, 0.9), rgba(40, 20, 80, 0.9));
            padding: 50px 0;
        }
        
        .chart-container {
            max-width: 900px;
            margin: 0 auto;
            background: var(--card-bg);
            border-radius: 15px;
            padding: 20px;
            border: 1px solid rgba(138, 43, 226, 0.3);
            height: 500px;
            overflow: hidden;
        }
        
        .chart-container iframe {
            width: 100%;
            height: 100%;
            border: none;
            border-radius: 10px;
        }
        
        /* Footer */
        footer {
            background: rgba(10, 10, 10, 0.9);
            padding: 30px 0;
            text-align: center;
            border-top: 1px solid rgba(138, 43, 226, 0.3);
        }
        
        .footer-content p {
            margin-bottom: 10px;
            color: var(--text-muted);
        }
        
        .disclaimer {
            font-size
