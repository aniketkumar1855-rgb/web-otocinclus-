<!doctype html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Otocinclus - HR Consultancy &amp; HRMS Implementation Partner | Build, Operate, Transfer</title>
  <meta name="description" content="Otocinclus delivers integrated HR infrastructure for India's growing businesses. Expert HR consultancy, HRMS implementation, payroll compliance, flat 7% recruitment services. We audit, advise, implement, and transfer." />
  <meta name="keywords" content="HR consultancy, HRMS implementation, payroll services, recruitment agency, HR outsourcing, compliance management, Build-Operate-Transfer, SME HR solutions" />

  <style>
    :root{
      --primary-blue:#4A90E2;
      --secondary-blue:#5BA3F5;
      --accent-orange:#E89F5F;
      --dark-navy:#1F2533;
      --light-bg:#FCFCF9;
      --text-dark:#1F2533;
      --text-light:#626C71;
      --white:#FFFFFF;
      --gradient-primary:linear-gradient(135deg, #4A90E2 0%, #5BA3F5 100%);
      --gradient-secondary:linear-gradient(135deg, #E89F5F 0%, #F5B87F 100%);
      --shadow-sm:0 5px 20px rgba(0,0,0,0.08);
      --shadow-md:0 10px 40px rgba(0,0,0,0.10);
      --radius-lg:20px;
      --radius-md:15px;
      --radius-sm:10px;
      --nav-height:90px;
    }

    *{margin:0;padding:0;box-sizing:border-box;}
    html{scroll-behavior:smooth;}
    body{
      font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
      color:var(--text-dark);
      line-height:1.6;
      overflow-x:hidden;
      background-color:var(--light-bg);
    }

    /* Fixed navbar offset for anchors */
    section{scroll-margin-top:90px;}

    a{color:inherit;}
    img{max-width:100%;height:auto;display:block;}

    /* Navigation */
    nav{
      position:fixed;
      top:0;
      left:0;
      width:100%;
      background:rgba(255,255,255,0.95);
      backdrop-filter:blur(10px);
      box-shadow:0 2px 20px rgba(0,0,0,0.10);
      z-index:1000;
      transition:all 0.3s ease;
    }
    nav.scrolled{
      box-shadow:0 4px 30px rgba(0,0,0,0.15);
    }
    .nav-container{
      max-width:1400px;
      margin:0 auto;
      padding:1rem 2rem;
      display:flex;
      justify-content:space-between;
      align-items:center;
      gap:1rem;
      min-height:var(--nav-height);
    }
    .logo-container{
      display:flex;
      align-items:center;
      gap:1rem;
      min-width:240px;
    }
    .logo{
      width:50px;
      height:50px;
      animation:float 3s ease-in-out infinite;
    }
    @keyframes float{
      0%,100%{transform:translateY(0px);}
      50%{transform:translateY(-10px);}
    }
    .logo-text{
      display:flex;
      flex-direction:column;
      line-height:1.15;
    }
    .logo-text h1{
      font-size:1.5rem;
      font-weight:800;
      color:var(--dark-navy);
      letter-spacing:-0.5px;
    }
    .logo-text p{
      font-size:0.875rem;
      color:var(--primary-blue);
      font-weight:600;
      letter-spacing:0.5px;
    }

    .nav-links{
      display:flex;
      list-style:none;
      gap:2rem;
      align-items:center;
    }
    .nav-links a{
      text-decoration:none;
      color:var(--text-dark);
      font-weight:600;
      font-size:1rem;
      transition:color 0.3s ease;
      position:relative;
      white-space:nowrap;
    }
    .nav-links a::after{
      content:"";
      position:absolute;
      bottom:-6px;
      left:0;
      width:0%;
      height:2px;
      background:var(--gradient-primary);
      transition:width 0.3s ease;
    }
    .nav-links a:hover{color:var(--primary-blue);}
    .nav-links a:hover::after{width:100%;}

    .cta-button{
      background:var(--gradient-primary);
      color:var(--white);
      padding:0.75rem 1.5rem;
      border-radius:999px;
      text-decoration:none;
      font-weight:700;
      transition:transform 0.3s ease, box-shadow 0.3s ease;
      box-shadow:0 4px 15px rgba(74,144,226,0.30);
    }
    .cta-button:hover{
      transform:translateY(-2px);
      box-shadow:0 6px 25px rgba(74,144,226,0.40);
    }

    .mobile-menu{
      display:none;
      flex-direction:column;
      gap:5px;
      cursor:pointer;
      padding:0.5rem;
      border-radius:10px;
      border:2px solid rgba(0,0,0,0.05);
      background:rgba(255,255,255,0.7);
    }
    .mobile-menu span{
      width:25px;
      height:3px;
      background:var(--text-dark);
      border-radius:2px;
      transition:all 0.3s ease;
    }
    .nav-mobile-panel{
      display:none;
      width:100%;
      padding:0 2rem 1rem;
    }
    .nav-mobile-panel.open{display:block;}
    .nav-mobile-links{
      list-style:none;
      display:flex;
      flex-direction:column;
      gap:0.75rem;
      padding:0.75rem 0 0.25rem;
      border-top:1px solid rgba(0,0,0,0.06);
    }
    .nav-mobile-links a{
      text-decoration:none;
      font-weight:700;
      padding:0.75rem 0.75rem;
      border-radius:12px;
      background:rgba(74,144,226,0.06);
      color:var(--dark-navy);
    }
    .nav-mobile-links a.cta-button{
      display:inline-block;
      width:max-content;
      padding:0.9rem 1.1rem;
      border-radius:999px;
      background:var(--gradient-primary);
      color:var(--white);
    }

    /* Core values slideshow */
    .core-values{
      background:linear-gradient(135deg, rgba(74,144,226,0.03) 0%, rgba(232,159,95,0.03) 100%);
      padding:2rem 0 1rem;
      margin-top:80px;
    }
    .core-values-container{
      max-width:1400px;
      margin:0 auto;
      padding:0 2rem;
    }
    .slideshow-wrapper{
      position:relative;
      overflow:hidden;
      border-radius:var(--radius-lg);
      background:var(--white);
      box-shadow:0 10px 50px rgba(0,0,0,0.10);
    }
    .slide{
      display:none;
      animation:slideIn 0.5s ease;
    }
    .slide.active{display:block;}
    @keyframes slideIn{
      from{opacity:0;transform:translateX(30px);}
      to{opacity:1;transform:translateX(0);}
    }
    .slide-content{
      display:grid;
      grid-template-columns:1fr 1.5fr;
      gap:3rem;
      padding:3rem;
      align-items:center;
      min-height:500px;
    }
    .slide-graphic{
      display:flex;
      align-items:center;
      justify-content:center;
      padding:2rem;
    }
    .slide-text h2{
      font-size:2.5rem;
      font-weight:900;
      color:var(--dark-navy);
      margin-bottom:0.5rem;
      line-height:1.2;
      letter-spacing:-0.5px;
    }
    .highlight-orange{color:var(--accent-orange);}
    .slide-text .subtitle{
      font-size:1.125rem;
      color:var(--text-light);
      margin-bottom:2rem;
      font-weight:600;
    }
    .how-points{
      display:flex;
      flex-direction:column;
      gap:1.25rem;
      margin-bottom:2rem;
    }
    .how-point{
      display:flex;
      gap:1rem;
      align-items:flex-start;
      padding:1rem;
      background:linear-gradient(135deg, rgba(74,144,226,0.05) 0%, rgba(232,159,95,0.05) 100%);
      border-radius:12px;
      transition:transform 0.3s ease, box-shadow 0.3s ease;
    }
    .how-point:hover{
      transform:translateX(5px);
      box-shadow:0 5px 15px rgba(0,0,0,0.08);
    }
    .point-icon{
      font-size:2rem;
      flex-shrink:0;
      width:2.25rem;
      line-height:1;
      display:flex;
      align-items:center;
      justify-content:center;
      color:var(--primary-blue);
    }
    .point-text h4{
      font-size:1rem;
      color:var(--primary-blue);
      margin-bottom:0.25rem;
      font-weight:800;
    }
    .point-text p{
      font-size:0.9375rem;
      color:var(--text-light);
      margin:0;
      line-height:1.5;
    }

    .pricing-showcase{
      display:flex;
      flex-direction:column;
      gap:1rem;
      margin-bottom:2rem;
    }
    .pricing-bar{
      display:flex;
      align-items:center;
      gap:1rem;
    }
    .bar-label{
      min-width:150px;
      font-size:0.9375rem;
      color:var(--text-dark);
      font-weight:700;
    }
    .bar-container{
      flex:1;
      background:rgba(0,0,0,0.05);
      border-radius:20px;
      height:40px;
      position:relative;
      overflow:hidden;
    }
    .bar{
      height:100%;
      border-radius:20px;
      display:flex;
      align-items:center;
      justify-content:flex-end;
      padding-right:1rem;
      transition:width 1.5s ease;
    }
    .bar.traditional{
      background:linear-gradient(90deg, rgba(255,107,107,0.60) 0%, rgba(255,107,107,0.80) 100%);
    }
    .bar.otocinclus{
      background:var(--gradient-secondary);
      animation:barPulse 2s ease-in-out infinite;
    }
    @keyframes barPulse{
      0%,100%{opacity:0.9;}
      50%{opacity:1;}
    }
    .bar-value{
      color:var(--white);
      font-weight:900;
      font-size:0.9375rem;
      text-shadow:0 1px 3px rgba(0,0,0,0.30);
    }
    .highlight-bar{
      margin-top:0.5rem;
      padding-top:1rem;
      border-top:2px solid var(--accent-orange);
    }
    .highlight-bar .bar-label{
      font-size:1rem;
      color:var(--accent-orange);
    }

    .recruitment-benefits-quick{
      display:flex;
      flex-wrap:wrap;
      gap:1.5rem;
      margin-bottom:2rem;
    }
    .benefit-quick{
      display:flex;
      align-items:center;
      gap:0.5rem;
      font-size:0.9375rem;
      color:var(--text-dark);
      font-weight:700;
      padding:0.5rem 0.75rem;
      border-radius:999px;
      background:rgba(74,144,226,0.06);
    }
    .benefit-icon{
      font-size:1.25rem;
      line-height:1;
      color:var(--accent-orange);
    }

    .slide-cta{
      display:flex;
      gap:1rem;
      flex-wrap:wrap;
    }
    .btn-slide{
      background:var(--gradient-primary);
      color:var(--white);
      padding:0.875rem 2rem;
      border-radius:999px;
      text-decoration:none;
      font-weight:800;
      font-size:1rem;
      transition:transform 0.3s ease, box-shadow 0.3s ease;
      box-shadow:0 4px 15px rgba(74,144,226,0.30);
      display:inline-block;
    }
    .btn-slide:hover{
      transform:translateY(-2px);
      box-shadow:0 6px 25px rgba(74,144,226,0.40);
    }

    .slide-controls{
      display:flex;
      align-items:center;
      justify-content:center;
      gap:2rem;
      padding:1.5rem;
      background:linear-gradient(135deg, rgba(74,144,226,0.05) 0%, rgba(232,159,95,0.05) 100%);
    }
    .slide-control{
      background:var(--white);
      border:2px solid var(--primary-blue);
      color:var(--primary-blue);
      width:40px;
      height:40px;
      border-radius:50%;
      font-size:1.5rem;
      cursor:pointer;
      transition:all 0.3s ease;
      display:flex;
      align-items:center;
      justify-content:center;
      font-weight:900;
      line-height:1;
    }
    .slide-control:hover{
      background:var(--primary-blue);
      color:var(--white);
      transform:scale(1.08);
    }
    .slide-dots{
      display:flex;
      gap:0.75rem;
      align-items:center;
      justify-content:center;
    }
    .dot{
      width:12px;
      height:12px;
      border-radius:50%;
      background:rgba(74,144,226,0.30);
      cursor:pointer;
      transition:all 0.3s ease;
      display:inline-block;
    }
    .dot.active{
      background:var(--primary-blue);
      width:30px;
      border-radius:6px;
    }
    .dot:hover{background:var(--primary-blue);}

    /* Hero */
    .hero{
      min-height:100vh;
      display:flex;
      align-items:center;
      justify-content:center;
      background:linear-gradient(135deg, rgba(74,144,226,0.05) 0%, rgba(232,159,95,0.05) 100%);
      padding:6rem 2rem 4rem;
      position:relative;
      overflow:hidden;
    }
    .hero::before{
      content:"";
      position:absolute;
      top:-50px;
      right:-20px;
      width:800px;
      height:800px;
      background:radial-gradient(circle, rgba(74,144,226,0.10) 0%, transparent 70%);
      border-radius:50%;
      animation:pulse 8s ease-in-out infinite;
    }
    @keyframes pulse{
      0%,100%{transform:scale(1);opacity:0.5;}
      50%{transform:scale(1.1);opacity:0.8;}
    }
    .hero-content{
      max-width:1400px;
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:4rem;
      align-items:center;
      position:relative;
      z-index:1;
    }
    .hero-text h2{
      font-size:3.5rem;
      font-weight:900;
      line-height:1.1;
      margin-bottom:1.5rem;
      color:var(--dark-navy);
      letter-spacing:-1px;
    }
    .hero-text .highlight{
      background:var(--gradient-primary);
      -webkit-background-clip:text;
      background-clip:text;
      -webkit-text-fill-color:transparent;
      color:transparent;
    }
    .hero-text .tagline{
      font-size:1.5rem;
      color:var(--text-light);
      margin-bottom:2rem;
      font-weight:700;
    }
    .hero-text p{
      font-size:1.125rem;
      color:var(--text-light);
      margin-bottom:2.5rem;
      line-height:1.8;
    }
    .hero-buttons{
      display:flex;
      gap:1.5rem;
      flex-wrap:wrap;
    }
    .btn-primary{
      background:var(--gradient-primary);
      color:var(--white);
      padding:1rem 2.5rem;
      border-radius:999px;
      text-decoration:none;
      font-weight:900;
      font-size:1.125rem;
      transition:transform 0.3s ease, box-shadow 0.3s ease;
      box-shadow:0 6px 20px rgba(74,144,226,0.30);
      border:none;
      cursor:pointer;
      display:inline-block;
    }
    .btn-primary:hover{
      transform:translateY(-3px);
      box-shadow:0 8px 30px rgba(74,144,226,0.40);
    }
    .btn-secondary{
      background:var(--white);
      color:var(--primary-blue);
      padding:1rem 2.5rem;
      border-radius:999px;
      text-decoration:none;
      font-weight:900;
      font-size:1.125rem;
      border:2px solid var(--primary-blue);
      transition:all 0.3s ease;
      cursor:pointer;
      display:inline-block;
    }
    .btn-secondary:hover{
      background:var(--primary-blue);
      color:var(--white);
      transform:translateY(-3px);
    }

    .hero-visual{position:relative;perspective:1000px;}
    .floating-card{
      background:var(--white);
      border-radius:var(--radius-lg);
      padding:2rem;
      box-shadow:0 10px 40px rgba(0,0,0,0.10);
      margin-bottom:2rem;
      transition:transform 0.5s ease;
      transform-style:preserve-3d;
      will-change:transform;
    }
    .floating-card h3{
      font-size:1.25rem;
      color:var(--primary-blue);
      margin-bottom:0.5rem;
      font-weight:900;
    }
    .floating-card p{
      font-size:1rem;
      color:var(--text-light);
      margin:0;
    }

    /* Stats */
    .stats{
      background:var(--gradient-primary);
      padding:4rem 2rem;
      color:var(--white);
    }
    .stats-container{
      max-width:1400px;
      margin:0 auto;
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(250px, 1fr));
      gap:3rem;
      text-align:center;
    }
    .stat-item h3{
      font-size:3.5rem;
      font-weight:900;
      margin-bottom:0.5rem;
    }
    .stat-item p{
      font-size:1.125rem;
      opacity:0.95;
      font-weight:700;
    }

    /* Shared section */
    .section-title{
      text-align:center;
      margin-bottom:3rem;
    }
    .section-title h2{
      font-size:2.5rem;
      font-weight:900;
      color:var(--dark-navy);
      margin-bottom:1rem;
      letter-spacing:-0.6px;
    }
    .section-title p{
      font-size:1.25rem;
      color:var(--text-light);
      max-width:800px;
      margin:0 auto;
      font-weight:600;
    }

    /* Admin trap */
    .admin-trap{
      padding:6rem 2rem;
      background:var(--white);
    }
    .admin-trap-container{max-width:1400px;margin:0 auto;}
    .admin-trap-content{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:4rem;
      align-items:center;
      margin-top:4rem;
    }
    .trap-visual{
      background:linear-gradient(135deg, rgba(74,144,226,0.10) 0%, rgba(232,159,95,0.10) 100%);
      border-radius:var(--radius-lg);
      padding:3rem;
      position:relative;
      overflow:hidden;
    }
    .trap-visual .chart{
      width:100%;
      height:300px;
      position:relative;
    }
    .trap-points{
      display:flex;
      flex-direction:column;
      gap:2rem;
    }
    .trap-point{
      background:var(--light-bg);
      border-left:4px solid var(--primary-blue);
      padding:1.5rem;
      border-radius:var(--radius-sm);
      transition:transform 0.3s ease, box-shadow 0.3s ease;
    }
    .trap-point:hover{
      transform:translateX(10px);
      box-shadow:0 5px 20px rgba(0,0,0,0.10);
    }
    .trap-point h4{
      font-size:1.25rem;
      color:var(--primary-blue);
      margin-bottom:0.5rem;
      font-weight:900;
    }
    .trap-point p{
      color:var(--text-light);
      font-size:1rem;
      margin:0;
      font-weight:600;
    }

    /* Services */
    .services{
      padding:6rem 2rem;
      background:var(--light-bg);
    }
    .services-container{max-width:1400px;margin:0 auto;}
    .services-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(320px, 1fr));
      gap:2rem;
      margin-top:4rem;
    }
    .service-card{
      background:var(--white);
      border-radius:var(--radius-lg);
      padding:2.5rem;
      box-shadow:0 5px 30px rgba(0,0,0,0.08);
      transition:transform 0.3s ease, box-shadow 0.3s ease;
      position:relative;
      overflow:hidden;
    }
    .service-card::before{
      content:"";
      position:absolute;
      top:0;
      left:0;
      width:100%;
      height:4px;
      background:var(--gradient-primary);
      transform:scaleX(0);
      transition:transform 0.3s ease;
      transform-origin:left;
    }
    .service-card:hover{
      transform:translateY(-10px);
      box-shadow:0 15px 50px rgba(0,0,0,0.15);
    }
    .service-card:hover::before{transform:scaleX(1);}
    .service-icon{
      font-size:3rem;
      margin-bottom:1.5rem;
      line-height:1;
      color:var(--primary-blue);
    }
    .service-card h3{
      font-size:1.5rem;
      color:var(--dark-navy);
      margin-bottom:1rem;
      font-weight:900;
    }
    .service-card p{
      color:var(--text-light);
      font-size:1rem;
      margin-bottom:1.5rem;
      line-height:1.7;
      font-weight:600;
    }
    .service-card ul{
      list-style:none;
      margin-top:1rem;
    }
    .service-card ul li{
      padding:0.5rem 0;
      color:var(--text-light);
      font-size:0.9375rem;
      position:relative;
      padding-left:1.5rem;
      font-weight:650;
    }
    .service-card ul li::before{
      content:"•";
      position:absolute;
      left:0;
      color:var(--primary-blue);
      font-weight:900;
    }

    /* Models */
    .models{
      padding:6rem 2rem;
      background:var(--white);
    }
    .models-container{max-width:1400px;margin:0 auto;}
    .models-tabs{
      display:flex;
      justify-content:center;
      gap:2rem;
      margin-top:3rem;
      margin-bottom:3rem;
      flex-wrap:wrap;
    }
    .tab-button{
      background:var(--light-bg);
      color:var(--text-dark);
      padding:1rem 2.5rem;
      border-radius:999px;
      border:2px solid transparent;
      font-weight:900;
      font-size:1.125rem;
      cursor:pointer;
      transition:all 0.3s ease;
    }
    .tab-button.active{
      background:var(--gradient-primary);
      color:var(--white);
      box-shadow:0 6px 20px rgba(74,144,226,0.30);
    }
    .tab-content{display:none;}
    .tab-content.active{
      display:block;
      animation:fadeIn 0.5s ease;
    }
    @keyframes fadeIn{
      from{opacity:0;transform:translateY(20px);}
      to{opacity:1;transform:translateY(0);}
    }
    .model-content{
      background:linear-gradient(135deg, rgba(74,144,226,0.05) 0%, rgba(232,159,95,0.05) 100%);
      border-radius:var(--radius-lg);
      padding:3rem;
    }
    .model-flow{
      display:flex;
      justify-content:space-between;
      align-items:center;
      margin:3rem 0;
      flex-wrap:wrap;
      gap:1rem;
    }
    .flow-step{
      background:var(--white);
      border-radius:var(--radius-md);
      padding:1.5rem;
      text-align:center;
      flex:1;
      min-width:150px;
      box-shadow:var(--shadow-sm);
      position:relative;
    }
    .flow-step::after{
      content:"→";
      position:absolute;
      right:-1.5rem;
      top:50%;
      transform:translateY(-50%);
      font-size:2rem;
      color:var(--primary-blue);
      font-weight:900;
    }
    .flow-step:last-child::after{display:none;}
    .flow-step h4{
      font-size:1.125rem;
      color:var(--primary-blue);
      margin-bottom:0.5rem;
      font-weight:900;
    }
    .flow-step p{
      font-size:0.9375rem;
      color:var(--text-light);
      margin:0;
      font-weight:650;
    }
    .model-features{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(280px, 1fr));
      gap:2rem;
      margin-top:3rem;
    }
    .feature-box{
      background:var(--white);
      border-radius:var(--radius-md);
      padding:2rem;
      box-shadow:var(--shadow-sm);
    }
    .feature-box h4{
      font-size:1.25rem;
      color:var(--dark-navy);
      margin-bottom:1rem;
      font-weight:900;
    }
    .feature-box ul{list-style:none;}
    .feature-box ul li{
      padding:0.5rem 0;
      color:var(--text-light);
      position:relative;
      padding-left:1.5rem;
      font-weight:650;
    }
    .feature-box ul li::before{
      content:"•";
      position:absolute;
      left:0;
      color:var(--primary-blue);
      font-size:1.5rem;
      line-height:1;
      font-weight:900;
    }

    /* Recruitment */
    .recruitment{
      padding:6rem 2rem;
      background:var(--gradient-primary);
      color:var(--white);
    }
    .recruitment-container{max-width:1400px;margin:0 auto;}
    .recruitment-content{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:4rem;
      align-items:center;
      margin-top:3rem;
    }
    .pricing-comparison{
      background:rgba(255,255,255,0.15);
      backdrop-filter:blur(10px);
      border-radius:var(--radius-lg);
      padding:3rem;
    }
    .pricing-comparison h3{
      font-size:2rem;
      margin-bottom:2rem;
      font-weight:900;
    }
    .comparison-item{
      display:flex;
      justify-content:space-between;
      padding:1rem 0;
      border-bottom:1px solid rgba(255,255,255,0.20);
      gap:1rem;
    }
    .comparison-item:last-child{border-bottom:none;}
    .comparison-item span:first-child{font-weight:700;}
    .comparison-item span:last-child{font-weight:900;font-size:1.25rem;}
    .recruitment-benefits{
      display:flex;
      flex-direction:column;
      gap:2rem;
    }
    .benefit-item{
      background:rgba(255,255,255,0.15);
      backdrop-filter:blur(10px);
      border-radius:var(--radius-md);
      padding:2rem;
    }
    .benefit-item h4{
      font-size:1.5rem;
      margin-bottom:1rem;
      font-weight:900;
    }
    .benefit-item p{
      font-size:1rem;
      line-height:1.7;
      opacity:0.95;
      margin:0;
      font-weight:650;
    }

    /* Case studies */
    .case-studies{
      padding:6rem 2rem;
      background:var(--light-bg);
    }
    .case-studies-container{max-width:1400px;margin:0 auto;}
    .case-study-card{
      background:var(--white);
      border-radius:var(--radius-lg);
      padding:3rem;
      margin-top:3rem;
      box-shadow:var(--shadow-md);
    }
    .case-study-header{
      display:flex;
      justify-content:space-between;
      align-items:flex-start;
      margin-bottom:2rem;
      flex-wrap:wrap;
      gap:2rem;
    }
    .case-study-info h3{
      font-size:1.75rem;
      color:var(--dark-navy);
      margin-bottom:0.5rem;
      font-weight:900;
    }
    .case-study-info p{
      color:var(--text-light);
      font-size:1rem;
      margin:0;
      font-weight:650;
    }
    .case-study-metrics{
      display:flex;
      gap:2rem;
      flex-wrap:wrap;
    }
    .metric{text-align:center;min-width:120px;}
    .metric h4{
      font-size:2rem;
      color:var(--primary-blue);
      font-weight:900;
      margin:0;
    }
    .metric p{
      font-size:0.875rem;
      color:var(--text-light);
      margin:0;
      font-weight:650;
    }
    .case-study-body{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:2rem;
      margin-top:2rem;
    }
    .challenge, .solution{
      padding:1.5rem;
      background:var(--light-bg);
      border-radius:var(--radius-md);
    }
    .challenge h4, .solution h4{
      color:var(--primary-blue);
      margin-bottom:1rem;
      font-size:1.25rem;
      font-weight:900;
    }
    .challenge p, .solution p{
      color:var(--text-light);
      line-height:1.7;
      margin:0;
      font-weight:650;
    }

    /* Contact */
    .contact{
      padding:6rem 2rem;
      background:var(--white);
    }
    .contact-container{
      max-width:1400px;
      margin:0 auto;
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:4rem;
      align-items:start;
    }
    .contact-info h3{
      font-size:2rem;
      color:var(--dark-navy);
      margin-bottom:1rem;
      font-weight:900;
    }
    .contact-info p{
      color:var(--text-light);
      font-size:1.125rem;
      margin-bottom:2rem;
      line-height:1.7;
      font-weight:650;
    }
    .contact-details{
      display:flex;
      flex-direction:column;
      gap:1.5rem;
      margin-top:2rem;
    }
    .contact-item{
      display:flex;
      align-items:center;
      gap:1rem;
    }
    .contact-icon{
      width:50px;
      height:50px;
      background:var(--gradient-primary);
      border-radius:50%;
      display:flex;
      align-items:center;
      justify-content:center;
      color:var(--white);
      font-size:1.25rem;
      font-weight:900;
      flex-shrink:0;
    }
    .contact-item-text h4{
      font-size:1rem;
      color:var(--dark-navy);
      margin-bottom:0.25rem;
      font-weight:900;
    }
    .contact-item-text p{
      font-size:1rem;
      color:var(--text-light);
      margin:0;
      font-weight:650;
      word-break:break-word;
    }

    .contact-form{
      background:var(--light-bg);
      padding:3rem;
      border-radius:var(--radius-lg);
    }
    .form-group{margin-bottom:1.5rem;}
    .form-group label{
      display:block;
      font-weight:900;
      margin-bottom:0.5rem;
      color:var(--dark-navy);
      font-size:1rem;
    }
    .form-group input,
    .form-group textarea,
    .form-group select{
      width:100%;
      padding:1rem;
      border:2px solid #E2E8F0;
      border-radius:10px;
      font-size:1rem;
      font-family:inherit;
      transition:border-color 0.3s ease;
      background:var(--white);
      color:var(--text-dark);
    }
    .form-group input:focus,
    .form-group textarea:focus,
    .form-group select:focus{
      outline:none;
      border-color:var(--primary-blue);
    }
    .form-group textarea{resize:vertical;min-height:120px;}
    .submit-btn{
      background:var(--gradient-primary);
      color:var(--white);
      padding:1rem 3rem;
      border-radius:999px;
      border:none;
      font-weight:900;
      font-size:1.125rem;
      cursor:pointer;
      transition:transform 0.3s ease, box-shadow 0.3s ease;
      box-shadow:0 6px 20px rgba(74,144,226,0.30);
      width:100%;
    }
    .submit-btn:hover{
      transform:translateY(-3px);
      box-shadow:0 8px 30px rgba(74,144,226,0.40);
    }

    /* Footer */
    footer{
      background:var(--dark-navy);
      color:var(--white);
      padding:4rem 2rem 2rem;
    }
    .footer-container{
      max-width:1400px;
      margin:0 auto;
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(250px, 1fr));
      gap:3rem;
      margin-bottom:3rem;
    }
    .footer-section h4{
      font-size:1.25rem;
      margin-bottom:1.5rem;
      font-weight:900;
    }
    .footer-section p{
      opacity:0.85;
      line-height:1.7;
      font-size:0.9375rem;
      margin:0.5rem 0;
      font-weight:650;
    }
    .footer-links{
      list-style:none;
      padding:0;
      margin:0;
    }
    .footer-links li{margin-bottom:0.75rem;}
    .footer-links a{
      color:var(--white);
      text-decoration:none;
      opacity:0.85;
      transition:opacity 0.3s ease;
      font-size:0.9375rem;
      font-weight:750;
    }
    .footer-links a:hover{opacity:1;}
    .footer-bottom{
      border-top:1px solid rgba(255,255,255,0.10);
      padding-top:2rem;
      text-align:center;
      opacity:0.75;
      font-size:0.875rem;
      font-weight:650;
    }

    /* Scroll animations */
    .fade-in{
      opacity:0;
      transform:translateY(30px);
      transition:opacity 0.6s ease, transform 0.6s ease;
    }
    .fade-in.visible{
      opacity:1;
      transform:translateY(0);
    }

    /* Extra animations */
    @keyframes rotate{
      from{transform:rotate(0deg);}
      to{transform:rotate(360deg);}
    }
    @keyframes logoFloat{
      0%,100%{transform:translateY(0px);}
      50%{transform:translateY(-15px);}
    }
    .logo:hover{animation:rotate 1s ease-in-out;}

    /* Responsive */
    @media (max-width:968px){
      .nav-links{display:none;}
      .mobile-menu{display:flex;}
      .hero-content,
      .admin-trap-content,
      .recruitment-content,
      .contact-container,
      .case-study-body{
        grid-template-columns:1fr;
      }
      .hero-text h2{font-size:2.5rem;}
      .hero-text .tagline{font-size:1.25rem;}
      .section-title h2{font-size:2rem;}
      .flow-step::after{display:none;}
      .model-flow{flex-direction:column;}
      .slide-content{
        grid-template-columns:1fr;
        gap:2rem;
        padding:2rem;
        min-height:auto;
      }
      .slide-graphic{padding:1rem;}
      .slide-text h2{font-size:2rem;}
      .how-point{flex-direction:column;align-items:center;text-align:center;}
      .bar-label{min-width:120px;font-size:0.875rem;}
      .recruitment-benefits-quick{flex-direction:column;gap:1rem;}
      .nav-mobile-panel{display:block;}
      .nav-mobile-panel:not(.open) .nav-mobile-links{display:none;}
    }
    @media (max-width:640px){
      .hero-text h2{font-size:2rem;}
      .stat-item h3{font-size:2.5rem;}
      .services-grid,
      .model-features{
        grid-template-columns:1fr;
      }
      .core-values{padding:1rem 0 0.5rem;}
      .slide-content{padding:1.5rem;}
      .slide-text h2{font-size:1.75rem;}
      .pricing-bar{flex-direction:column;align-items:flex-start;gap:0.5rem;}
      .bar-label{min-width:auto;}
      .slide-controls{padding:1rem;}
      .nav-container{padding:0.75rem 1rem;}
      .nav-mobile-panel{padding:0 1rem 1rem;}
    }
  </style>
