<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我的个人网站</title>
    
    <style>
        /* 基础样式重置 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            color: #333;
            line-height: 1.6;
            background-color: #f9f9f9;
        }

        /* 导航栏 */
        header {
            background: #ffffff;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1100px;
            margin: 0 auto;
            padding: 20px;
        }

        nav .logo {
            font-size: 24px;
            font-weight: bold;
            color: #2c3e50;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: #555;
            font-weight: 600;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: #3498db;
        }

        /* Hero 欢迎区 */
        .hero {
            background: linear-gradient(135deg, #3498db, #2c3e50);
            color: white;
            text-align: center;
            padding: 100px 20px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }

        /* 通用 Section 样式 */
        .section {
            max-width: 1100px;
            margin: 0 auto;
            padding: 80px 20px;
            text-align: center;
        }

        .alt-bg {
            background-color: #f0f4f8;
            max-width: 100%;
            padding-left: calc((100% - 1100px)/2 + 20px);
            padding-right: calc((100% - 1100px)/2 + 20px);
        }

        h2 {
            font-size: 32px;
            margin-bottom: 40px;
            position: relative;
            color: #2c3e50;
        }

        /* Portfolio 网格 */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 20px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            text-align: left;
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            margin-bottom: 15px;
            color: #2c3e50;
        }

        .card p {
            color: #666;
            margin-bottom: 20px;
        }

        .btn {
            display: inline-block;
            padding: 10px 20px;
            background: #3498db;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s;
        }

        .btn:hover {
            background: #2980b9;
        }

        /* Contact 区域 */
        .contact-info {
            margin-top: 30px;
            font-size: 18px;
        }

        .contact-info p {
            margin: 15px 0;
        }

        .contact-info a {
            color: #3498db;
            text-decoration: none;
        }

        /* 页脚 */
        footer {
            background: #2c3e50;
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 14px;
        }
    </style>
</head>
<body>

    <header>
        <nav>
            <div class="logo">我的名字</div>
            <ul>
                <li><a href="#portfolio">作品集 (Portfolio)</a></li>
                <li><a href="#contact">联系我 (Contact)</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h1>你好，我是 [你的名字]</h1>
        <p>欢迎来到我的个人网站！这里展示我的作品与经历。</p>
    </section>

    <section id="portfolio" class="section">
        <h2>作品集 (Portfolio)</h2>
        <div class="grid">
            <div class="card">
                <h3>项目名称一</h3>
                <p>简短的项目描述。你可以写写在这个项目里你用了什么技术，解决了什么问题。</p>
                <a href="#" class="btn">查看详情</a>
            </div>
            <div class="card">
                <h3>项目名称二</h3>
                <p>另一个项目的描述。GitHub Pages 支持随时修改，你可以先用占位文字。</p>
                <a href="#" class="btn">查看详情</a>
            </div>
        </div>
    </section>

    <section id="contact" class="section alt-bg">
        <h2>联系我 (Contact Me)</h2>
        <p>如果你对我的作品感兴趣，或者想一起合作，欢迎通过以下方式联系我：</p>
        <div class="contact-info">
            <p>📧 电子邮箱: <a href="mailto:your-email@example.com">your-email@example.com</a></p>
            <p>🐱 GitHub: <a href="https://github.com/你的用户名" target="_blank">github.com/你的用户名</a></p>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 基于 GitHub Pages 构建</p>
    </footer>

</body>
</html>
