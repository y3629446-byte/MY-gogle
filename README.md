<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>محرك البحث المخصص</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #ffffff;
            display: flex;
            flex-direction: column;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }
        .header {
            width: 100%;
            max-width: 600px;
            display: flex;
            justify-content: center;
            margin-bottom: 20px;
        }
        .logo {
            font-size: 3.5rem;
            font-weight: bold;
            letter-spacing: -1px;
            margin-top: 40px;
            margin-bottom: 30px;
        }
        .logo span:nth-child(1) { color: #4285F4; }
        .logo span:nth-child(2) { color: #EA4335; }
        .logo span:nth-child(3) { color: #FBBC05; }
        .logo span:nth-child(4) { color: #4285F4; }
        .logo span:nth-child(5) { color: #34A853; }
        .logo span:nth-child(6) { color: #EA4335; }

        /* منطقة محرك بحث جوجل المخصص */
        .search-container {
            width: 100%;
            max-width: 600px;
            margin-bottom: 25px;
        }

        /* الميزات الإضافية (محاكاة الواجهة المطلوبة) */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
            width: 100%;
            max-width: 600px;
            margin-bottom: 25px;
        }
        .feature-card {
            background: #f8f9fa;
            border: 1px solid #dadce0;
            border-radius: 12px;
            padding: 15px;
            text-align: center;
            font-size: 0.9rem;
            color: #3c4043;
        }
        .feature-card h4 {
            font-size: 0.8rem;
            color: #70757a;
            margin-bottom: 5px;
        }
        .feature-card p {
            font-weight: bold;
            font-size: 1.1rem;
        }
        .feed-container {
            width: 100%;
            max-width: 600px;
            border: 1px solid #dadce0;
            border-radius: 16px;
            overflow: hidden;
            background: #fff;
            box-shadow: 0 1px 6px rgba(32,33,36,0.1);
        }
        .feed-image {
            width: 100%;
            height: 250px;
            background-color: #e8eaed;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #70757a;
        }
        .feed-content {
            padding: 15px;
        }
        .feed-title {
            font-size: 1.1rem;
            font-weight: bold;
            margin-bottom: 8px;
            color: #202124;
        }
    </style>
</head>
<body>

    <!-- الشعار الملون -->
    <div class="logo">
        <span>G</span><span>o</span><span>o</span><span>g</span><span>l</span><span>e</span>
    </div>

    <!-- صندوق البحث المرتبط بسيرفر جوجل -->
    <div class="search-container">
        <!-- ضع كود الـ <script> الخاص بك هنا ليعمل البحث -->
        <script async src="https://cse.google.com/cse.js?cx=55e3aaa1fc35c4e1c"></script>
        <div class="gcse-search"></div>
    </div>

    <!-- قسم الميزات الذكية (أرقام توضيحية) -->
    <div class="features-grid">
        <div class="feature-card">
            <h4>المحتوى الرائج</h4>
            <p>العراق 3 - 2 الكويت</p>
        </div>
        <div class="feature-card">
            <h4>الطقس الحالي</h4>
            <p>42° مئوية</p>
        </div>
        <div class="feature-card">
            <h4>الوقت الحالي</h4>
            <p>04:14 PM</p>
        </div>
    </div>

    <!-- قسم الأخبار التفاعلي (Feed) -->
    <div class="feed-container">
        <div class="feed-image">
            [ مساحة مخصصة لصورة الخبر ]
        </div>
        <div class="feed-content">
            <div class="feed-title">عنوان الخبر المقترح للزائر يظهر هنا بشكل تلقائي</div>
            <p style="color: #5f6368; font-size: 0.9rem;">متابعة بواسطة حيدر علي</p>
        </div>
    </div>

</body>
</html>
