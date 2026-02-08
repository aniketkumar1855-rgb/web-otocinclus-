<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Otocinclus - HR Consultancy & HRMS Implementation Partner | Build, Operate, Transfer</title>
    <meta name="description" content="Otocinclus delivers integrated HR infrastructure for India's growing businesses. Expert HR consultancy, HRMS implementation, payroll compliance & flat 7% recruitment services. We audit, advise, implement, and transfer.">
    <meta name="keywords" content="HR consultancy, HRMS implementation, payroll services, recruitment agency, HR outsourcing, compliance management, Build-Operate-Transfer, SME HR solutions">
    <style>
        :root {
            --primary-blue: #4A90E2;
            --secondary-blue: #5BA3F5;
            --accent-orange: #E89F5F;
            --dark-navy: #1F2533;
            --light-bg: #FCFCF9;
            --text-dark: #1F2533;
            --text-light: #626C71;
            --white: #FFFFFF;
            --gradient-primary: linear-gradient(135deg, #4A90E2 0%, #5BA3F5 100%);
            --gradient-secondary: linear-gradient(135deg, #E89F5F 0%, #F5B87F 100%);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Helvetica Neue', Arial, sans-serif;
            color: var(--text-dark);
            line-height: 1.6;
            overflow-x: hidden;
            background-color: var(--light-bg);
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
            z-index: 1000;
            transition: all 0.3s ease;
        }

        nav.scrolled {
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.15);
        }

        .nav-container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo-container {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .logo {
            width: 50px;
            height: 50px;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        .logo-text {
            display: flex;
            flex-direction: column;
        }

        .logo-text h1 {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--dark-navy);
            letter-spacing: -0.5px;
        }

        .logo-text p {
            font-size: 0.875rem;
            color: var(--primary-blue);
            font-weight: 500;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
            align-items: center;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 500;
            font-size: 1rem;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--gradient-primary);
            transition: width 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--primary-blue);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .cta-button {
            background: var(--gradient-primary);
            color: var(--white);
            padding: 0.75rem 1.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1rem;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 15px rgba(74, 144, 226, 0.3);
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 25px rgba(74, 144, 226, 0.4);
        }

        .mobile-menu {
            display: none;
            flex-direction: column;
            gap: 5px;
            cursor: pointer;
        }

        .mobile-menu span {
            width: 25px;
            height: 3px;
            background: var(--text-dark);
            border-radius: 2px;
            transition: all 0.3s ease;
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, rgba(74, 144, 226, 0.05) 0%, rgba(232, 159, 95, 0.05) 100%);
            padding: 6rem 2rem 4rem;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -20%;
            width: 800px;
            height: 800px;
            background: radial-gradient(circle, rgba(74, 144, 226, 0.1) 0%, transparent 70%);
            border-radius: 50%;
            animation: pulse 8s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 0.5; }
            50% { transform: scale(1.1); opacity: 0.8; }
        }

        .hero-content {
            max-width: 1400px;
            display: grid;
            grid-template-columns: 1.15fr 1fr;
            gap: 4rem;
            align-items: center;
            position: relative;
            z-index: 1;
        }

        .hero-text h2 {
            font-size: 3.5rem;
            font-weight: 800;
            line-height: 1.1;
            margin-bottom: 1.5rem;
            color: var(--dark-navy);
            letter-spacing: -1px;
        }

        .hero-text .highlight {
            background: var(--gradient-primary);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-text .tagline {
            font-size: 1.5rem;
            color: var(--text-light);
            margin-bottom: 2rem;
            font-weight: 500;
        }

        .hero-text p {
            font-size: 1.125rem;
            color: var(--text-light);
            margin-bottom: 2.5rem;
            line-height: 1.8;
        }

        .hero-buttons {
            display: flex;
            gap: 1.5rem;
            flex-wrap: wrap;
        }

        .btn-primary {
            background: var(--gradient-primary);
            color: var(--white);
            padding: 1rem 2.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.125rem;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 6px 20px rgba(74, 144, 226, 0.3);
            border: none;
            cursor: pointer;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 30px rgba(74, 144, 226, 0.4);
        }

        .btn-secondary {
            background: var(--white);
            color: var(--primary-blue);
            padding: 1rem 2.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.125rem;
            border: 2px solid var(--primary-blue);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .btn-secondary:hover {
            background: var(--primary-blue);
            color: var(--white);
            transform: translateY(-3px);
        }

        .hero-visual {
            position: relative;
        }

        /* Hero Slider */
        .hero-slider {
            background: var(--white);
            border-radius: 24px;
            box-shadow: 0 14px 45px rgba(0, 0, 0, 0.12);
            padding: 2.25rem 2.5rem 2.75rem;
            position: relative;
            overflow: hidden;
        }

        .hero-slider::before {
            content: '';
            position: absolute;
            inset: 0;
            background: radial-gradient(circle at top right, rgba(74,144,226,0.12), transparent 55%),
                        radial-gradient(circle at bottom left, rgba(232,159,95,0.1), transparent 55%);
            pointer-events: none;
        }

        .slider-slide {
            display: none;
            position: relative;
            z-index: 1;
            grid-template-columns: auto 1fr;
            gap: 1.75rem;
            align-items: center;
        }

        .slider-slide.active {
            display: grid;
            animation: fadeInSlide 0.6s ease forwards;
        }

        @keyframes fadeInSlide {
            from { opacity: 0; transform: translateY(14px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .slide-logo-orbit {
            width: 92px;
            height: 92px;
            border-radius: 50%;
            background: radial-gradient(circle, rgba(74,144,226,0.15), transparent 65%);
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }

        .slide-logo-orbit::after {
            content: '';
            position: absolute;
            width: 120%;
            height: 120%;
            border-radius: 50%;
            border: 1px dashed rgba(74,144,226,0.4);
            animation: orbit 12s linear infinite;
        }

        @keyframes orbit {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .slide-logo-orbit img {
            width: 64px;
            height: 64px;
            object-fit: contain;
        }

        .slide-content-tag {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.35rem 0.85rem;
            border-radius: 999px;
            background: rgba(74,144,226,0.08);
            color: var(--primary-blue);
            font-size: 0.8rem;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 0.06em;
            margin-bottom: 0.5rem;
        }

        .slide-heading {
            font-size: 1.6rem;
            font-weight: 750;
            color: var(--dark-navy);
            margin-bottom: 0.45rem;
        }

        .slide-subtitle {
            font-size: 0.98rem;
            color: var(--text-light);
            margin-bottom: 0.85rem;
        }

        .slide-points {
            list-style: none;
            margin-top: 0.25rem;
        }

        .slide-points li {
            font-size: 0.9rem;
            color: var(--text-light);
            padding: 0.35rem 0;
            display: flex;
            align-items: flex-start;
            gap: 0.45rem;
        }

        .slide-points li::before {
            content: '●';
            font-size: 0.55rem;
            margin-top: 0.4rem;
            color: var(--primary-blue);
        }

        /* Mini pricing graphic for 7% slide */
        .price-graphic {
            margin-top: 0.6rem;
            display: grid;
            gap: 0.45rem;
        }

        .price-bar-row {
            display: flex;
            align-items: center;
            gap: 0.55rem;
            font-size: 0.8rem;
            color: var(--text-light);
        }

        .price-label {
            min-width: 70px;
        }

        .price-bar-track {
            flex: 1;
            height: 7px;
            background: rgba(255,255,255,0.9);
            border-radius: 999px;
            overflow: hidden;
        }

        .price-bar-fill {
            height: 100%;
            border-radius: 999px;
            background: var(--gradient-secondary);
            transform-origin: left;
            animation: growBar 1.2s ease-out forwards;
        }

        .price-bar-fill.senior {
            background: linear-gradient(90deg, #E89F5F, #F36F45);
        }

        @keyframes growBar {
            from { transform: scaleX(0); }
            to { transform: scaleX(1); }
        }

        .price-note {
            font-size: 0.75rem;
            color: var(--text-light);
            margin-top: 0.35rem;
        }

        .hero-slider-controls {
            position: relative;
            z-index: 1;
            margin-top: 1.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .slider-dots {
            display: flex;
            gap: 0.45rem;
            align-items: center;
        }

        .slider-dot {
            width: 9px;
            height: 9px;
            border-radius: 50%;
            border: 1px solid rgba(74,144,226,0.5);
            background: transparent;
            cursor: pointer;
            transition: all 0.25s ease;
        }

        .slider-dot.active {
            background: var(--primary-blue);
            transform: scale(1.1);
            border-color: transparent;
        }

        .slider-caption {
            font-size: 0.78rem;
            color: var(--text-light);
        }

        /* (Old floating-card styles remain in case needed elsewhere) */
        .floating-card {
            background: var(--white);
            border-radius: 20px;
            padding: 2rem;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
            margin-bottom: 2rem;
            transition: transform 0.5s ease;
            transform-style: preserve-3d;
        }

        .floating-card:hover {
            transform: translateZ(20px) rotateY(5deg);
        }

        .floating-card h3 {
            font-size: 1.25rem;
            color: var(--primary-blue);
            margin-bottom: 0.5rem;
        }

        .floating-card p {
            font-size: 1rem;
            color: var(--text-light);
        }

        /* Stats Section */
        .stats {
            background: var(--gradient-primary);
            padding: 4rem 2rem;
            color: var(--white);
        }

        .stats-container {
            max-width: 1400px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            text-align: center;
        }

        .stat-item h3 {
            font-size: 3.5rem;
            font-weight: 800;
            margin-bottom: 0.5rem;
        }

        .stat-item p {
            font-size: 1.125rem;
            opacity: 0.95;
            font-weight: 500;
        }

        /* Admin Trap Section */
        .admin-trap {
            padding: 6rem 2rem;
            background: var(--white);
        }

        .admin-trap-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-title h2 {
            font-size: 2.5rem;
            font-weight: 800;
            color: var(--dark-navy);
            margin-bottom: 1rem;
        }

        .section-title p {
            font-size: 1.25rem;
            color: var(--text-light);
            max-width: 800px;
            margin: 0 auto;
        }

        .admin-trap-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
            margin-top: 4rem;
        }

        .trap-visual {
            background: linear-gradient(135deg, rgba(74, 144, 226, 0.1) 0%, rgba(232, 159, 95, 0.1) 100%);
            border-radius: 20px;
            padding: 3rem;
            position: relative;
        }

        .trap-visual .chart {
            width: 100%;
            height: 300px;
            position: relative;
        }

        .trap-points {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }

        .trap-point {
            background: var(--light-bg);
            border-left: 4px solid var(--primary-blue);
            padding: 1.5rem;
            border-radius: 10px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .trap-point:hover {
            transform: translateX(10px);
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }

        .trap-point h4 {
            font-size: 1.25rem;
            color: var(--primary-blue);
            margin-bottom: 0.5rem;
        }

        .trap-point p {
            color: var(--text-light);
            font-size: 1rem;
        }

        /* Services Section */
        .services {
            padding: 6rem 2rem;
            background: var(--light-bg);
        }

        .services-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
            margin-top: 4rem;
        }

        .service-card {
            background: var(--white);
            border-radius: 20px;
            padding: 2.5rem;
            box-shadow: 0 5px 30px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: var(--gradient-primary);
            transform: scaleX(0);
            transition: transform 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 50px rgba(0, 0, 0, 0.15);
        }

        .service-card:hover::before {
            transform: scaleX(1);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 1.5rem;
        }

        .service-card h3 {
            font-size: 1.5rem;
            color: var(--dark-navy);
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .service-card p {
            color: var(--text-light);
            font-size: 1rem;
            margin-bottom: 1.5rem;
            line-height: 1.7;
        }

        .service-card ul {
            list-style: none;
            margin-top: 1rem;
        }

        .service-card ul li {
            padding: 0.5rem 0;
            color: var(--text-light);
            font-size: 0.9375rem;
            position: relative;
            padding-left: 1.5rem;
        }

        .service-card ul li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--primary-blue);
            font-weight: bold;
        }

        .learn-more {
            color: var(--primary-blue);
            font-weight: 600;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            transition: gap 0.3s ease;
        }

        .learn-more:hover {
            gap: 1rem;
        }

        /* Models Section */
        .models {
            padding: 6rem 2rem;
            background: var(--white);
        }

        .models-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .models-tabs {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 3rem;
            margin-bottom: 3rem;
            flex-wrap: wrap;
        }

        .tab-button {
            background: var(--light-bg);
            color: var(--text-dark);
            padding: 1rem 2.5rem;
            border-radius: 50px;
            border: 2px solid transparent;
            font-weight: 600;
            font-size: 1.125rem;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .tab-button.active {
            background: var(--gradient-primary);
            color: var(--white);
            box-shadow: 0 6px 20px rgba(74, 144, 226, 0.3);
        }

        .tab-content {
            display: none;
        }

        .tab-content.active {
            display: block;
            animation: fadeIn 0.5s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .model-content {
            background: linear-gradient(135deg, rgba(74, 144, 226, 0.05) 0%, rgba(232, 159, 95, 0.05) 100%);
            border-radius: 20px;
            padding: 3rem;
        }

        .model-flow {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 3rem 0;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .flow-step {
            background: var(--white);
            border-radius: 15px;
            padding: 1.5rem;
            text-align: center;
            flex: 1;
            min-width: 150px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
            position: relative;
        }

        .flow-step::after {
            content: '→';
            position: absolute;
            right: -1.5rem;
            top: 50%;
            transform: translateY(-50%);
            font-size: 2rem;
            color: var(--primary-blue);
        }

        .flow-step:last-child::after {
            display: none;
        }

        .flow-step h4 {
            font-size: 1.125rem;
            color: var(--primary-blue);
            margin-bottom: 0.5rem;
        }

        .flow-step p {
            font-size: 0.9375rem;
            color: var(--text-light);
        }

        .model-features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .feature-box {
            background: var(--white);
            border-radius: 15px;
            padding: 2rem;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
        }

        .feature-box h4 {
            font-size: 1.25rem;
            color: var(--dark-navy);
            margin-bottom: 1rem;
        }

        .feature-box ul {
            list-style: none;
        }

        .feature-box ul li {
            padding: 0.5rem 0;
            color: var(--text-light);
            position: relative;
            padding-left: 1.5rem;
        }

        .feature-box ul li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--primary-blue);
            font-size: 1.5rem;
            line-height: 1;
        }

        /* Recruitment Section */
        .recruitment {
            padding: 6rem 2rem;
            background: var(--gradient-primary);
            color: var(--white);
        }

        .recruitment-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .recruitment-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
            margin-top: 3rem;
        }

        .pricing-comparison {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 3rem;
        }

        .pricing-comparison h3 {
            font-size: 2rem;
            margin-bottom: 2rem;
        }

        .comparison-item {
            display: flex;
            justify-content: space-between;
            padding: 1rem 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }

        .comparison-item:last-child {
            border-bottom: none;
        }

        .comparison-item span:first-child {
            font-weight: 500;
        }

        .comparison-item span:last-child {
            font-weight: 700;
            font-size: 1.25rem;
        }

        .recruitment-benefits {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }

        .benefit-item {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 2rem;
        }

        .benefit-item h4 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .benefit-item p {
            font-size: 1rem;
            line-height: 1.7;
            opacity: 0.95;
        }

        /* Case Studies */
        .case-studies {
            padding: 6rem 2rem;
            background: var(--light-bg);
        }

        .case-studies-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .case-study-card {
            background: var(--white);
            border-radius: 20px;
            padding: 3rem;
            margin-top: 3rem;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
        }

        .case-study-header {
            display: flex;
            justify-content: space-between;
            align-items: start;
            margin-bottom: 2rem;
            flex-wrap: wrap;
            gap: 2rem;
        }

        .case-study-info h3 {
            font-size: 1.75rem;
            color: var(--dark-navy);
            margin-bottom: 0.5rem;
        }

        .case-study-info p {
            color: var(--text-light);
            font-size: 1rem;
        }

        .case-study-metrics {
            display: flex;
            gap: 2rem;
        }

        .metric {
            text-align: center;
        }

        .metric h4 {
            font-size: 2rem;
            color: var(--primary-blue);
            font-weight: 800;
        }

        .metric p {
            font-size: 0.875rem;
            color: var(--text-light);
        }

        .case-study-body {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            margin-top: 2rem;
        }

        .challenge, .solution {
            padding: 1.5rem;
            background: var(--light-bg);
            border-radius: 15px;
        }

        .challenge h4, .solution h4 {
            color: var(--primary-blue);
            margin-bottom: 1rem;
            font-size: 1.25rem;
        }

        .challenge p, .solution p {
            color: var(--text-light);
            line-height: 1.7;
        }

        /* Contact Section */
        .contact {
            padding: 6rem 2rem;
            background: var(--white);
        }

        .contact-container {
            max-width: 1400px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
        }

        .contact-info h3 {
            font-size: 2rem;
            color: var(--dark-navy);
            margin-bottom: 1rem;
        }

        .contact-info p {
            color: var(--text-light);
            font-size: 1.125rem;
            margin-bottom: 2rem;
            line-height: 1.7;
        }

        .contact-details {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .contact-icon {
            width: 50px;
            height: 50px;
            background: var(--gradient-primary);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--white);
            font-size: 1.25rem;
        }

        .contact-item-text h4 {
            font-size: 1rem;
            color: var(--dark-navy);
            margin-bottom: 0.25rem;
        }

        .contact-item-text p {
            font-size: 1rem;
            color: var(--text-light);
            margin: 0;
        }

        .contact-form {
            background: var(--light-bg);
            padding: 3rem;
            border-radius: 20px;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: var(--dark-navy);
            font-size: 1rem;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 1rem;
            border: 2px solid #E2E8F0;
            border-radius: 10px;
            font-size: 1rem;
            font-family: inherit;
            transition: border-color 0.3s ease;
            background: var(--white);
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--primary-blue);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }

        .submit-btn {
            background: var(--gradient-primary);
            color: var(--white);
            padding: 1rem 3rem;
            border-radius: 50px;
            border: none;
            font-weight: 600;
            font-size: 1.125rem;
            cursor: pointer;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 6px 20px rgba(74, 144, 226, 0.3);
            width: 100%;
        }

        .submit-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 30px rgba(74, 144, 226, 0.4);
        }

        /* Footer */
        footer {
            background: var(--dark-navy);
            color: var(--white);
            padding: 4rem 2rem 2rem;
        }

        .footer-container {
            max-width: 1400px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            margin-bottom: 3rem;
        }

        .footer-section h4 {
            font-size: 1.25rem;
            margin-bottom: 1.5rem;
        }

        .footer-section p {
            opacity: 0.8;
            line-height: 1.7;
            font-size: 0.9375rem;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 0.75rem;
        }

        .footer-links a {
            color: var(--white);
            text-decoration: none;
            opacity: 0.8;
            transition: opacity 0.3s ease;
            font-size: 0.9375rem;
        }

        .footer-links a:hover {
            opacity: 1;
        }

        .footer-bottom {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: 2rem;
            text-align: center;
            opacity: 0.7;
            font-size: 0.875rem;
        }

        /* Responsive Design */
        @media (max-width: 968px) {
            .nav-links {
                display: none;
            }

            .mobile-menu {
                display: flex;
            }

            .hero-content,
            .admin-trap-content,
            .recruitment-content,
            .contact-container,
            .case-study-body {
                grid-template-columns: 1fr;
            }

            .hero-text h2 {
                font-size: 2.5rem;
            }

            .hero-text .tagline {
                font-size: 1.25rem;
            }

            .section-title h2 {
                font-size: 2rem;
            }

            .flow-step::after {
                display: none;
            }

            .model-flow {
                flex-direction: column;
            }

            .slider-slide {
                grid-template-columns: 1fr;
            }

            .slide-logo-orbit {
                margin-bottom: 0.75rem;
            }
        }

        @media (max-width: 640px) {
            .hero-text h2 {
                font-size: 2rem;
            }

            .stat-item h3 {
                font-size: 2.5rem;
            }

            .services-grid,
            .model-features {
                grid-template-columns: 1fr;
            }

            .hero-slider {
                padding: 1.75rem 1.75rem 2.25rem;
            }
        }

        /* Scroll Animations */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.6s ease, transform 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Loading Animation */
        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .logo:hover {
            animation: rotate 1s ease-in-out;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav id="navbar">
        <div class="nav-container">
            <div class="logo-container">
                <!-- Use the exact brand logo -->
                <img src="https://agi-prod-file-upload-public-main-use1.s3.amazonaws.com/4f9e60f6-2d9e-475f-b0f1-cf9f812f2d26" alt="Otocinclus Logo" class="logo">
                <div class="logo-text">
                    <h1>OTOCINCLUS</h1>
                    <p>TECHNOLOGY</p>
                </div>
            </div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#models">Engagement Models</a></li>
                <li><a href="#recruitment">Recruitment</a></li>
                <li><a href="#case-studies">Case Studies</a></li>
                <li><a href="#contact" class="cta-button">Get Started</a></li>
            </ul>
            <div class="mobile-menu">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </div>
    </nav>

    <!-- Hero Section with Core Value Slideshow -->
    <section id="home" class="hero">
        <div class="hero-content">
            <div class="hero-text">
                <h2>We Remove the <span class="highlight">Admin Trap</span></h2>
                <p class="tagline">Audit. Advise. Implement. Transfer.</p>
                <p>Otocinclus is your <strong>HR Consultancy &amp; HRMS Implementation Partner</strong> delivering integrated HR infrastructure for India's growing businesses. We build professional HR systems, operate them flawlessly, and transfer them to your team when you're ready.</p>
                <div class="hero-buttons">
                    <a href="#contact" class="btn-primary">Schedule Consultation</a>
                    <a href="#services" class="btn-secondary">Explore Services</a>
                </div>
            </div>
            <div class="hero-visual">
                <div class="hero-slider" aria-label="Otocinclus core value propositions">
                    <!-- Slide 1: We Remove the Admin Trap -->
                    <div class="slider-slide active" data-slide="0">
                        <div class="slide-logo-orbit">
                            <img src="https://agi-prod-file-upload-public-main-use1.s3.amazonaws.com/4f9e60f6-2d9e-475f-b0f1-cf9f812f2d26" alt="Otocinclus Logo">
                        </div>
                        <div>
                            <div class="slide-content-tag">
                                <span>Core 01</span> · <span>Admin Trap</span>
                            </div>
                            <h3 class="slide-heading">We Remove the Admin Trap</h3>
                            <p class="slide-subtitle">Free founders from HR firefighting so they can reclaim strategic time and grow confidently.</p>
                            <ul class="slide-points">
                                <li><strong>Audit &amp; Diagnose:</strong> Map your current HR, payroll and compliance risks across the employee lifecycle.</li>
                                <li><strong>Design Infrastructure:</strong> Create policies, processes and HRMS configuration tailored to your stage and industry.</li>
                                <li><strong>Run Operations:</strong> We handle payroll, attendance, compliance and employee records as your managed HR team.</li>
                                <li><strong>Transfer Ownership:</strong> When you are ready, we train your internal HR, hand over SOPs, and stay as your implementation partner.</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Slide 2: Flat 7% Recruitment -->
                    <div class="slider-slide" data-slide="1">
                        <div class="slide-logo-orbit">
                            <img src="https://agi-prod-file-upload-public-main-use1.s3.amazonaws.com/4f9e60f6-2d9e-475f-b0f1-cf9f812f2d26" alt="Otocinclus Logo">
                        </div>
                        <div>
                            <div class="slide-content-tag" style="background: rgba(232,159,95,0.12); color: #E89F5F;">
                                <span>Core 02</span> · <span>Flat 7% Hiring</span>
                            </div>
                            <h3 class="slide-heading">Flat 7% Recruitment – All Levels</h3>
                            <p class="slide-subtitle">Transparent, affordable hiring without a leadership penalty. Recruitment is a separate, flat 7% service.</p>
                            <ul class="slide-points">
                                <li><strong>One Rate for All Levels:</strong> 7% of annual CTC across junior, mid and senior roles – no hidden slabs.</li>
                                <li><strong>Integrated Delivery:</strong> Sourcing, screening, interview coordination, offer negotiation and joining support.</li>
                                <li><strong>Admin-Light for Founders:</strong> Our HR &amp; payroll integration means candidates join with ready HRMS, payroll and compliance setups.</li>
                                <li><strong>Affordable vs Market:</strong> Typical agencies charge 8.33–20% – Otocinclus keeps hiring budgets predictable and sustainable.</li>
                            </ul>

                            <div class="price-graphic" aria-hidden="true">
                                <div class="price-bar-row">
                                    <span class="price-label">Junior</span>
                                    <div class="price-bar-track">
                                        <div class="price-bar-fill" style="width: 80%;"></div>
                                    </div>
                                    <span style="font-size:0.75rem;">8.33% → 7%</span>
                                </div>
                                <div class="price-bar-row">
                                    <span class="price-label">Mid</span>
                                    <div class="price-bar-track">
                                        <div class="price-bar-fill" style="width: 95%;"></div>
                                    </div>
                                    <span style="font-size:0.75rem;">12–15% → 7%</span>
                                </div>
                                <div class="price-bar-row">
                                    <span class="price-label">Senior</span>
                                    <div class="price-bar-track">
                                        <div class="price-bar-fill senior" style="width: 100%;"></div>
                                    </div>
                                    <span style="font-size:0.75rem;">20%+ → 7%</span>
                                </div>
                                <p class="price-note">Recruitment is billed separately at a flat 7% fee, keeping all other HR services affordable and transparent.</p>
                            </div>
                        </div>
                    </div>

                    <div class="hero-slider-controls">
                        <div class="slider-dots">
                            <button class="slider-dot active" aria-label="Admin Trap slide"></button>
                            <button class="slider-dot" aria-label="Flat 7% Recruitment slide"></button>
                        </div>
                        <div class="slider-caption">
                            Swipe or tap dots to explore how Otocinclus removes the Admin Trap and makes hiring affordable.
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="stats">
        <div class="stats-container">
            <div class="stat-item">
                <h3>30-65%</h3>
                <p>Cost Savings vs. Traditional Agencies</p>
            </div>
            <div class="stat-item">
                <h3>20+ Hours</h3>
                <p>Founder Bandwidth Reclaimed Monthly</p>
            </div>
            <div class="stat-item">
                <h3>28 Days</h3>
                <p>Reduced Time-to-Hire</p>
            </div>
            <div class="stat-item">
                <h3>99.5%</h3>
                <p>Payroll Accuracy Target</p>
            </div>
        </div>
    </section>

    <!-- Admin Trap Section -->
    <section id="admin-trap" class="admin-trap">
        <div class="admin-trap-container">
            <div class="section-title">
                <h2>The Admin Trap: Where Growth Stalls</h2>
                <p>Growing businesses between 15-100 employees face a critical inflection point. Too large for spreadsheets. Too small for a VP of HR. Too risky to ignore.</p>
            </div>
            <div class="admin-trap-content">
                <div class="trap-visual">
                    <div class="chart">
                        <svg viewBox="0 0 400 300" xmlns="http://www.w3.org/2000/svg">
                            <text x="10" y="20" font-size="14" fill="#626C71">Administrative Complexity</text>
                            <path d="M 50 250 L 50 50 L 350 50" stroke="#626C71" stroke-width="2" fill="none"/>
                            <path d="M 50 250 Q 100 240, 150 180 T 250 80 T 350 60" stroke="#4A90E2" stroke-width="4" fill="none"/>
                            <circle cx="150" cy="180" r="6" fill="#E89F5F"/>
                            <text x="140" y="210" font-size="12" fill="#E89F5F" font-weight="bold">The Admin Trap</text>
                            <text x="130" y="225" font-size="11" fill="#626C71">(15-100 employees)</text>
                            <text x="10" y="280" font-size="12" fill="#626C71">Employee Count →</text>
                        </svg>
                    </div>
                </div>
                <div class="trap-points">
                    <div class="trap-point">
                        <h4>⏱️ Time Drain</h4>
                        <p>Founders and CXOs spend 15-25 hours per week on HR administration - that's 25% of strategic capacity lost.</p>
                    </div>
                    <div class="trap-point">
                        <h4>⚖️ Compliance Risk</h4>
                        <p>New Social Security Code penalties include imprisonment and substantial fines. Ignorance is not protection.</p>
                    </div>
                    <div class="trap-point">
                        <h4>💸 Financial Loss</h4>
                        <p>30-40% higher effective HR costs due to hidden burdens like errors, delays, and opportunity costs.</p>
                    </div>
                    <div class="trap-point">
                        <h4>🎯 Strategic Impact</h4>
                        <p>Poor HR infrastructure blocks investor readiness, damages employer branding, and limits growth velocity.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <div class="services-container">
            <div class="section-title">
                <h2>Comprehensive HR Infrastructure Services</h2>
                <p>Full-stack HR solutions designed for growing businesses. We handle everything so you can focus on growth.</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">📋</div>
                    <h3>HR Governance &amp; Policy Design</h3>
                    <p>Build compliant, scalable HR foundations with professionally designed policies and organizational frameworks.</p>
                    <ul>
                        <li>HR policy &amp; employee handbook</li>
                        <li>Organizational structure &amp; role definitions</li>
                        <li>HR process mapping and SOPs</li>
                        <li>Compliance framework (PF, ESI, PT, labour laws)</li>
                    </ul>
                </div>

                <div class="service-card">
                    <div class="service-icon">💻</div>
                    <h3>HRMS Selection, Implementation &amp; Administration</h3>
                    <p>Vendor-agnostic HRMS implementation expertise. We help you select, configure, and operate the right system.</p>
                    <ul>
                        <li>HRMS selection &amp; fitment advisory</li>
                        <li>Complete configuration (payroll, attendance, leave)</li>
                        <li>Data migration from legacy systems</li>
                        <li>Ongoing HRMS administration &amp; support</li>
                        <li>HRMS training for internal teams</li>
                    </ul>
                </div>

                <div class="service-card">
                    <div class="service-icon">💰</div>
                    <h3>Payroll &amp; Statutory Compliance</h3>
                    <p>Accurate, timely payroll processing with zero compliance risk. Your compliance shield.</p>
                    <ul>
                        <li>Monthly payroll processing &amp; payslips</li>
                        <li>Statutory deductions &amp; filings (PF, ESI, PT, TDS)</li>
                        <li>Statutory returns &amp; challans</li>
                        <li>Full &amp; final settlements</li>
                        <li>Payroll MIS &amp; analytics reports</li>
                    </ul>
                </div>

                <div class="service-card">
                    <div class="service-icon">📅</div>
                    <h3>Attendance, Leave &amp; Time Management</h3>
                    <p>Automated attendance tracking with intelligent shift and leave management systems.</p>
                    <ul>
                        <li>Shift rules and attendance logic design</li>
                        <li>Leave policy design, setup, and tracking</li>
                        <li>Monthly attendance reconciliation</li>
                        <li>Attendance and leave dashboards</li>
                    </ul>
                </div>

                <div class="service-card">
                    <div class="service-icon">👥</div>
                    <h3>Employee Lifecycle Management</h3>
                    <p>Seamless employee journey management from onboarding to exit with complete documentation.</p>
                    <ul>
                        <li>End-to-end onboarding (documentation, KYC)</li>
                        <li>Employee records management (digital files)</li>
                        <li>Confirmation &amp; probation tracking</li>
                        <li>Appraisal cycle coordination support</li>
                        <li>Exit management, NOC, and F&amp;F settlements</li>
                    </ul>
                </div>

                <div class="service-card">
                    <div class="service-icon">🎯</div>
                    <h3>Recruitment Services (Flat 7% - All Levels)</h3>
                    <p>Industry-disrupting recruitment pricing. Same quality, transparent cost across all levels. <strong>Recruitment services charged separately at flat 7% - affordable rates compared to market standard.</strong></p>
                    <ul>
                        <li>Requirement understanding &amp; JD creation</li>
                        <li>Multi-channel sourcing &amp; screening</li>
                        <li>Interview coordination with hiring managers</li>
                        <li>Offer negotiation support</li>
                        <li>Joining &amp; onboarding coordination</li>
                        <li>90-day free replacement guarantee</li>
                    </ul>
                </div>

                <div class="service-card">
                    <div class="service-icon">🎓</div>
                    <h3>Capability Building &amp; Handover</h3>
                    <p>Knowledge transfer and training to empower your internal HR team for independence.</p>
                    <ul>
                        <li>HRMS admin training for internal HR</li>
                        <li>Payroll &amp; compliance training</li>
                        <li>Process walkthroughs with SOP handover</li>
                        <li>Knowledge transfer sessions</li>
                        <li>Post-handover support</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Models Section -->
    <section id="models" class="models">
        <div class="models-container">
            <div class="section-title">
                <h2>Engagement Models Designed for Your Journey</h2>
                <p>Choose the model that matches your growth stage and internal capabilities.</p>
            </div>
            
            <div class="models-tabs">
                <button class="tab-button active" onclick="switchTab('model1')">Model 1: Managed HR Services</button>
                <button class="tab-button" onclick="switchTab('model2')">Model 2: Build-Operate-Transfer</button>
            </div>

            <div id="model1" class="tab-content active">
                <div class="model-content">
                    <h3 style="font-size: 2rem; color: var(--dark-navy); margin-bottom: 1rem;">Complete Outsourced HR Services (Managed HR)</h3>
                    <p style="font-size: 1.125rem; color: var(--text-light); margin-bottom: 2rem;">Best for companies who want us to handle everything. We act as your extended HR department.</p>
                    
                    <div class="model-flow">
                        <div class="flow-step">
                            <h4>Start</h4>
                            <p>Initial Audit</p>
                        </div>
                        <div class="flow-step">
                            <h4>Audit</h4>
                            <p>Gap Analysis</p>
                        </div>
                        <div class="flow-step">
                            <h4>Setup</h4>
                            <p>Implementation</p>
                        </div>
                        <div class="flow-step">
                            <h4>Operate</h4>
                            <p>Ongoing Management</p>
                        </div>
                    </div>

                    <div class="model-features">
                        <div class="feature-box">
                            <h4>HR Policy &amp; Process Setup</h4>
                            <ul>
                                <li>HR policies &amp; employee handbook</li>
                                <li>Organizational structure &amp; role definitions</li>
                                <li>HR process mapping &amp; documentation</li>
                                <li>Compliance framework setup</li>
                            </ul>
                        </div>
                        <div class="feature-box">
                            <h4>HRMS Implementation &amp; Management</h4>
                            <ul>
                                <li>HRMS selection support</li>
                                <li>Complete system configuration</li>
                                <li>Employee master data setup</li>
                                <li>Ongoing HRMS administration</li>
                            </ul>
                        </div>
                        <div class="feature-box">
                            <h4>Payroll &amp; Compliance</h4>
                            <ul>
                                <li>Monthly payroll processing</li>
                                <li>Statutory deductions &amp; filings</li>
                                <li>Payroll reports &amp; MIS</li>
                                <li>Full compliance management</li>
                            </ul>
                        </div>
                        <div class="feature-box">
                            <h4>Employee Lifecycle Management</h4>
                            <ul>
                                <li>Onboarding &amp; documentation</li>
                                <li>Employee records management</li>
                                <li>Confirmation &amp; appraisal support</li>
                                <li>Exit management &amp; F&amp;F settlement</li>
                            </ul>
                        </div>
                    </div>

                    <div style="background: var(--white); padding: 2rem; border-radius: 15px; margin-top: 3rem; text-align: center;">
                        <h4 style="font-size: 1.5rem; color: var(--primary-blue); margin-bottom: 1rem;">Outcome</h4>
                        <p style="font-size: 1.125rem; color: var(--text-light);">Get a fully functional HR department without hiring an internal HR team. Per-employee monthly subscription model provides predictable costs and enterprise-grade HR infrastructure.</p>
                    </div>
                </div>
            </div>

            <div id="model2" class="tab-content">
                <div class="model-content">
                    <h3 style="font-size: 2rem; color: var(--dark-navy); margin-bottom: 1rem;">HR Setup + Transition to Client HR Team</h3>
                    <p style="font-size: 1.125rem; color: var(--text-light); margin-bottom: 2rem;">Best for companies planning to build an internal HR team. We set up, stabilize, then hand over.</p>
                    
                    <div class="model-flow">
                        <div class="flow-step">
                            <h4>Phase 1</h4>
                            <p>HR Setup &amp; HRMS Implementation</p>
                        </div>
                        <div class="flow-step">
                            <h4>Phase 2</h4>
                            <p>Initial Operations (2-3 Months)</p>
                        </div>
                        <div class="flow-step">
                            <h4>Phase 3</h4>
                            <p>Training &amp; Handover</p>
                        </div>
                    </div>

                    <div class="model-features">
                        <div class="feature-box">
                            <h4>Phase 1: HR Setup &amp; HRMS Implementation</h4>
                            <ul>
                                <li>HR policy &amp; handbook creation</li>
                                <li>Compliance &amp; statutory setup</li>
                                <li>HRMS implementation</li>
                                <li>Payroll, attendance &amp; leave setup</li>
                                <li>Employee data migration</li>
                                <li>Process documentation (SOPs)</li>
                            </ul>
                        </div>
                        <div class="feature-box">
                            <h4>Phase 2: Initial Operations (2-3 Months)</h4>
                            <ul>
                                <li>Payroll processing &amp; compliance filings</li>
                                <li>Attendance &amp; leave administration</li>
                                <li>Employee lifecycle support</li>
                                <li>HRMS monitoring &amp; fine-tuning</li>
                                <li>Issue resolution &amp; stabilization</li>
                            </ul>
                        </div>
                        <div class="feature-box">
                            <h4>Phase 3: Training &amp; Handover</h4>
                            <ul>
                                <li>HRMS training for internal HR</li>
                                <li>Payroll &amp; compliance training</li>
                                <li>Process walkthroughs &amp; SOP handover</li>
                                <li>Knowledge transfer sessions</li>
                                <li>Post-handover support (as required)</li>
                            </ul>
                        </div>
                    </div>

                    <div style="background: var(--white); padding: 2rem; border-radius: 15px; margin-top: 3rem; text-align: center;">
                        <h4 style="font-size: 1.5rem; color: var(--primary-blue); margin-bottom: 1rem;">Outcome</h4>
                        <p style="font-size: 1.125rem; color: var(--text-light);">Your internal HR team inherits a professionally built, fully operational HR system with complete documentation, training, and post-handover support. You own the function.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Recruitment Section -->
    <section id="recruitment" class="recruitment">
        <div class="recruitment-container">
            <div class="section-title" style="color: var(--white);">
                <h2>Recruitment Services: Flat 7% - All Levels</h2>
                <p style="color: rgba(255, 255, 255, 0.95);">We eliminate the "Leadership Penalty" charged by traditional agencies. Same quality, transparent pricing across all levels. <strong>Charged separately at affordable rates below market standard.</strong></p>
            </div>

            <div class="recruitment-content">
                <div class="pricing-comparison">
                    <h3>Pricing Comparison</h3>
                    <div class="comparison-item">
                        <span>Traditional Agency - Junior</span>
                        <span>8.33%</span>
                    </div>
                    <div class="comparison-item">
                        <span>Traditional Agency - Mid</span>
                        <span>12-15%</span>
                    </div>
                    <div class="comparison-item">
                        <span>Traditional Agency - Senior</span>
                        <span>20%+</span>
                    </div>
                    <div class="comparison-item" style="border-top: 2px solid rgba(255, 255, 255, 0.4); padding-top: 1.5rem; margin-top: 1.5rem;">
                        <span style="font-size: 1.5rem;">Otocinclus - All Levels</span>
                        <span style="font-size: 1.75rem; color: #E89F5F;">7%</span>
                    </div>
                </div>

                <div class="recruitment-benefits">
                    <div class="benefit-item">
                        <h4>💰 30-65% Savings on Senior Hires</h4>
                        <p>Traditional agencies charge 20%+ for leadership roles. We charge flat 7% regardless of seniority, saving you massive costs on critical hires.</p>
                    </div>
                    <div class="benefit-item">
                        <h4>🎯 Comprehensive Recruitment Support</h4>
                        <p>Includes sourcing, screening, interview coordination, offer negotiation, joining coordination, and 90-day free replacement guarantee.</p>
                    </div>
                    <div class="benefit-item">
                        <h4>⚡ Faster Turnaround</h4>
                        <p>28 days average time-to-hire (down from industry standard 45 days). Integration with our HR &amp; payroll operations enables seamless onboarding.</p>
                    </div>
                    <div class="benefit-item">
                        <h4>🤝 Continued Support Post-HR Handover</h4>
                        <p>Recruitment services can continue even after HR handover in Model 2, providing long-term talent acquisition support.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Case Studies Section -->
    <section id="case-studies" class="case-studies">
        <div class="case-studies-container">
            <div class="section-title">
                <h2>Success Stories: Real Impact, Real Results</h2>
                <p>See how we've helped growing businesses break free from the Admin Trap and scale confidently.</p>
            </div>

            <div class="case-study-card fade-in">
                <div class="case-study-header">
                    <div class="case-study-info">
                        <h3>SaaS Startup - 45 Employees</h3>
                        <p>Industry: B2B SaaS | Challenge: Scaling from 15 to 45 employees in 8 months</p>
                    </div>
                    <div class="case-study-metrics">
                        <div class="metric">
                            <h4>20 Hours</h4>
                            <p>Founder Time Saved/Week</p>
                        </div>
                        <div class="metric">
                            <h4>Zero</h4>
                            <p>Compliance Issues</p>
                        </div>
                        <div class="metric">
                            <h4>100%</h4>
                            <p>Payroll Accuracy</p>
                        </div>
                    </div>
                </div>
                <div class="case-study-body">
                    <div class="challenge">
                        <h4>The Challenge</h4>
                        <p>Founder was spending 25+ hours weekly on HR tasks using spreadsheets. Rapid hiring created compliance risks. Lack of professional HR infrastructure was blocking Series A funding discussions.</p>
                    </div>
                    <div class="solution">
                        <h4>Otocinclus Solution</h4>
                        <p>Implemented Model 1 (Managed HR Services). Set up GreytHR with complete payroll configuration. Established compliance framework for PF, ESI, PT. Onboarded 30 new employees seamlessly during growth phase. Result: Clean due diligence for Series A raise.</p>
                    </div>
                </div>
            </div>

            <div class="case-study-card fade-in">
                <div class="case-study-header">
                    <div class="case-study-info">
                        <h3>Manufacturing Company - 80 Employees</h3>
                        <p>Industry: Manufacturing | Challenge: Transition to internal HR team</p>
                    </div>
                    <div class="case-study-metrics">
                        <div class="metric">
                            <h4>6 Months</h4>
                            <p>Complete Handover</p>
                        </div>
                        <div class="metric">
                            <h4>52%</h4>
                            <p>Cost Savings vs Agency</p>
                        </div>
                        <div class="metric">
                            <h4>3 Months</h4>
                            <p>Senior Hire Time</p>
                        </div>
                    </div>
                </div>
                <div class="case-study-body">
                    <div class="challenge">
                        <h4>The Challenge</h4>
                        <p>Company was ready to hire internal HR team but lacked systems and processes. Previous agency recruitment costs were 15-20% per hire. Needed professional HRMS but no expertise to implement.</p>
                    </div>
                    <div class="solution">
                        <h4>Otocinclus Solution</h4>
                        <p>Deployed Model 2 (Build-Operate-Transfer). Phase 1: Implemented Keka HRMS with complete configuration. Phase 2: Ran operations for 3 months while hiring internal HR. Phase 3: Trained internal team with SOP handover. Recruited 5 senior positions at flat 7% (saved ₹12L+ vs traditional agency fees).</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="contact-container">
            <div class="contact-info">
                <h3>Ready to Remove the Admin Trap?</h3>
                <p>Schedule a free HR infrastructure audit. We'll analyze your current state, identify risks, and recommend the right engagement model for your business.</p>
                
                <div class="contact-details">
                    <div class="contact-item">
                        <div class="contact-icon">📍</div>
                        <div class="contact-item-text">
                            <h4>Location</h4>
                            <p>Bengaluru, Karnataka, India</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">📧</div>
                        <div class="contact-item-text">
                            <h4>Email</h4>
                            <p>contact@otocinclus.com</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">📞</div>
                        <div class="contact-item-text">
                            <h4>Phone</h4>
                            <p>+91 XXXXX XXXXX</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="contact-form">
                <form id="contactForm">
                    <div class="form-group">
                        <label for="name">Full Name *</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email Address *</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="phone">Phone Number *</label>
                        <input type="tel" id="phone" name="phone" required>
                    </div>
                    <div class="form-group">
                        <label for="company">Company Name *</label>
                        <input type="text" id="company" name="company" required>
                    </div>
                    <div class="form-group">
                        <label for="employees">Number of Employees *</label>
                        <select id="employees" name="employees" required>
                            <option value="">Select range</option>
                            <option value="1-15">1-15 employees</option>
                            <option value="15-50">15-50 employees</option>
                            <option value="50-100">50-100 employees</option>
                            <option value="100-250">100-250 employees</option>
                            <option value="250+">250+ employees</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="interest">Service Interest *</label>
                        <select id="interest" name="interest" required>
                            <option value="">Select service</option>
                            <option value="model1">Model 1: Managed HR Services</option>
                            <option value="model2">Model 2: Build-Operate-Transfer</option>
                            <option value="recruitment">Recruitment Services Only</option>
                            <option value="hrms">HRMS Implementation Only</option>
                            <option value="consultation">Free HR Audit</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message">Tell us about your HR challenges</label>
                        <textarea id="message" name="message" rows="4"></textarea>
                    </div>
                    <button type="submit" class="submit-btn">Schedule Free Consultation</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-container">
            <div class="footer-section">
                <h4>Otocinclus Technology</h4>
                <p>The integrated HR infrastructure layer enabling India's SME growth engine. We audit, advise, implement, and transfer.</p>
                <p style="margin-top: 1rem;"><strong>Mission:</strong> To ensure no business fails due to administrative burden or compliance ignorance.</p>
            </div>
            <div class="footer-section">
                <h4>Services</h4>
                <ul class="footer-links">
                    <li><a href="#services">HR Governance &amp; Policy Design</a></li>
                    <li><a href="#services">HRMS Implementation</a></li>
                    <li><a href="#services">Payroll &amp; Compliance</a></li>
                    <li><a href="#services">Recruitment Services (7%)</a></li>
                    <li><a href="#services">Employee Lifecycle Management</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h4>Engagement Models</h4>
                <ul class="footer-links">
                    <li><a href="#models">Model 1: Managed HR Services</a></li>
                    <li><a href="#models">Model 2: Build-Operate-Transfer</a></li>
                    <li><a href="#recruitment">Flat 7% Recruitment</a></li>
                    <li><a href="#case-studies">Case Studies</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h4>Company</h4>
                <ul class="footer-links">
                    <li><a href="#home">About Us</a></li>
                    <li><a href="#admin-trap">The Admin Trap</a></li>
                    <li><a href="#contact">Contact Us</a></li>
                    <li><a href="#contact">Free HR Audit</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2026 Otocinclus Technology. All rights reserved. | HR Consultancy &amp; HRMS Implementation Partner | Bengaluru, Karnataka</p>
        </div>
    </footer>

    <script>
        // Navbar scroll effect
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        });

        // Smooth scroll for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                const href = this.getAttribute('href');
                if (href && href.startsWith('#')) {
                    e.preventDefault();
                    const target = document.querySelector(href);
                    if (target) {
                        target.scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                    }
                }
            });
        });

        // Tab switching
        function switchTab(modelId) {
            const tabs = document.querySelectorAll('.tab-content');
            const buttons = document.querySelectorAll('.tab-button');
            
            tabs.forEach(tab => tab.classList.remove('active'));
            buttons.forEach(btn => btn.classList.remove('active'));
            
            const targetTab = document.getElementById(modelId);
            if (targetTab) {
                targetTab.classList.add('active');
            }
            // event may not exist if called programmatically, so guard it
            if (window.event && window.event.target) {
                window.event.target.classList.add('active');
            }
        }

        // Scroll animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Form submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const formData = new FormData(this);
            const data = Object.fromEntries(formData);
            console.log('Form submitted:', data);
            alert('Thank you for your interest! We will contact you within 24 hours to schedule your free HR infrastructure audit.');
            this.reset();
        });

        // Mobile menu toggle (basic implementation)
        document.querySelector('.mobile-menu').addEventListener('click', function() {
            const navLinks = document.querySelector('.nav-links');
            if (navLinks.style.display === 'flex') {
                navLinks.style.display = 'none';
            } else {
                navLinks.style.display = 'flex';
                navLinks.style.flexDirection = 'column';
                navLinks.style.background = 'rgba(255,255,255,0.98)';
                navLinks.style.position = 'absolute';
                navLinks.style.top = '64px';
                navLinks.style.right = '16px';
                navLinks.style.padding = '1.25rem 1.5rem';
                navLinks.style.borderRadius = '16px';
                navLinks.style.boxShadow = '0 10px 40px rgba(0,0,0,0.12)';
                navLinks.style.gap = '1rem';
            }
        });

        // Counter animation for stats
        function animateValue(element, start, end, duration, suffix) {
            let startTimestamp = null;
            const step = (timestamp) => {
                if (!startTimestamp) startTimestamp = timestamp;
                const progress = Math.min((timestamp - startTimestamp) / duration, 1);
                const value = Math.floor(progress * (end - start) + start);
                element.textContent = value + (suffix || '');
                if (progress < 1) {
                    window.requestAnimationFrame(step);
                }
            };
            window.requestAnimationFrame(step);
        }

        // Trigger counter animation when stats section is visible
        const statsObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const statItems = entry.target.querySelectorAll('.stat-item h3');
                    statItems.forEach(stat => {
                        const text = stat.textContent.trim();
                        if (text.includes('%')) {
                            const num = parseInt(text);
                            animateValue(stat, 0, num, 2000, '%');
                        } else if (text.includes('+')) {
                            const num = parseInt(text);
                            animateValue(stat, 0, num, 2000, '+');
                        } else if (!isNaN(parseInt(text))) {
                            const num = parseInt(text);
                            animateValue(stat, 0, num, 2000, '');
                        }
                    });
                    statsObserver.unobserve(entry.target);
                }
            });
        }, { threshold: 0.5 });

        const statsSection = document.querySelector('.stats');
        if (statsSection) {
            statsObserver.observe(statsSection);
        }

        // Hero slider logic (Admin Trap + Flat 7% Recruitment)
        (function() {
            const slides = document.querySelectorAll('.hero-slider .slider-slide');
            const dots = document.querySelectorAll('.hero-slider .slider-dot');
            let currentSlide = 0;
            let intervalId = null;
            const SLIDE_DURATION = 8000;

            function showSlide(index) {
                if (!slides.length) return;
                slides[currentSlide].classList.remove('active');
                dots[currentSlide].classList.remove('active');
                currentSlide = (index + slides.length) % slides.length;
                slides[currentSlide].classList.add('active');
                dots[currentSlide].classList.add('active');
            }

            function startAutoPlay() {
                stopAutoPlay();
                intervalId = setInterval(() => {
                    showSlide(currentSlide + 1);
                }, SLIDE_DURATION);
            }

            function stopAutoPlay() {
                if (intervalId) {
                    clearInterval(intervalId);
                    intervalId = null;
                }
            }

            dots.forEach((dot, index) => {
                dot.addEventListener('click', () => {
                    stopAutoPlay();
                    showSlide(index);
                    startAutoPlay();
                });
            });

            // Start autoplay when DOM is ready
            if (slides.length) {
                startAutoPlay();
            }
        })();
    </script>
</body>
</html>
