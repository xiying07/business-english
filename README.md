<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>广东科技学院外国语学院 - 商务英语专业</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Noto Sans SC', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f0f5ff 0%, #e6f0ff 100%);
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .header {
            background: linear-gradient(90deg, #1a3a6c 0%, #2c5aa0 100%);
            color: white;
            padding: 1.5rem 0;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .header::before {
            content: "";
            position: absolute;
            top: -50px;
            left: -50px;
            width: 150px;
            height: 150px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
        }
        
        .header::after {
            content: "";
            position: absolute;
            bottom: -30px;
            right: -30px;
            width: 100px;
            height: 100px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
        }
        
        .logo-container {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 1rem;
        }
        
        .logo {
            width: 80px;
            height: 80px;
            background: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        .logo i {
            font-size: 2.5rem;
            color: #2c5aa0;
        }
        
        .header h1 {
            font-size: 2.2rem;
            margin-bottom: 0.5rem;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.3);
        }
        
        .header p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .motto {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 1rem;
            font-weight: 600;
            font-size: 1.1rem;
            letter-spacing: 1px;
        }
        
        .nav-container {
            background: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .nav {
            display: flex;
            justify-content: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .nav a {
            color: #2c5aa0;
            text-decoration: none;
            padding: 1rem 1.5rem;
            font-weight: 600;
            transition: all 0.3s ease;
            position: relative;
        }
        
        .nav a:hover {
            color: #1a3a6c;
            background: #f0f5ff;
        }
        
        .nav a::after {
            content: "";
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 0;
            height: 3px;
            background: #2c5aa0;
            transition: width 0.3s ease;
        }
        
        .nav a:hover::after {
            width: 70%;
        }
        
        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 20px;
        }
        
        .section {
            background: white;
            border-radius: 12px;
            box-shadow: 0 6px 16px rgba(0, 0, 0, 0.08);
            padding: 2.5rem;
            margin-bottom: 2.5rem;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.12);
        }
        
        .section-title {
            color: #1a3a6c;
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
            padding-bottom: 0.8rem;
            border-bottom: 3px solid #2c5aa0;
            display: inline-block;
        }
        
        .history-timeline {
            display: flex;
            justify-content: space-between;
            position: relative;
            margin-top: 2rem;
        }
        
        .history-timeline::before {
            content: "";
            position: absolute;
            top: 20px;
            left: 0;
            right: 0;
            height: 3px;
            background: #2c5aa0;
            z-index: 1;
        }
        
        .history-item {
            text-align: center;
            position: relative;
            z-index: 2;
            flex: 1;
            padding: 0 10px;
        }
        
        .history-year {
            background: #2c5aa0;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 15px;
            font-weight: bold;
            font-size: 1.2rem;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        .history-content {
            background: #f0f5ff;
            padding: 15px;
            border-radius: 8px;
            font-size: 0.95rem;
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .feature-card {
            background: #f8faff;
            border-radius: 10px;
            padding: 1.8rem;
            border-left: 4px solid #2c5aa0;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .feature-card:hover {
            background: #e6f0ff;
            transform: translateY(-3px);
        }
        
        .feature-card h3 {
            color: #1a3a6c;
            margin-bottom: 0.8rem;
            font-size: 1.3rem;
            position: relative;
            z-index: 2;
        }
        
        .feature-card p {
            position: relative;
            z-index: 2;
        }
        
        .feature-card::before {
            content: "";
            position: absolute;
            top: -20px;
            right: -20px;
            width: 60px;
            height: 60px;
            background: rgba(26, 58, 108, 0.05);
            border-radius: 50%;
        }
        
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .stat-card {
            background: linear-gradient(135deg, #e6f0ff 0%, #d4e4fd 100%);
            border-radius: 10px;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
            position: relative;
            overflow: hidden;
        }
        
        .stat-card::before {
            content: "";
            position: absolute;
            top: -15px;
            left: -15px;
            width: 40px;
            height: 40px;
            background: rgba(26, 58, 108, 0.1);
            border-radius: 50%;
        }
        
        .stat-value {
            font-size: 2.2rem;
            font-weight: 700;
            color: #1a3a6c;
            margin-bottom: 0.5rem;
        }
        
        .courses {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .course-category {
            background: #f8faff;
            border-radius: 10px;
            padding: 1.5rem;
            position: relative;
            overflow: hidden;
            transition: all 0.3s ease;
        }
        
        .course-category:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
        }
        
        .course-category::before {
            content: "";
            position: absolute;
            bottom: -20px;
            right: -20px;
            width: 60px;
            height: 60px;
            background: rgba(26, 58, 108, 0.05);
            border-radius: 50%;
        }
        
        .course-category h3 {
            color: #1a3a6c;
            margin-bottom: 1rem;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid #a8c6ff;
            position: relative;
        }
        
        .course-category ul {
            list-style-type: none;
        }
        
        .course-category li {
            padding: 0.5rem 0;
            border-bottom: 1px dashed #d1e0ff;
            position: relative;
            padding-left: 1.2rem;
        }
        
        .course-category li:last-child {
            border-bottom: none;
        }
        
        .course-category li::before {
            content: "•";
            color: #2c5aa0;
            font-weight: bold;
            display: inline-block;
            position: absolute;
            left: 0;
        }
        
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .gallery-item {
            border-radius: 10px;
            overflow: hidden;
            position: relative;
            height: 220px;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
            cursor: pointer;
        }
        
        .gallery-item:hover {
            transform: translateY(-5px);
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .gallery-item:hover img {
            transform: scale(1.05);
        }
        
        .gallery-caption {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: rgba(26, 58, 108, 0.85);
            color: white;
            padding: 12px;
            font-size: 0.95rem;
        }
        
        .student-showcase {
            background: linear-gradient(135deg, #1a3a6c 0%, #2c5aa0 100%);
            border-radius: 12px;
            padding: 2.5rem;
            color: white;
            margin: 3rem 0;
            position: relative;
            overflow: hidden;
        }
        
        .student-showcase::before {
            content: "";
            position: absolute;
            top: -50px;
            right: -50px;
            width: 150px;
            height: 150px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
        }
        
        .student-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
            position: relative;
            z-index: 2;
        }
        
        .student-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s ease;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }
        
        .student-card:hover {
            transform: translateY(-8px);
        }
        
        .student-image {
            height: 200px;
            overflow: hidden;
        }
        
        .student-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .student-card:hover .student-image img {
            transform: scale(1.05);
        }
        
        .student-info {
            padding: 1.2rem;
        }
        
        .student-name {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
        }
        
        .student-details {
            font-size: 0.9rem;
            opacity: 0.9;
        }
        
        .facilities {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .facility-card {
            background: #f8faff;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s ease;
        }
        
        .facility-card:hover {
            transform: translateY(-5px);
        }
        
        .facility-image {
            height: 200px;
            overflow: hidden;
        }
        
        .facility-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .facility-card:hover .facility-image img {
            transform: scale(1.05);
        }
        
        .facility-content {
            padding: 1.5rem;
        }
        
        .facility-title {
            color: #1a3a6c;
            font-size: 1.3rem;
            margin-bottom: 0.8rem;
        }
        
        .footer {
            background: #1a3a6c;
            color: white;
            padding: 2rem 0;
            text-align: center;
            margin-top: 3rem;
        }
        
        .footer-content {
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .school-code {
            font-size: 1.2rem;
            margin: 1rem 0;
            padding: 0.8rem;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 8px;
            display: inline-block;
        }
        
        @media (max-width: 768px) {
            .nav {
                flex-wrap: wrap;
            }
            
            .nav a {
                padding: 0.8rem;
                font-size: 0.9rem;
            }
            
            .history-timeline {
                flex-direction: column;
                align-items: flex-start;
            }
            
            .history-timeline::before {
                display: none;
            }
            
            .history-item {
                margin-bottom: 1.5rem;
                display: flex;
                align-items: center;
                text-align: left;
                width: 100%;
            }
            
            .history-year {
                margin: 0 1rem 0 0;
                flex-shrink: 0;
            }
            
            .section {
                padding: 1.8rem;
            }
        }
        
        .intro-banner {
            background: linear-gradient(rgba(26, 58, 108, 0.8), rgba(26, 58, 108, 0.8)), 
                        url('https://images.unsplash.com/photo-1523240795612-9a054b0db644?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
            height: 400px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            margin: 2rem 0;
            position: relative;
            overflow: hidden;
        }
        
        .intro-content {
            max-width: 800px;
            padding: 0 20px;
            z-index: 2;
        }
        
        .intro-title {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
        }
        
        .intro-text {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }
        
        .highlight {
            color: #FFD700;
            font-weight: 600;
        }
        
        .award-badge {
            background: #FFD700;
            color: #1a3a6c;
            padding: 8px 15px;
            border-radius: 20px;
            font-weight: bold;
            display: inline-block;
            margin-top: 1rem;
        }
        
        .partner-logos {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 2rem;
            margin: 2rem 0;
        }
        
        .partner-logo {
            width: 120px;
            height: 60px;
            background: #f8faff;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            padding: 10px;
        }
        
        .partner-logo img {
            max-width: 100%;
            max-height: 100%;
        }
        
        .talent-cultivation {
            background: linear-gradient(135deg, #1a3a6c 0%, #2c5aa0 100%);
            border-radius: 12px;
            padding: 2.5rem;
            color: white;
            margin: 3rem 0;
            text-align: center;
        }
        
        .cultivation-title {
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
        }
        
        .cultivation-points {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 2rem;
            margin-top: 1.5rem;
        }
        
        .cultivation-point {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 1.5rem;
            width: 250px;
        }
        
        .cultivation-point i {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #FFD700;
        }
        
        .employment-highlights {
            background: #f8faff;
            border-radius: 10px;
            padding: 1.5rem;
            margin: 2rem 0;
            text-align: center;
        }
        
        .highlight-title {
            color: #1a3a6c;
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
        }
        
        .highlight-badge {
            display: inline-block;
            background: #2c5aa0;
            color: white;
            padding: 8px 20px;
            border-radius: 30px;
            margin: 0.5rem;
            font-weight: 500;
        }
        
        /* 课外实践和学生竞赛区域 */
        .practice-section {
            background: linear-gradient(135deg, #f8faff 0%, #e6f0ff 100%);
            border-radius: 12px;
            padding: 2.5rem;
            margin: 3rem 0;
            box-shadow: 0 6px 16px rgba(0, 0, 0, 0.08);
        }
        
        .section-subtitle {
            color: #1a3a6c;
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
            padding-bottom: 0.8rem;
            border-bottom: 3px solid #2c5aa0;
            display: inline-block;
        }
        
        .practice-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.8rem;
            margin-top: 1.8rem;
        }
        
        .practice-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
            transition: all 0.4s ease;
            position: relative;
        }
        
        .practice-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 25px rgba(0, 0, 0, 0.15);
        }
        
        .practice-image {
            height: 220px;
            overflow: hidden;
        }
        
        .practice-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.6s ease;
        }
        
        .practice-card:hover .practice-image img {
            transform: scale(1.08);
        }
        
        .practice-content {
            padding: 1.8rem;
        }
        
        .practice-title {
            color: #1a3a6c;
            font-size: 1.4rem;
            margin-bottom: 1rem;
            font-weight: 600;
        }
        
        .practice-description {
            color: #555;
            margin-bottom: 1.2rem;
            font-size: 1rem;
            line-height: 1.6;
        }
        
        .practice-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 0.6rem;
        }
        
        .practice-badge {
            background: #e6f0ff;
            color: #2c5aa0;
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        .practice-badge:hover {
            background: #2c5aa0;
            color: white;
            transform: translateY(-2px);
        }
        
        /* 回到顶部按钮 */
        .back-to-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 50px;
            height: 50px;
            background: #2c5aa0;
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            z-index: 99;
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.3s ease;
        }
        
        .back-to-top.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        .back-to-top:hover {
            background: #1a3a6c;
            transform: translateY(-3px);
        }
        
        /* 灯箱效果 */
        .lightbox {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 1000;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }
        
        .lightbox.active {
            opacity: 1;
            visibility: visible;
        }
        
        .lightbox-content {
            max-width: 90%;
            max-height: 90%;
        }
        
        .lightbox-content img {
            max-width: 100%;
            max-height: 80vh;
            border-radius: 8px;
        }
        
        .lightbox-close {
            position: absolute;
            top: 20px;
            right: 20px;
            color: white;
            font-size: 2rem;
            cursor: pointer;
            background: rgba(255, 255, 255, 0.2);
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        
        .lightbox-close:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: rotate(90deg);
        }
        
        /* 动画效果 */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .animated {
            animation: fadeInUp 0.6s ease forwards;
        }
    </style>
</head>
<body>
    <header class="header">
        <div class="logo-container">
            <div class="logo">
                <i class="fas fa-graduation-cap"></i>
            </div>
            <div>
                <h1>广东科技学院外国语学院</h1>
                <p>商务英语专业</p>
            </div>
        </div>
        <div class="motto">
            <span>BE GROUNDED</span>
            <span>DARE TO DREAM</span>
        </div>
    </header>

    <div class="nav-container">
        <nav class="nav">
            <a href="#overview">专业概况</a>
            <a href="#faculty">专业师资</a>
            <a href="#training">学生培养</a>
            <a href="#future">学生去向</a>
            <a href="#admission">招生计划</a>
        </nav>
    </div>

    <div class="container">
        <div class="intro-banner">
            <div class="intro-content">
                <h2 class="intro-title">"外语+跨境电商+数字技术"复合型人才</h2>
                <p class="intro-text">以数字技术驱动商业思维  培养兼具国际视野、数字素养与跨境实战能力的应用创新型人才</p>
                <div class="award-badge">2024年艾瑞森校友会5星级一流应用型专业</div>
            </div>
        </div>

        <section id="overview" class="section">
            <h2 class="section-title">专业概况</h2>
            <p>商务英语专业扎根粤港澳大湾区，对接职业需求，采用"三维融合"跨学科培养模式，注重"地方特色+职业能力+本科标准"相结合，培养"外语+跨境电商+数字技术"复合型人才。</p>
            
            <div class="history-timeline">
                <div class="history-item">
                    <div class="history-year">2014</div>
                    <div class="history-content">商务英语专业正式招生</div>
                </div>
                <div class="history-item">
                    <div class="history-year">2018</div>
                    <div class="history-content">成立跨境电商产业学院</div>
                </div>
                <div class="history-item">
                    <div class="history-year">2020</div>
                    <div class="history-content">立项省级产业学院</div>
                </div>
                <div class="history-item">
                    <div class="history-year">2024</div>
                    <div class="history-content">产业学院通过省教育厅验收</div>
                </div>
            </div>
            
            <h3 style="margin-top: 2rem; color: #1a3a6c;">区位优势</h3>
            <p>东莞地处粤港澳大湾区地理中心，全市陆地面积2400平方公里，常住人口1048万人，是全国第15个地区生产总值近万亿、人口超千万的"双万"城市。</p>
            <p>作为国际制造名城，东莞坚持"科技创新+先进制造"的城市特色，拥有涉及34个大类、6万多种产品的完整制造业体系，形成了万亿级电子信息集群和装备制造、新材料、食品饮料、纺织服装4大千亿集群。</p>
            
            <div class="features">
                <div class="feature-card">
                    <h3>专业特色</h3>
                    <p>扎根湾区，对接职业</p>
                    <p>地方特色+职业能力+本科标准</p>
                </div>
                <div class="feature-card">
                    <h3>培养模式</h3>
                    <p>三维融合，跨学科培养</p>
                    <p>外语+跨境电商+数字技术</p>
                </div>
                <div class="feature-card">
                    <h3>产教融合</h3>
                    <p>实战育才，校企合作</p>
                    <p>省级跨境电商产业学院</p>
                </div>
            </div>
            
            <h3 style="margin-top: 2rem; color: #1a3a6c;">产业合作</h3>
            <p>我们与5个企业联盟，近1800家企业建立合作关系，为学生提供真实项目实践机会。</p>
            
            <div class="partner-logos">
                <div class="partner-logo">
                    <i class="fab fa-ebay fa-3x" style="color: #1a3a6c;"></i>
                </div>
                <div class="partner-logo">
                    <i class="fab fa-amazon fa-3x" style="color: #FF9900;"></i>
                </div>
                <div class="partner-logo">
                    <i class="fas fa-globe-asia fa-3x" style="color: #1a3a6c;"></i>
                </div>
            </div>
        </section>

        <section id="faculty" class="section">
            <h2 class="section-title">专业师资</h2>
            <p>商务英语专业拥有一支结构合理、素质优良的师资队伍，现有专业教学团队教师34人。</p>
            
            <div class="stats-container">
                <div class="stat-card">
                    <div class="stat-value">10人</div>
                    <div>副高及以上职称教师</div>
                </div>
                <div class="stat-card">
                    <div class="stat-value">4人</div>
                    <div>外籍教师</div>
                </div>
                <div class="stat-card">
                    <div class="stat-value">13人</div>
                    <div>博士（含在读）</div>
                </div>
                <div class="stat-card">
                    <div class="stat-value">26人</div>
                    <div>"双师双能型"教师</div>
                </div>
            </div>
            
            <div style="margin-top: 2rem; display: flex; justify-content: space-around; flex-wrap: wrap;">
                <div class="stat-card" style="margin: 10px;">
                    <div class="stat-value">100%</div>
                    <div>具有硕士及以上学位教师</div>
                </div>
                <div class="stat-card" style="margin: 10px;">
                    <div class="stat-value">82%</div>
                    <div>具有海外经历教师</div>
                </div>
            </div>
            
            <h3 style="margin-top: 2rem; color: #1a3a6c;">教研成果</h3>
            <ul style="margin-top: 1rem; padding-left: 1.5rem;">
                <li>国家社会科学基金项目：1项</li>
                <li>教育部产学合作协同育人项目：4项</li>
                <li>广东省教学质量与教学改革工程项目：4项</li>
                <li>校企合编教材：3部</li>
                <li>公开发表学术论文：108篇</li>
            </ul>
            
            <h3 style="margin-top: 2rem; color: #1a3a6c;">教学团队风采</h3>
            <div class="gallery">
                <div class="gallery-item">
                    <img src="https://s1.imagehub.cc/images/2025/06/29/47962a55a31a76dbec3fa52929cb7695.jpg" alt="专业教师团队" border="0">
                    <div class="gallery-caption">专业教师团队</div>
                </div>
                <div class="gallery-item">
                   <img src="https://s1.imagehub.cc/images/2025/06/29/208f3acceb4e34a3e1c572672a0f9636.png" alt="教科研成果" border="0">
                    <div class="gallery-caption">教科研成果</div>
                </div>
                <div class="gallery-item">
                    <img src="https://s1.imagehub.cc/images/2025/06/29/4540095bea269d15ef02ab02a055e0e3.png" alt="教学竞赛获奖" border="0">
                    <div class="gallery-caption">教学竞赛获奖</div>
                </div>
            </div>
        </section>

        <section id="training" class="section">
            <h2 class="section-title">学生培养</h2>
            
            <h3 style="margin-top: 1.5rem; color: #1a3a6c;">主干课程</h3>
            <div class="courses">
                <div class="course-category">
                    <h3>必修课</h3>
                    <ul>
                        <li>综合英语</li>
                        <li>英语听力</li>
                        <li>英语口语</li>
                        <li>英语写作</li>
                        <li>商业伦理与企业社会责任</li>
                    </ul>
                </div>
                <div class="course-category">
                    <h3>专业必修课</h3>
                    <ul>
                        <li>综合商务英语</li>
                        <li>商务英语口语</li>
                        <li>商务英语写作</li>
                        <li>国际贸易实务</li>
                        <li>人工智能与英语创新应用</li>
                    </ul>
                </div>
                <div class="course-category">
                    <h3>专业方向课</h3>
                    <ul>
                        <li>跨境电商实务</li>
                        <li>海外社交媒体运营与营销 </li>
                        <li>跨境电商平台运营与推广</li>
                        <li>跨境直播电商</li>
                        <li>跨境电商数据分析</li>
                    </ul>
                </div>
            </div>
            
            <h3 style="margin-top: 2rem; color: #1a3a6c;">教学设备</h3>
            <p>建有42间语言实验室，包括同声传译室、虚拟仿真实验室、虚拟演播室、录播室等；配备跨境电商实训模拟软件。</p>
            
            <div class="facilities">
                <div class="facility-card">
                    <div class="facility-image">
                        <img src="https://s1.imagehub.cc/images/2025/06/29/56e2d48f76b4cdf2e2ad61c676d17996.png" alt="同声传译实验室" border="0">
                    </div>
                    <div class="facility-content">
                        <h3 class="facility-title">同声传译实验室</h3>
                        <p>配备先进的同声传译设备，模拟真实国际会议场景，培养学生专业口译能力。</p>
                    </div>
                </div>
                <div class="facility-card">
                    <div class="facility-image">
                        <img src="https://s1.imagehub.cc/images/2025/06/29/5b547a4983645678ae2b6dd1d0d93480.png" alt="跨境电商实训中心" border="0">
                    </div>
                    <div class="facility-content">
                        <h3 class="facility-title">跨境电商实训中心</h3>
                        <p>模拟真实电商平台操作环境，提供阿里巴巴、亚马逊等平台实操训练。</p>
                    </div>
                </div>
                <div class="facility-card">
                    <div class="facility-image">
                        <img src="https://s1.imagehub.cc/images/2025/06/29/27e5017f1cc8a8478fa017eec7522685.png" alt="虚拟演播室" border="0">
                    </div>
                    <div class="facility-content">
                        <h3 class="facility-title">虚拟演播室</h3>
                        <p>配备绿幕和虚拟场景技术，支持学生开展跨境直播电商实训。</p>
                    </div>
                </div>
            </div>
            
            <div class="talent-cultivation">
                <h3 class="cultivation-title">产教融合，共育人才</h3>
                <p>依托省级跨境电商产业学院，通过"共建专业课程、共筑实习基地、共办特色班"，实施产教融合一体化育人模式，提升学生专业技能与职业竞争力。</p>
                
                <div class="gallery" style="margin-top: 2rem;">
                    <div class="gallery-item">
                        <img src="https://s1.imagehub.cc/images/2025/06/29/698db25d41d9ee739c76854ceca3cda0.png" alt="校企共建专业课程" border="0">
                        <div class="gallery-caption">校企共建专业课程</div>
                    </div>
                    <div class="gallery-item">
                        <img src="https://s1.imagehub.cc/images/2025/06/29/d6abc216b742f0b33ede33c5cb74b629.png" alt="共筑校内外实习基地" border="0">
                        <div class="gallery-caption">共筑校内外实习基地</div>
                    </div>
                    <div class="gallery-item">
                        <img src="https://s1.imagehub.cc/images/2025/06/29/a2e996daff0fa3f3b3081b966affff1f.png" alt="共办跨境电商实战特色班" border="0">
                        <div class="gallery-caption">共办跨境电商实战特色班</div>
                    </div>
                </div>
            </div>
            
            <!-- 课外实践与学生竞赛部分 -->
            <div class="practice-section">
                <h2 class="section-subtitle">课外实践与学生竞赛</h2>
                
                <div class="practice-grid">
                    <div class="practice-card">
                        <div class="practice-image">
                            <img src="https://s1.imagehub.cc/images/2025/06/29/c5c081f1891a698d3aa3e36328d64a8f.png" alt="展会实践" border="0">
                        </div>
                        <div class="practice-content">
                            <h3 class="practice-title">国际展会翻译实践</h3>
                            <p class="practice-description">学生参与广交会、高交会等国际展会，担任商务翻译，提升实战能力与跨文化交际水平。</p>
                            <div class="practice-badges">
                                <span class="practice-badge">翻译实践</span>
                                <span class="practice-badge">跨文化交际</span>
                                <span class="practice-badge">国际展会</span>
                            </div>
                        </div>
                    </div>

                    <div class="practice-card">
                        <div class="practice-image">
                            <img src="https://s1.imagehub.cc/images/2025/06/29/a482626c85a14b9774e624703cc35b27.png" alt="乡村振兴" border="0">
                        </div>
                        <div class="practice-content">
                            <h3 class="practice-title">乡村振兴电商助农</h3>
                            <p class="practice-description">学生运用跨境电商技能助力农产品出口，服务乡村振兴战略，践行社会责任。</p>
                            <div class="practice-badges">
                                <span class="practice-badge">社会实践</span>
                                <span class="practice-badge">乡村振兴</span>
                                <span class="practice-badge">社会责任</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="practice-card">
                        <div class="practice-image">
                            <img src="https://s1.imagehub.cc/images/2025/06/29/5ab563d6a1b9a9e94fe766e535b16b40.png" alt="跨境电商创新创业大赛" border="0">
                        </div>
                        <div class="practice-content">
                            <h3 class="practice-title">跨境电商创新创业大赛</h3>
                            <p class="practice-description">学生参加全国跨境电商大赛，提升平台运营与直播带货能力，多次获得省级奖项。</p>
                            <div class="practice-badges">
                                <span class="practice-badge">直播技能</span>
                                <span class="practice-badge">平台运营</span>
                                <span class="practice-badge">省级荣誉</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="future" class="section">
            <h2 class="section-title">学生去向</h2>
            
            <div class="talent-cultivation">
                <h3 class="cultivation-title">人职匹配、因材施教、分类培养</h3>
                <div class="cultivation-points">
                    <div class="cultivation-point">
                        <i class="fas fa-briefcase"></i>
                        <h4>就业</h4>
                        <p>进入国企、上市公司，运营海外社媒体矩阵</p>
                    </div>
                    <div class="cultivation-point">
                        <i class="fas fa-graduation-cap"></i>
                        <h4>升学考研</h4>
                        <p>近3年考研成功率持续攀升</p>
                    </div>
                    <div class="cultivation-point">
                        <i class="fas fa-trophy"></i>
                        <h4>创新创业</h4>
                        <p>孵化创业项目，创新创业竞赛屡获佳绩</p>
                    </div>
                </div>
            </div>
            
            <div class="employment-highlights">
                <h3 class="highlight-title">毕业生就业亮点</h3>
                <div>
                    <span class="highlight-badge">国有企业</span>
                    <span class="highlight-badge">上市公司</span>
                    <span class="highlight-badge">跨境电商企业</span>
                    <span class="highlight-badge">国际品牌管理</span>
                    <span class="highlight-badge">海外市场拓展</span>
                    <span class="highlight-badge">国际贸易专员</span>
                </div>
            </div>
            
            <div class="student-showcase">
                <h3 style="text-align: center; font-size: 1.6rem; margin-bottom: 1.5rem;">优秀毕业生风采</h3>
                <div class="student-grid">
                    <div class="student-card">
                        <div class="student-image">
                            <img src="https://s1.imagehub.cc/images/2025/06/29/81440caee0f79c4996679319c033ca44.png" alt="实习就业">
                        </div>
                        <div class="student-info">
                            <div class="student-name">实习就业</div>
                            <div class="student-details">就业单位：国有企业、上市公司以及跨境电商企业，从事国际品牌管理、海外市场拓展、外贸业务员、跨境电商运营等工作</div>
                        </div>
                    </div>
                    
                    <div class="student-card">
                        <div class="student-image">
                            <img src="https://s1.imagehub.cc/images/2025/06/29/7c840b70c8885b009ca033fb5c7713fa.png" alt="考研升学">
                        </div>
                        <div class="student-info">
                            <div class="student-name">升学考研</div>
                            <div class="student-details">录取院校：英国曼彻斯特大学、诺丁汉大学、香港浸会大学、广东外语外贸大学、海南大学、汕头大学</div>
                        </div>
                    </div>
                    
                    <div class="student-card">
                        <div class="student-image">
                            <img src="https://s1.imagehub.cc/images/2025/06/29/f2193417d23b97a8bbfcf272d19cf8eb.png" alt="创新创业">
                        </div>
                        <div class="student-info">
                            <div class="student-name">创新创业</div>
                            <div class="student-details">创新创业大赛夺冠：孵化创业项目，开拓海外市场，海外社媒运营助力企业出海</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="admission" class="section">
            <h2 class="section-title">2025年招生计划</h2>
            
            <div style="overflow-x: auto; margin-top: 1.5rem;">
                <table style="width: 100%; border-collapse: collapse; min-width: 600px;">
                    <thead>
                        <tr style="background: #2c5aa0; color: white;">
                            <th style="padding: 12px 15px; text-align: left;">二级学院</th>
                            <th style="padding: 12px 15px; text-align: left;">招生类别</th>
                            <th style="padding: 12px 15px; text-align: left;">专业名称</th>
                            <th style="padding: 12px 15px; text-align: center;">物理类</th>
                            <th style="padding: 12px 15px; text-align: center;">历史类</th>
                            <th style="padding: 12px 15px; text-align: center;">学费(元/年)</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr style="border-bottom: 1px solid #e0e0e0;">
                            <td style="padding: 12px 15px;" rowspan="4">外国语学院</td>
                            <td style="padding: 12px 15px;" rowspan="3">普通类招生专业</td>
                            <td style="padding: 12px 15px;">英语</td>
                            <td style="padding: 12px 15px; text-align: center;">150</td>
                            <td style="padding: 12px 15px; text-align: center;">220</td>
                            <td style="padding: 12px 15px; text-align: center;">34800</td>
                        </tr>
                        <tr style="border-bottom: 1px solid #e0e0e0;">
                            <td style="padding: 12px 15px;">商务英语</td>
                            <td style="padding: 12px 15px; text-align: center;">45</td>
                            <td style="padding: 12px 15px; text-align: center;">45</td>
                            <td style="padding: 12px 15px; text-align: center;">34800</td>
                        </tr>
                        <tr style="border-bottom: 1px solid #e0e0e0;">
                            <td style="padding: 12px 15px;">翻译</td>
                            <td style="padding: 12px 15px; text-align: center;">20</td>
                            <td style="padding: 12px 15px; text-align: center;">25</td>
                            <td style="padding: 12px 15px; text-align: center;">34800</td>
                        </tr>
                        <tr style="border-bottom: 1px solid #e0e0e0;">
                            <td style="padding: 12px 15px;">中外联合培养</td>
                            <td style="padding: 12px 15px;">英语</td>
                            <td style="padding: 12px 15px; text-align: center;">15</td>
                            <td style="padding: 12px 15px; text-align: center;">15</td>
                            <td style="padding: 12px 15px; text-align: center;">49800</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            
            <div style="margin-top: 2rem; text-align: center; font-size: 1.1rem;">
                <p>欢迎报考广东科技学院外国语学院商务英语专业！</p>
                <p style="font-weight: bold; color: #1a3a6c; margin-top: 0.5rem;">学校代码：13719</p>
            </div>
        </section>
    </div>

    <footer class="footer">
        <div class="footer-content">
            <h3>广东科技学院外国语学院</h3>
            <p>商务英语专业招生</p>
            <div class="school-code">学校代码：13719</div>
            <p style="margin-top: 1.5rem; opacity: 0.8;">© 2025 广东科技学院外国语学院 版权所有</p>
        </div>
    </footer>

    <script>
        // 平滑滚动
        document.addEventListener('DOMContentLoaded', function() {
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    const target = document.querySelector(this.getAttribute('href'));
                    if (target) {
                        target.scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                    }
                });
            });
        });
    </script>
</body>
</html>