</head>

<body>
  <!-- Navigation -->
  <nav id="navbar" aria-label="Primary">
    <div class="nav-container">
      <div class="logo-container">
        <img
          src="https://agi-prod-file-upload-public-main-use1.s3.amazonaws.com/4f9e60f6-2d9e-475f-b0f1-cf9f812f2d26"
          alt="Otocinclus Logo"
          class="logo"
        />
        <div class="logo-text">
          <h1>OTOCINCLUS</h1>
          <p>TECHNOLOGY</p>
        </div>
      </div>

      <ul class="nav-links" id="navLinksDesktop">
        <li><a href="#home">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#models">Engagement Models</a></li>
        <li><a href="#recruitment">Recruitment</a></li>
        <li><a href="#case-studies">Case Studies</a></li>
        <li><a href="#contact" class="cta-button">Get Started</a></li>
      </ul>

      <button class="mobile-menu" id="mobileMenuButton" type="button" aria-label="Open menu" aria-expanded="false" aria-controls="mobileNavPanel">
        <span></span><span></span><span></span>
      </button>
    </div>

    <div class="nav-mobile-panel" id="mobileNavPanel">
      <ul class="nav-mobile-links" id="navLinksMobile">
        <li><a href="#home">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#models">Engagement Models</a></li>
        <li><a href="#recruitment">Recruitment</a></li>
        <li><a href="#case-studies">Case Studies</a></li>
        <li><a href="#contact" class="cta-button">Get Started</a></li>
      </ul>
    </div>
  </nav>

  <!-- Core Value Propositions - Slideshow -->
  <section class="core-values" aria-label="Core value propositions slideshow">
    <div class="core-values-container">
      <div class="slideshow-wrapper">
        <div class="slide active" data-slide="0">
          <div class="slide-content">
            <div class="slide-graphic">
              <img
                src="https://agi-prod-file-upload-public-main-use1.s3.amazonaws.com/4f9e60f6-2d9e-475f-b0f1-cf9f812f2d26"
                alt="Otocinclus Logo - Admin Trap Solution"
                style="width:100%;max-width:280px;height:auto;animation:logoFloat 3s ease-in-out infinite;"
              />
            </div>
            <div class="slide-text">
              <h2>We Remove the <span class="highlight-orange">Admin Trap</span></h2>
              <p class="subtitle">How We Free Your Business from HR Chaos</p>

              <div class="how-points">
                <div class="how-point">
                  <div class="point-icon">✓</div>
                  <div class="point-text">
                    <h4>Complete HR Infrastructure Setup</h4>
                    <p>We build professional HR policies, HRMS systems, and compliance frameworks from scratch</p>
                  </div>
                </div>

                <div class="how-point">
                  <div class="point-icon">✓</div>
                  <div class="point-text">
                    <h4>End-to-End Operations</h4>
                    <p>Monthly payroll, statutory compliance, attendance tracking - we handle everything</p>
                  </div>
                </div>

                <div class="how-point">
                  <div class="point-icon">✓</div>
                  <div class="point-text">
                    <h4>Zero Compliance Risk</h4>
                    <p>Professional indemnity coverage, maker-checker systems, automated compliance calendars</p>
                  </div>
                </div>

                <div class="how-point">
                  <div class="point-icon">✓</div>
                  <div class="point-text">
                    <h4>Build-Operate-Transfer Model</h4>
                    <p>We build it, run it flawlessly, then transfer complete ownership when you're ready</p>
                  </div>
                </div>
              </div>

              <div class="slide-cta">
                <a href="#admin-trap" class="btn-slide">Learn More</a>
              </div>
            </div>
          </div>
        </div>

        <div class="slide" data-slide="1">
          <div class="slide-content">
            <div class="slide-graphic">
              <img
                src="https://agi-prod-file-upload-public-main-use1.s3.amazonaws.com/4f9e60f6-2d9e-475f-b0f1-cf9f812f2d26"
                alt="Otocinclus Logo - Flat 7 Recruitment"
                style="width:100%;max-width:280px;height:auto;animation:logoFloat 3s ease-in-out infinite;"
              />
            </div>

            <div class="slide-text">
              <h2><span class="highlight-orange">Flat 7 Recruitment</span> - All Levels</h2>
              <p class="subtitle">Industry-Disrupting Pricing That Saves You Massive Costs</p>

              <div class="pricing-showcase" aria-label="Pricing showcase bars">
                <div class="pricing-bar">
                  <div class="bar-label">Traditional - Junior</div>
                  <div class="bar-container" aria-hidden="true">
                    <div class="bar traditional" style="width:42%;">
                      <span class="bar-value">8.33%</span>
                    </div>
                  </div>
                </div>

                <div class="pricing-bar">
                  <div class="bar-label">Traditional - Mid</div>
                  <div class="bar-container" aria-hidden="true">
                    <div class="bar traditional" style="width:65%;">
                      <span class="bar-value">12-15%</span>
                    </div>
                  </div>
                </div>

                <div class="pricing-bar">
                  <div class="bar-label">Traditional - Senior</div>
                  <div class="bar-container" aria-hidden="true">
                    <div class="bar traditional" style="width:100%;">
                      <span class="bar-value">20%</span>
                    </div>
                  </div>
                </div>

                <div class="pricing-bar highlight-bar">
                  <div class="bar-label"><strong>Otocinclus - ALL Levels</strong></div>
                  <div class="bar-container" aria-hidden="true">
                    <div class="bar otocinclus" style="width:35%;">
                      <span class="bar-value">7% FLAT</span>
                    </div>
                  </div>
                </div>
              </div>

              <div class="recruitment-benefits-quick" aria-label="Recruitment benefits quick list">
                <div class="benefit-quick"><span class="benefit-icon">★</span><span>30-65% savings on senior hires</span></div>
                <div class="benefit-quick"><span class="benefit-icon">★</span><span>28 days avg. time-to-hire</span></div>
                <div class="benefit-quick"><span class="benefit-icon">★</span><span>90-day free replacement</span></div>
              </div>

              <div class="slide-cta">
                <a href="#recruitment" class="btn-slide">View Full Details</a>
              </div>
            </div>
          </div>
        </div>

        <!-- Slideshow Controls -->
        <div class="slide-controls" aria-label="Slideshow controls">
          <button class="slide-control prev" type="button" id="slidePrev" aria-label="Previous slide">‹</button>
          <div class="slide-dots" role="tablist" aria-label="Slide dots">
            <span class="dot active" role="tab" aria-selected="true" tabindex="0" data-dot="0"></span>
            <span class="dot" role="tab" aria-selected="false" tabindex="0" data-dot="1"></span>
          </div>
          <button class="slide-control next" type="button" id="slideNext" aria-label="Next slide">›</button>
        </div>
      </div>
    </div>
  </section>

  <!-- Hero Section -->
  <section id="home" class="hero" aria-label="Hero">
    <div class="hero-content">
      <div class="hero-text">
        <h2>We Remove the <span class="highlight">Admin Trap</span></h2>
        <p class="tagline">Audit. Advise. Implement. Transfer.</p>
        <p>
          Otocinclus is your <strong>HR Consultancy &amp; HRMS Implementation Partner</strong> delivering integrated HR infrastructure for India's growing businesses.
          We build professional HR systems, operate them flawlessly, and transfer them to your team when you're ready.
        </p>
        <div class="hero-buttons">
          <a href="#contact" class="btn-primary">Schedule Consultation</a>
          <a href="#services" class="btn-secondary">Explore Services</a>
        </div>
      </div>

      <div class="hero-visual" aria-label="Hero highlights">
        <div class="floating-card">
          <h3>Build-Operate-Transfer Model</h3>
          <p>We build your HR infrastructure, operate it seamlessly, and transfer complete ownership when ready.</p>
        </div>
        <div class="floating-card">
          <h3>Vendor-Agnostic HRMS Implementation</h3>
          <p>Expert implementation of Keka, GreytHR, Zoho, Darwinbox - we help you choose and deploy the right fit.</p>
        </div>
        <div class="floating-card">
          <h3>Flat 7 Recruitment - All Levels</h3>
          <p>Industry-disrupting recruitment pricing. Save 30-65% on senior hires compared to traditional agencies.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Stats Section -->
  <section class="stats" aria-label="Key stats">
    <div class="stats-container">
      <div class="stat-item">
        <h3 data-suffix="%">30-65</h3>
        <p>Cost Savings vs. Traditional Agencies</p>
      </div>
      <div class="stat-item">
        <h3 data-suffix=" Hours">20 Hours</h3>
        <p>Founder Bandwidth Reclaimed Monthly</p>
      </div>
      <div class="stat-item">
        <h3 data-suffix=" Days">28 Days</h3>
        <p>Reduced Time-to-Hire</p>
      </div>
      <div class="stat-item">
        <h3 data-suffix="%">99.5</h3>
        <p>Payroll Accuracy Target</p>
      </div>
    </div>
  </section>

  <!-- Admin Trap Section -->
  <section id="admin-trap" class="admin-trap" aria-label="Admin trap">
    <div class="admin-trap-container">
      <div class="section-title">
        <h2>The Admin Trap Where Growth Stalls</h2>
        <p>Growing businesses between 15-100 employees face a critical inflection point. Too large for spreadsheets. Too small for a VP of HR. Too risky to ignore.</p>
      </div>

      <div class="admin-trap-content">
        <div class="trap-visual" aria-label="Admin trap visual">
          <div class="chart" aria-hidden="true">
            <svg viewBox="0 0 400 300" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Administrative complexity chart">
              <text x="10" y="20" font-size="14" fill="#626C71">Administrative Complexity</text>
              <path d="M 50 250 L 50 50 L 350 50" stroke="#626C71" stroke-width="2" fill="none"></path>
              <path d="M 50 250 Q 100 240, 150 180 T 250 80 T 350 60" stroke="#4A90E2" stroke-width="4" fill="none"></path>
              <circle cx="150" cy="180" r="6" fill="#E89F5F"></circle>
              <text x="140" y="210" font-size="12" fill="#E89F5F" font-weight="700">The Admin Trap</text>
              <text x="130" y="225" font-size="11" fill="#626C71">15-100 employees</text>
              <text x="10" y="280" font-size="12" fill="#626C71">Employee Count</text>
            </svg>
          </div>
        </div>

        <div class="trap-points">
          <div class="trap-point">
            <h4>Time Drain</h4>
            <p>Founders and CXOs spend 15-25 hours per week on HR administration - that's 25% of strategic capacity lost.</p>
          </div>
          <div class="trap-point">
            <h4>Compliance Risk</h4>
            <p>New Social Security Code penalties include imprisonment and substantial fines. Ignorance is not protection.</p>
          </div>
          <div class="trap-point">
            <h4>Financial Loss</h4>
            <p>30-40% higher effective HR costs due to hidden burdens like errors, delays, and opportunity costs.</p>
          </div>
          <div class="trap-point">
            <h4>Strategic Impact</h4>
            <p>Poor HR infrastructure blocks investor readiness, damages employer branding, and limits growth velocity.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section id="services" class="services" aria-label="Services">
    <div class="services-container">
      <div class="section-title">
        <h2>Comprehensive HR Infrastructure Services</h2>
        <p>Full-stack HR solutions designed for growing businesses. We handle everything so you can focus on growth.</p>
      </div>

      <div class="services-grid">
        <div class="service-card fade-in">
          <div class="service-icon">⚙</div>
          <h3>HR Governance &amp; Policy Design</h3>
          <p>Build compliant, scalable HR foundations with professionally designed policies and organizational frameworks.</p>
          <ul>
            <li>HR policy &amp; employee handbook</li>
            <li>Organizational structure &amp; role definitions</li>
            <li>HR process mapping and SOPs</li>
            <li>Compliance framework: PF, ESI, PT, labour laws</li>
          </ul>
        </div>

        <div class="service-card fade-in">
          <div class="service-icon">🧩</div>
          <h3>HRMS Selection, Implementation &amp; Administration</h3>
          <p>Vendor-agnostic HRMS implementation expertise. We help you select, configure, and operate the right system.</p>
          <ul>
            <li>HRMS selection &amp; fitment advisory</li>
            <li>Complete configuration: payroll, attendance, leave</li>
            <li>Data migration from legacy systems</li>
            <li>Ongoing HRMS administration &amp; support</li>
            <li>HRMS training for internal teams</li>
          </ul>
        </div>

        <div class="service-card fade-in">
          <div class="service-icon">🧾</div>
          <h3>Payroll &amp; Statutory Compliance</h3>
          <p>Accurate, timely payroll processing with zero compliance risk. Your compliance shield.</p>
          <ul>
            <li>Monthly payroll processing &amp; payslips</li>
            <li>Statutory deductions &amp; filings: PF, ESI, PT, TDS</li>
            <li>Statutory returns &amp; challans</li>
            <li>Full &amp; final settlements</li>
            <li>Payroll MIS &amp; analytics reports</li>
          </ul>
        </div>

        <div class="service-card fade-in">
          <div class="service-icon">⏱</div>
          <h3>Attendance, Leave &amp; Time Management</h3>
          <p>Automated attendance tracking with intelligent shift and leave management systems.</p>
          <ul>
            <li>Shift rules and attendance logic design</li>
            <li>Leave policy design, setup, and tracking</li>
            <li>Monthly attendance reconciliation</li>
            <li>Attendance and leave dashboards</li>
          </ul>
        </div>

        <div class="service-card fade-in">
          <div class="service-icon">👥</div>
          <h3>Employee Lifecycle Management</h3>
          <p>Seamless employee journey management from onboarding to exit with complete documentation.</p>
          <ul>
            <li>End-to-end onboarding documentation, KYC</li>
            <li>Employee records management: digital files</li>
            <li>Confirmation &amp; probation tracking</li>
            <li>Appraisal cycle coordination support</li>
            <li>Exit management, NOC, and F&amp;F settlements</li>
          </ul>
        </div>

        <div class="service-card fade-in">
          <div class="service-icon">🎯</div>
          <h3>Recruitment Services Flat 7 - All Levels</h3>
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

        <div class="service-card fade-in">
          <div class="service-icon">📚</div>
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
  <section id="models" class="models" aria-label="Engagement models">
    <div class="models-container">
      <div class="section-title">
        <h2>Engagement Models Designed for Your Journey</h2>
        <p>Choose the model that matches your growth stage and internal capabilities.</p>
      </div>

      <div class="models-tabs" role="tablist" aria-label="Engagement model tabs">
        <button class="tab-button active" type="button" data-model="model1" aria-controls="model1" aria-selected="true">Model 1 Managed HR Services</button>
        <button class="tab-button" type="button" data-model="model2" aria-controls="model2" aria-selected="false">Model 2 Build-Operate-Transfer</button>
      </div>

      <div id="model1" class="tab-content active" role="tabpanel" aria-label="Model 1 Managed HR Services">
        <div class="model-content">
          <h3 style="font-size:2rem;color:var(--dark-navy);margin-bottom:1rem;font-weight:900;">Complete Outsourced HR Services - Managed HR</h3>
          <p style="font-size:1.125rem;color:var(--text-light);margin-bottom:2rem;font-weight:650;">Best for companies who want us to handle everything. We act as your extended HR department.</p>

          <div class="model-flow" aria-label="Model 1 flow">
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

          <div class="model-features" aria-label="Model 1 features">
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

          <div style="background:var(--white);padding:2rem;border-radius:15px;margin-top:3rem;text-align:center;">
            <h4 style="font-size:1.5rem;color:var(--primary-blue);margin-bottom:1rem;font-weight:900;">Outcome</h4>
            <p style="font-size:1.125rem;color:var(--text-light);margin:0;font-weight:650;">
              Get a fully functional HR department without hiring an internal HR team. Per-employee monthly subscription model provides predictable costs and enterprise-grade HR infrastructure.
            </p>
          </div>
        </div>
      </div>

      <div id="model2" class="tab-content" role="tabpanel" aria-label="Model 2 Build-Operate-Transfer">
        <div class="model-content">
          <h3 style="font-size:2rem;color:var(--dark-navy);margin-bottom:1rem;font-weight:900;">HR Setup + Transition to Client HR Team</h3>
          <p style="font-size:1.125rem;color:var(--text-light);margin-bottom:2rem;font-weight:650;">Best for companies planning to build an internal HR team. We set up, stabilize, then hand over.</p>

          <div class="model-flow" aria-label="Model 2 flow">
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

          <div class="model-features" aria-label="Model 2 features">
            <div class="feature-box">
              <h4>Phase 1 HR Setup &amp; HRMS Implementation</h4>
              <ul>
                <li>HR policy &amp; handbook creation</li>
                <li>Compliance &amp; statutory setup</li>
                <li>HRMS implementation</li>
                <li>Payroll, attendance &amp; leave setup</li>
                <li>Employee data migration</li>
                <li>Process documentation: SOPs</li>
              </ul>
            </div>

            <div class="feature-box">
              <h4>Phase 2 Initial Operations (2-3 Months)</h4>
              <ul>
                <li>Payroll processing &amp; compliance filings</li>
                <li>Attendance &amp; leave administration</li>
                <li>Employee lifecycle support</li>
                <li>HRMS monitoring &amp; fine-tuning</li>
                <li>Issue resolution &amp; stabilization</li>
              </ul>
            </div>

            <div class="feature-box">
              <h4>Phase 3 Training &amp; Handover</h4>
              <ul>
                <li>HRMS training for internal HR</li>
                <li>Payroll &amp; compliance training</li>
                <li>Process walkthroughs &amp; SOP handover</li>
                <li>Knowledge transfer sessions</li>
                <li>Post-handover support as required</li>
              </ul>
            </div>
          </div>

          <div style="background:var(--white);padding:2rem;border-radius:15px;margin-top:3rem;text-align:center;">
            <h4 style="font-size:1.5rem;color:var(--primary-blue);margin-bottom:1rem;font-weight:900;">Outcome</h4>
            <p style="font-size:1.125rem;color:var(--text-light);margin:0;font-weight:650;">
              Your internal HR team inherits a professionally built, fully operational HR system with complete documentation, training, and post-handover support. You own the function.
            </p>
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- Recruitment Section -->
  <section id="recruitment" class="recruitment" aria-label="Recruitment">
    <div class="recruitment-container">
      <div class="section-title" style="color:var(--white);">
        <h2 style="color:var(--white);">Recruitment Services Flat 7 - All Levels</h2>
        <p style="color:rgba(255,255,255,0.95);">We eliminate the "Leadership Penalty" charged by traditional agencies. Same quality, transparent pricing across all levels. <strong>Charged separately at affordable rates below market standard.</strong></p>
      </div>

      <div class="recruitment-content">
        <div class="pricing-comparison fade-in">
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
            <span>20%</span>
          </div>

          <div class="comparison-item" style="border-top:2px solid rgba(255,255,255,0.40);padding-top:1.5rem;margin-top:1.5rem;border-bottom:none;">
            <span style="font-size:1.5rem;font-weight:900;">Otocinclus - All Levels</span>
            <span style="font-size:1.75rem;color:var(--accent-orange);font-weight:900;">7%</span>
          </div>
        </div>

        <div class="recruitment-benefits">
          <div class="benefit-item fade-in">
            <h4>30-65% Savings on Senior Hires</h4>
            <p>Traditional agencies charge 20%+ for leadership roles. We charge flat 7% regardless of seniority, saving you massive costs on critical hires.</p>
          </div>
          <div class="benefit-item fade-in">
            <h4>Comprehensive Recruitment Support</h4>
            <p>Includes sourcing, screening, interview coordination, offer negotiation, joining coordination, and 90-day free replacement guarantee.</p>
          </div>
          <div class="benefit-item fade-in">
            <h4>Faster Turnaround</h4>
            <p>28 days average time-to-hire (down from industry standard 45 days). Integration with our HR &amp; payroll operations enables seamless onboarding.</p>
          </div>
          <div class="benefit-item fade-in">
            <h4>Continued Support Post-HR Handover</h4>
            <p>Recruitment services can continue even after HR handover in Model 2, providing long-term talent acquisition support.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Case Studies Section -->
  <section id="case-studies" class="case-studies" aria-label="Case studies">
    <div class="case-studies-container">
      <div class="section-title">
        <h2>Success Stories - Real Impact, Real Results</h2>
        <p>See how we've helped growing businesses break free from the Admin Trap and scale confidently.</p>
      </div>

      <article class="case-study-card fade-in" aria-label="Case study 1">
        <div class="case-study-header">
          <div class="case-study-info">
            <h3>SaaS Startup - 45 Employees</h3>
            <p>Industry: B2B SaaS | Challenge: Scaling from 15 to 45 employees in 8 months</p>
          </div>
          <div class="case-study-metrics" aria-label="Case study metrics">
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
      </article>

      <article class="case-study-card fade-in" aria-label="Case study 2">
        <div class="case-study-header">
          <div class="case-study-info">
            <h3>Manufacturing Company - 80 Employees</h3>
            <p>Industry: Manufacturing | Challenge: Transition to internal HR team</p>
          </div>
          <div class="case-study-metrics" aria-label="Case study metrics">
            <div class="metric">
              <h4>6 Month</h4>
              <p>Complete Handover</p>
            </div>
            <div class="metric">
              <h4>52%</h4>
              <p>Cost Savings vs Agency</p>
            </div>
            <div class="metric">
              <h4>3 Month</h4>
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
      </article>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact" aria-label="Contact">
    <div class="contact-container">
      <div class="contact-info">
        <h3>Ready to Remove the Admin Trap?</h3>
        <p>Schedule a free HR infrastructure audit. We'll analyze your current state, identify risks, and recommend the right engagement model for your business.</p>

        <div class="contact-details" aria-label="Contact details">
          <div class="contact-item">
            <div class="contact-icon" aria-hidden="true">⌁</div>
            <div class="contact-item-text">
              <h4>Location</h4>
              <p>Bengaluru, Karnataka, India</p>
            </div>
          </div>

          <div class="contact-item">
            <div class="contact-icon" aria-hidden="true">@</div>
            <div class="contact-item-text">
              <h4>Email</h4>
              <p>contact@otocinclus.com</p>
            </div>
          </div>

          <div class="contact-item">
            <div class="contact-icon" aria-hidden="true">☎</div>
            <div class="contact-item-text">
              <h4>Phone</h4>
              <p>+91 XXXXX XXXXX</p>
            </div>
          </div>
        </div>
      </div>

      <div class="contact-form" aria-label="Contact form">
        <form id="contactForm" novalidate>
          <div class="form-group">
            <label for="name">Full Name</label>
            <input type="text" id="name" name="name" required />
          </div>

          <div class="form-group">
            <label for="email">Email Address</label>
            <input type="email" id="email" name="email" required />
          </div>

          <div class="form-group">
            <label for="phone">Phone Number</label>
            <input type="tel" id="phone" name="phone" required />
          </div>

          <div class="form-group">
            <label for="company">Company Name</label>
            <input type="text" id="company" name="company" required />
          </div>

          <div class="form-group">
            <label for="employees">Number of Employees</label>
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
            <label for="interest">Service Interest</label>
            <select id="interest" name="interest" required>
              <option value="">Select service</option>
              <option value="model1">Model 1 Managed HR Services</option>
              <option value="model2">Model 2 Build-Operate-Transfer</option>
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
  <footer aria-label="Footer">
    <div class="footer-container">
      <div class="footer-section">
        <h4>Otocinclus Technology</h4>
        <p>The integrated HR infrastructure layer enabling India's SME growth engine. We audit, advise, implement, and transfer.</p>
        <p style="margin-top:1rem;"><strong>Mission</strong> To ensure no business fails due to administrative burden or compliance ignorance.</p>
      </div>

      <div class="footer-section">
        <h4>Services</h4>
        <ul class="footer-links">
          <li><a href="#services">HR Governance &amp; Policy Design</a></li>
          <li><a href="#services">HRMS Implementation</a></li>
          <li><a href="#services">Payroll &amp; Compliance</a></li>
          <li><a href="#services">Recruitment Services 7%</a></li>
          <li><a href="#services">Employee Lifecycle Management</a></li>
        </ul>
      </div>

      <div class="footer-section">
        <h4>Engagement Models</h4>
        <ul class="footer-links">
          <li><a href="#models">Model 1 Managed HR Services</a></li>
          <li><a href="#models">Model 2 Build-Operate-Transfer</a></li>
          <li><a href="#recruitment">Flat 7 Recruitment</a></li>
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
      <p>© 2026 Otocinclus Technology. All rights reserved. HR Consultancy &amp; HRMS Implementation Partner | Bengaluru, Karnataka</p>
    </div>
  </footer>

  <script defer>
    (function () {
      function ready(fn) {
        if (document.readyState === "loading") {
          document.addEventListener("DOMContentLoaded", fn, { once: true });
        } else {
          fn();
        }
      }

      ready(function () {
        // Navbar scroll effect
        var navbar = document.getElementById("navbar");
        function onScroll() {
          if (!navbar) return;
          if (window.scrollY > 50) {
            navbar.classList.add("scrolled");
          } else {
            navbar.classList.remove("scrolled");
          }
        }
        window.addEventListener("scroll", onScroll, { passive: true });
        onScroll();

        // Smooth scroll for same-page anchors
        document.querySelectorAll('a[href^="#"]').forEach(function (anchor) {
          anchor.addEventListener("click", function (e) {
            var href = anchor.getAttribute("href");
            if (!href || href === "#") return;
            var target = document.querySelector(href);
            if (target) {
              e.preventDefault();
              target.scrollIntoView({ behavior: "smooth", block: "start" });
            }
          });
        });

        // Mobile nav toggle
        var mobileBtn = document.getElementById("mobileMenuButton");
        var mobilePanel = document.getElementById("mobileNavPanel");
        function setMobileOpen(isOpen) {
          if (!mobileBtn || !mobilePanel) return;
          mobilePanel.classList.toggle("open", isOpen);
          mobileBtn.setAttribute("aria-expanded", isOpen ? "true" : "false");
        }
        if (mobileBtn) {
          mobileBtn.addEventListener("click", function () {
            var isOpen = mobilePanel && mobilePanel.classList.contains("open");
            setMobileOpen(!isOpen);
          });
        }
        // Close mobile nav on link click
        var mobileLinks = document.getElementById("navLinksMobile");
        if (mobileLinks) {
          mobileLinks.querySelectorAll('a[href^="#"]').forEach(function (a) {
            a.addEventListener("click", function () {
              setMobileOpen(false);
            });
          });
        }

        // Tabs: Engagement Models
        var tabButtons = document.querySelectorAll(".tab-button");
        var tabPanels = document.querySelectorAll(".tab-content");

        function setActiveTab(modelId, buttonEl) {
          tabPanels.forEach(function (panel) {
            panel.classList.toggle("active", panel.id === modelId);
          });
          tabButtons.forEach(function (btn) {
            var isActive = btn === buttonEl;
            btn.classList.toggle("active", isActive);
            btn.setAttribute("aria-selected", isActive ? "true" : "false");
          });
        }

        tabButtons.forEach(function (btn) {
          btn.addEventListener("click", function () {
            var modelId = btn.getAttribute("data-model");
            if (!modelId) return;
            var panel = document.getElementById(modelId);
            if (!panel) return;
            setActiveTab(modelId, btn);
          });
        });

        // Default to Model 1
        var defaultBtn = document.querySelector('.tab-button[data-model="model1"]');
        if (defaultBtn) {
          setActiveTab("model1", defaultBtn);
        }

        // Scroll animations
        var observerOptions = { threshold: 0.1, rootMargin: "0px 0px -50px 0px" };
        var observer = new IntersectionObserver(function (entries) {
          entries.forEach(function (entry) {
            if (entry.isIntersecting) {
              entry.target.classList.add("visible");
            }
          });
        }, observerOptions);

        document.querySelectorAll(".fade-in").forEach(function (el) {
          observer.observe(el);
        });

        // Form submission (simulated)
        var contactForm = document.getElementById("contactForm");
        if (contactForm) {
          contactForm.addEventListener("submit", function (e) {
            e.preventDefault();
            alert("Thank you for your interest! We will contact you within 24 hours to schedule your free HR infrastructure audit.");
            contactForm.reset();
          });
        }

        // Floating card 3D effect
        document.querySelectorAll(".floating-card").forEach(function (card) {
          card.addEventListener("mousemove", function (e) {
            var rect = card.getBoundingClientRect();
            var x = e.clientX - rect.left;
            var y = e.clientY - rect.top;
            var centerX = rect.width / 2;
            var centerY = rect.height / 2;
            var rotateX = (y - centerY) / 10;
            var rotateY = (centerX - x) / 10;
            card.style.transform = "perspective(1000px) rotateX(" + rotateX + "deg) rotateY(" + rotateY + "deg) translateZ(10px)";
          });
          card.addEventListener("mouseleave", function () {
            card.style.transform = "perspective(1000px) rotateX(0deg) rotateY(0deg) translateZ(0px)";
          });
        });

        // Slideshow
        var currentSlideIndex = 0;
        var slides = document.querySelectorAll(".slide");
        var dots = document.querySelectorAll(".dot");
        var prevBtn = document.getElementById("slidePrev");
        var nextBtn = document.getElementById("slideNext");

        function showSlide(index) {
          if (!slides.length) return;

          slides.forEach(function (s) { s.classList.remove("active"); });
          dots.forEach(function (d) { d.classList.remove("active"); d.setAttribute("aria-selected", "false"); });

          if (index >= slides.length) currentSlideIndex = 0;
          else if (index < 0) currentSlideIndex = slides.length - 1;
          else currentSlideIndex = index;

          slides[currentSlideIndex].classList.add("active");
          if (dots[currentSlideIndex]) {
            dots[currentSlideIndex].classList.add("active");
            dots[currentSlideIndex].setAttribute("aria-selected", "true");
          }
        }

        function changeSlide(direction) {
          showSlide(currentSlideIndex + direction);
        }

        if (prevBtn) prevBtn.addEventListener("click", function () { changeSlide(-1); });
        if (nextBtn) nextBtn.addEventListener("click", function () { changeSlide(1); });

        dots.forEach(function (dot) {
          dot.addEventListener("click", function () {
            var idx = parseInt(dot.getAttribute("data-dot") || "0", 10);
            showSlide(idx);
          });
          dot.addEventListener("keydown", function (e) {
            if (e.key === "Enter" || e.key === " ") {
              e.preventDefault();
              var idx = parseInt(dot.getAttribute("data-dot") || "0", 10);
              showSlide(idx);
            }
          });
        });

        // Auto-advance slideshow every 8 seconds
        if (slides.length > 1) {
          window.setInterval(function () { changeSlide(1); }, 8000);
        }
        showSlide(0);

        // Counter animation for stats
        function animateValue(element, start, end, duration, suffix) {
          var startTimestamp = null;
          function step(timestamp) {
            if (!startTimestamp) startTimestamp = timestamp;
            var progress = Math.min((timestamp - startTimestamp) / duration, 1);
            var value = Math.floor(progress * (end - start) + start);
            element.textContent = String(value) + (suffix || "");
            if (progress < 1) {
              window.requestAnimationFrame(step);
            }
          }
          window.requestAnimationFrame(step);
        }

        var statsSection = document.querySelector(".stats");
        if (statsSection) {
          var statsObserver = new IntersectionObserver(function (entries) {
            entries.forEach(function (entry) {
              if (!entry.isIntersecting) return;
              var statItems = entry.target.querySelectorAll(".stat-item h3");
              statItems.forEach(function (stat) {
                var text = (stat.textContent || "").trim();
                var suffix = stat.getAttribute("data-suffix") || "";

                // Keep original non-numeric formats as-is (e.g., "20 Hours", "28 Days", "30-65")
                // Only animate pure numbers like "99.5" (we'll animate as integer 99 then rely on original if float).
                var numeric = text.replace(/[^\d.]/g, "");
                if (!numeric) return;

                // Animate only if it's a single number (no ranges)
                if (text.indexOf("-") !== -1) return;
                if (text.indexOf(" ") !== -1) return;

                var endValue = parseFloat(numeric);
                if (!isFinite(endValue)) return;

                // For 99.5: animate to 99 and then set final "99.5" + suffix
                if (String(endValue).indexOf(".") !== -1) {
                  animateValue(stat, 0, Math.floor(endValue), 1500, suffix);
                  window.setTimeout(function () {
                    stat.textContent = String(endValue) + suffix;
                  }, 1600);
                } else {
                  animateValue(stat, 0, endValue, 1500, suffix);
                }
              });
              statsObserver.unobserve(entry.target);
            });
          }, { threshold: 0.5 });

          statsObserver.observe(statsSection);
        }
      });
    })();
  </script>
</body>
</html>
