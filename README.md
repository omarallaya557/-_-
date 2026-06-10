<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>بن أمازون | الفخامة في كل حبة</title>
    
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Store",
      "name": "بن أمازون",
      "image": "logo.png",
      "telephone": "+201152277696",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Alexandria",
        "addressCountry": "EG"
      },
      "url": "https://www.banamazon.com",
      "sameAs": [
        "https://wa.me/201152277696"
      ]
    }
    </script>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Amiri:ital@1&family=Marcellus&family=Cairo:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        /* ==========================================================================
           1. المتغيرات والألوان الأساسية (Theming & Variables)
           ========================================================================== */
        :root {
            --bg-primary: #fdfbf7;
            --bg-secondary: #f4eee1;
            --card-bg: rgba(255, 255, 255, 0.85);
            --text-main: #2b1b17;
            --text-muted: #5c4033;
            --accent-gold: #c5a059;
            --accent-gold-hover: #a38141;
            --coffee-dark: #3e2723;
            --glass-border: rgba(197, 160, 89, 0.2);
            --shadow: 0 10px 30px rgba(62, 39, 35, 0.05);
            --transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
        }

        [data-theme="dark"] {
            --bg-primary: #120c0a;
            --bg-secondary: #1a120f;
            --card-bg: rgba(26, 18, 15, 0.8);
            --text-main: #f4eee1;
            --text-muted: #d7ccc8;
            --glass-border: rgba(197, 160, 89, 0.3);
            --shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
        }

        /* إعادة ضبط العناصر الأساسية */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Cairo', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-primary);
            color: var(--text-main);
            transition: var(--transition);
            overflow-x: hidden;
        }

        /* ==========================================================================
           3. الهيدر والبطل (Header & Hero Section)
           ========================================================================== */
        header {
            background: linear-gradient(to bottom, rgba(62, 39, 35, 0.95), rgba(43, 27, 23, 0.95));
            color: #fff;
            padding: 25px 5%;
            text-align: center;
            position: relative;
            box-shadow: 0 5px 20px rgba(0,0,0,0.3);
        }
        
        .header-top {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto 20px auto;
        }

        .logo-area {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .logo-placeholder {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            border: 2px solid var(--accent-gold);
            display: flex; align-items: center; justify-content: center;
            background: rgba(255,255,255,0.1);
            font-size: 1.5rem; color: var(--accent-gold);
        }

        .brand-name {
            font-family: 'Amiri', serif;
            font-size: 2.5rem;
            font-weight: bold;
            color: var(--accent-gold);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.4);
        }

        .theme-toggle-btn {
            background: none;
            border: 2px solid var(--accent-gold);
            color: var(--accent-gold);
            padding: 8px 15px; border-radius: 20px;
            cursor: pointer; transition: var(--transition);
        }
        .theme-toggle-btn:hover {
            background: var(--accent-gold);
            color: #fff;
        }

        /* شريط البحث المتقدم */
        .search-container {
            max-width: 500px;
            margin: 15px auto 0 auto;
            position: relative;
        }
        .search-input {
            width: 100%;
            padding: 12px 20px 12px 50px;
            border-radius: 30px; border: 1px solid var(--accent-gold);
            background: rgba(255,255,255,0.1);
            color: #fff; font-size: 1rem; transition: var(--transition);
        }
        .search-input:focus {
            background: rgba(255,255,255,0.2);
            outline: none; box-shadow: 0 0 10px rgba(197, 160, 89, 0.5);
        }
        .search-container i {
            position: absolute;
            left: 20px; top: 50%;
            transform: translateY(-50%); color: var(--accent-gold);
        }

        /* بنر الترحيب الفاخر */
        .hero {
            padding: 60px 20px;
            text-align: center;
            background: linear-gradient(rgba(43,27,23,0.6), rgba(43,27,23,0.8)), url('mahmas.jpg') no-repeat center/cover;
            color: #fff;
            margin-bottom: 40px;
        }
        .hero h2 { font-family: 'Amiri', serif; font-size: 3rem; margin-bottom: 10px; color: var(--accent-gold); }
        .hero p { font-size: 1.2rem; max-width: 600px; margin: 0 auto; opacity: 0.9; }

        /* ==========================================================================
           4. أزرار الفلترة والتصنيفات العصرية (Navigation Grid)
           ========================================================================== */
        .categories-container {
            max-width: 1200px;
            margin: 0 auto 40px auto;
            padding: 0 20px;
        }
        .categories-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(130px, 1fr));
            gap: 15px;
            justify-content: center;
        }
        .cat-card {
            background: var(--bg-secondary);
            border: 1px solid var(--glass-border);
            padding: 20px 10px;
            border-radius: 15px;
            text-align: center;
            cursor: pointer;
            transition: var(--transition);
            box-shadow: var(--shadow);
            font-weight: 600;
        }
        .cat-card i {
            display: block;
            font-size: 1.8rem; margin-bottom: 10px; color: var(--accent-gold);
            transition: var(--transition);
        }
        .cat-card:hover, .cat-card.active {
            background: var(--coffee-dark);
            color: #fff;
            transform: translateY(-5px);
            border-color: var(--accent-gold);
        }
        .cat-card:hover i, .cat-card.active i {
            color: #fff;
            transform: scale(1.1);
        }

        /* ==========================================================================
           5. شبكة المنتجات (Products Grid)
           ========================================================================== */
        .main-content {
            max-width: 1200px;
            margin: 0 auto 60px auto;
            padding: 0 20px;
        }
        .section-title {
            font-family: 'Amiri', serif;
            font-size: 2.2rem;
            margin-bottom: 30px;
            border-bottom: 2px solid var(--accent-gold);
            padding-bottom: 10px;
            display: inline-block;
        }
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
            animation: fadeIn 0.8s ease forwards;
        }

        /* كارد المنتج الاحترافي (Glassmorphism Effect) */
        .product-card {
            background: var(--card-bg);
            border: 1px solid var(--glass-border);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        
        .product-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 20px 40px rgba(197, 160, 89, 0.15);
            border-color: var(--accent-gold);
        }

        .img-container {
            width: 100%;
            height: 230px;
            overflow: hidden;
            position: relative;
            background: #eee;
        }
        .product-card:hover .product-img {
            transform: scale(1.12);
        }
        .product-img {
            width: 100%;
            height: 100%; object-fit: cover;
            transition: var(--transition);
        }

        .product-info {
            padding: 20px;
            text-align: center;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .product-name {
            font-size: 1.3rem;
            font-weight: 700; margin-bottom: 10px; color: var(--text-main);
        }
        .product-desc {
            font-size: 0.95rem;
            color: var(--text-muted); margin-bottom: 20px; line-height: 1.6;
        }

        .order-btn {
            background: linear-gradient(135deg, var(--accent-gold), var(--accent-gold-hover));
            color: white; border: none; padding: 12px 25px;
            border-radius: 30px; font-weight: 600; cursor: pointer;
            transition: var(--transition); width: 100%;
            display: flex;
            align-items: center; justify-content: center; gap: 10px;
            text-decoration: none; box-shadow: 0 4px 15px rgba(197,160,89,0.3);
        }
        .order-btn:hover {
            box-shadow: 0 6px 20px rgba(197,160,89,0.5);
            transform: translateY(-2px);
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* ==========================================================================
           6. الفوتر وزر الواتساب العائم (Footer & Floating WhatsApp)
           ========================================================================== */
        footer {
            background: #1a120f;
            color: #f4eee1;
            padding: 40px 20px;
            text-align: center;
            border-top: 3px solid var(--accent-gold);
        }
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: flex; flex-direction: column; gap: 20px; align-items: center;
        }
        .footer-contacts {
            display: flex;
            gap: 30px; flex-wrap: wrap; justify-content: center;
        }
        .contact-item {
            font-size: 1.1rem;
            text-decoration: none; color: #f4eee1;
            display: flex; align-items: center; gap: 10px; transition: var(--transition);
        }
        .contact-item:hover { color: var(--accent-gold); }
        .contact-item i { font-size: 1.4rem; color: var(--accent-gold); }
        
        .whatsapp-float {
            position: fixed;
            bottom: 30px; left: 30px;
            background-color: #25d366; color: white;
            width: 60px; height: 60px; border-radius: 50%;
            display: flex; align-items: center; justify-content: center;
            font-size: 30px; box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            z-index: 100; transition: var(--transition);
            text-decoration: none;
        }
        .whatsapp-float:hover { transform: scale(1.1) rotate(10deg); background-color: #20ba5a; }

        /* الشاشات الصغيرة */
        @media (max-width: 768px) {
            .header-top { flex-direction: column; gap: 15px; }
            .hero h2 { font-size: 2.2rem; }
            .categories-grid { grid-template-columns: repeat(3, 1fr); }
        }
        @media (max-width: 480px) {
            .categories-grid { grid-template-columns: repeat(2, 1fr); }
        }
    </style>
</head>
<body>

    <header>
        <div class="header-top">
            <div class="logo-area">
<div class="logo-placeholder">
    <img src="logo.jpg" alt="logo.jpg" style="width: 100%; height: 100%; border-radius: 50%; object-fit: cover;">
</div>
                <h1 class="brand-name">بن أمازون</h1>
            </div>
            <button class="theme-toggle-btn" onclick="toggleTheme()" id="themeBtn">
                <i class="fa-solid fa-moon"></i> المظهر الداكن
            </button>
        </div>
        
        <div class="search-container">
            <input type="text" id="searchInput" class="search-input" placeholder="ابحث عن قهوتك، مكسراتك أو حلوياتك المفضل..." onkeyup="searchProducts()">
            <i class="fa-solid fa-magnifying-glass"></i>
        </div>
    </header>

    <section class="hero">
        <h2>عالم من المذاق الرفيع</h2>
        <p>نعمل بأجود حبات البن والمكسرات العالمية ونحمصها بشغف عربي لتصل إليكم طازجة وفاخرة.</p>
    </section>

    <div class="categories-container">
        <div class="categories-grid">
            <div class="cat-card" onclick="filterCategory('all', this)" id="defaultCat"><i class="fa-solid fa-border-all"></i>الكل</div>
            <div class="cat-card" onclick="filterCategory('nuts', this)"><i class="fa-solid fa-seedling"></i>المكسرات</div>
            <div class="cat-card" onclick="filterCategory('coffee', this)"><i class="fa-solid fa-mug-hot"></i>القهوة</div>
            <div class="cat-card" onclick="filterCategory('seeds', this)"><i class="fa-solid fa-spa"></i>اللب</div>
            <div class="cat-card" onclick="filterCategory('sweets', this)"><i class="fa-solid fa-candy-cane"></i>شوكولا وحلويات</div>
            <div class="cat-card" onclick="filterCategory('savory', this)"><i class="fa-solid fa-cheese"></i>حوادق</div>
            <div class="cat-card" onclick="filterCategory('offers', this)"><i class="fa-solid fa-tags"></i>العروض الحصرية</div>
           <div class="cat-card" onclick="filterCategory('others', this)"><i class="fa-solid fa-ellipsis-h"></i>أخرى</div>
        </div>
    </div>

    <main class="main-content">
        <h2 class="section-title" id="sectionTitle">كل المنتجات الفاخرة</h2>
        <div class="products-grid" id="productsGrid"></div>
    </main>

    <footer>
        <div class="footer-content">
            <h3 style="font-family: 'Amiri', serif; font-size: 1.8rem; color: var(--accent-gold);">بن أمازون</h3>
            <p>الجودة دائماً تتحدث عن نفسها. طلباتكم تصلكم أينما كنتم.</p>
            <div class="footer-contacts">
                <a href="tel:+201152277696" class="contact-item">
                    <i class="fa-solid fa-phone"></i> 0115 227 7696
                </a>
                <a href="https://wa.me/201152277696" target="_blank" class="contact-item">
                    <i class="fa-brands fa-whatsapp"></i> 0115 227 7696
                </a>
            </div>
            <p style="font-size: 0.85rem; opacity: 0.6; margin-top: 20px;">&copy; 2026 بن أمازون. جميع الحقوق محفوظة.</p>
        </div>
    </footer>

    <a href="https://wa.me/201152277696" class="whatsapp-float" target="_blank" title="تواصل معنا فوراً">
        <i class="fa-brands fa-whatsapp"></i>
    </a>

    <script>
        // قاعدة بيانات المنتجات - التعديلات الأخيرة
        const productsData = [
            // ==================== تصنيف القهوة (coffee) ====================
            { id: 1, category: 'coffee', name: 'بن السيلفر', desc: '', img: 'images/gomaa.jpg' },
            { id: 2, category: 'coffee', name: 'بن الجولد', desc: '', img: 'https://images.unsplash.com/photo-1509042239860-f550ce710b93?q=80&w=600' },
            { id: 3, category: 'coffee', name: 'بن برونز', desc: '', img: 'https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?q=80&w=600' },
            { id: 4, category: 'coffee', name: 'بن وسط', desc: '', img: 'https://images.unsplash.com/photo-1511920170033-f8396924c348?q=80&w=600' },
            { id: 5, category: 'coffee', name: 'بن فاتح', desc: '', img: 'https://images.unsplash.com/photo-1541167760496-1628856ab772?q=80&w=600' },
            { id: 6, category: 'coffee', name: 'بن غامق', desc: '', img: 'https://images.unsplash.com/photo-1514432324607-a09d9b4aefdd?q=80&w=600' },
            { id: 7, category: 'coffee', name: 'بن اسبريسو', desc: '', img: 'https://images.unsplash.com/photo-1510972527409-cca19de31749?q=80&w=600' },
            { id: 8, category: 'coffee', name: 'قهوة فرنساوي', desc: 'قهوة مع سكر وحليب فرنساوي سادة - فلفر بندق - قطع بندق', img: 'https://images.unsplash.com/photo-1534778101976-62847782c213?q=80&w=600' },
            { id: 9, category: 'coffee', name: 'نسكافيه 3×1', desc: '', img: 'https://images.unsplash.com/photo-1578314675249-a6910f80cc4e?q=80&w=600' },
            { id: 10, category: 'coffee', name: 'نسكافيه بلاك', desc: '', img: 'https://images.unsplash.com/photo-1607687325211-ac6624da304a?q=80&w=600' },
            { id: 11, category: 'coffee', name: 'قهوة مرة عربية', desc: 'قهوة من 6 أنواع بن مختلفة سريعة التحضير قوية الكافيين طعمها مرار مع حموضة تحميصها غامق', img: 'https://images.unsplash.com/photo-1599639085605-a044456868a1?q=80&w=600' },

            // ==================== تصنيف المكسرات (nuts) ====================
            { id: 12, category: 'nuts', name: 'كاجو', desc: '', img: 'https://images.unsplash.com/photo-1536510233921-8e5043fce771?q=80&w=600' },
            { id: 13, category: 'nuts', name: 'كاجو مدخن', desc: '', img: 'https://images.unsplash.com/photo-1536510233921-8e5043fce771?q=80&w=600' },
            { id: 14, category: 'nuts', name: 'فستق حلبي', desc: '', img: 'https://images.unsplash.com/photo-1596547609652-9cf5d8d76921?q=80&w=600' },
            { id: 15, category: 'nuts', name: 'فستق حلبي مدخن', desc: '', img: 'https://images.unsplash.com/photo-1596547609652-9cf5d8d76921?q=80&w=600' },
            { id: 16, category: 'nuts', name: 'عين جمل', desc: '', img: 'https://images.unsplash.com/photo-1600189020840-e9da189b7c3f?q=80&w=600' },
            { id: 18, category: 'nuts', name: 'لوز مدخن', desc: '', img: 'https://images.unsplash.com/photo-1508061253366-f7da158b6d46?q=80&w=600' },
            { id: 19, category: 'nuts', name: 'لوز مالح', desc: '', img: 'https://images.unsplash.com/photo-1508061253366-f7da158b6d46?q=80&w=600' },
            { id: 20, category: 'nuts', name: 'تشكيلة مكسرات اكسترا', desc: '', img: 'https://images.unsplash.com/photo-1541532713592-79a0317b6b77?q=80&w=600' },

            // ==================== تصنيف اللب (seeds) ====================
            { id: 21, category: 'seeds', name: 'سوداني فلسطيني', desc: 'تحميص مالح وعليه قرمشة سكرية', img: 'https://images.unsplash.com/photo-1567331707731-60ac995583b5?q=80&w=600' },
            { id: 22, category: 'seeds', name: 'سوداني مدخن', desc: '', img: 'https://images.unsplash.com/photo-1567331707731-60ac995583b5?q=80&w=600' },
            { id: 23, category: 'seeds', name: 'لب أبيض قرع', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 24, category: 'seeds', name: 'لب سوبر', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 25, category: 'seeds', name: 'لب سوبر مدخن', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 26, category: 'seeds', name: 'لب أفغاني', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 27, category: 'seeds', name: 'لب كوسا', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 28, category: 'seeds', name: 'لب كوسا مدخن', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 29, category: 'seeds', name: 'أبيض قرع متقشر', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 30, category: 'seeds', name: 'لب أسود', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 31, category: 'seeds', name: 'قضامة', desc: 'حمص مقرمش على الطريقة السورية مالح - سادة - سكر', img: 'https://images.unsplash.com/photo-1536510233921-8e5043fce771?q=80&w=600' },

            // ==================== تصنيف الحلويات والشوكولا (sweets) ====================
            { id: 32, category: 'sweets', name: 'اوريانا', desc: 'شوكولا محشية شوكولا سائلة مع حليب', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 33, category: 'sweets', name: 'جوز هند', desc: 'شوكولا محشية جوز هند', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 34, category: 'sweets', name: 'نسله', desc: 'شوكولا محشية حليب مكثف محلى', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 35, category: 'sweets', name: 'لاكتيه سائلة', desc: 'شوكولا محشية عجينة كاكاو سائلة', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 36, category: 'sweets', name: 'لاكتيه', desc: 'شوكولا محشية عجينة كاكاو', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 37, category: 'sweets', name: 'دارك سادة', desc: 'شوكولا دارك سادة 100%', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 38, category: 'sweets', name: 'كاستا مع فستق حلبي', desc: 'شوكولا محشية كاستا بالحليب مع حبات فستق حلبي الصحيحة', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 39, category: 'sweets', name: '6 بندق', desc: 'شوكولا محشية 6 حبات بندق مغطسة بطبقة سكر محروق وطبقة شوكولا حليب', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 40, category: 'sweets', name: 'مشكل أطعم', desc: 'كراميل - وايت - دارك - فراولة - بندق', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 42, category: 'sweets', name: 'شوكولا رول', desc: '', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 43, category: 'sweets', name: 'ويفر محشي', desc: 'ويفر مقرمش لوتس - شوكولا - فراولة', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 44, category: 'sweets', name: 'شوكولا سميري', desc: '', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 45, category: 'sweets', name: 'شوكولا حجر بحر', desc: '', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },
            { id: 46, category: 'sweets', name: 'كونو محشي', desc: 'قطعة بسكوت على شكل كونو شوكولا بنية - فراولة - شوكولا بيضاء', img: 'https://images.unsplash.com/photo-1548907040-4d42b52145ca?q=80&w=600' },

            // ==================== تصنيف حوادق (savory) ====================
            { id: 47, category: 'savory', name: 'سوداني مقرمش بطعم', desc: 'جبنة - فراخ - كاتشب - خل وملح - باربكيو', img: 'https://images.unsplash.com/photo-1567331707731-60ac995583b5?q=80&w=600' },
            { id: 48, category: 'savory', name: 'لب مقشر بطعم', desc: 'جبنة - كاتشب - فراخ - باربكيو - خل وملح', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },
            { id: 49, category: 'savory', name: 'درة اسباني بطعم', desc: 'جبنة - كاتشب - مدخن - باربكيو - ملح', img: 'https://images.unsplash.com/photo-1536510233921-8e5043fce771?q=80&w=600' },
            { id: 50, category: 'savory', name: 'مقرمشات سورية', desc: 'مقرمشات مشوية مختلفة الأطعمة وملونة', img: 'https://images.unsplash.com/photo-1536510233921-8e5043fce771?q=80&w=600' },
            { id: 51, category: 'savory', name: 'مقرمشات صيني', desc: '', img: 'https://images.unsplash.com/photo-1536510233921-8e5043fce771?q=80&w=600' },
            { id: 52, category: 'savory', name: 'بريتزل بطعم', desc: 'جبنة - كاتشب - جبنة شيدر - باربكيو - خل وملح - ملح - شطة', img: 'https://images.unsplash.com/photo-1536510233921-8e5043fce771?q=80&w=600' },

            // ==================== تصنيف العروض الحصرية (offers) ====================
            { id: 53, category: 'offers', name: 'تشكيلة مكسرات اكسترا الفاخرة', desc: '', img: 'https://images.unsplash.com/photo-1541532713592-79a0317b6b77?q=80&w=600' },
            { id: 54, category: 'offers', name: 'تشكيلة لب اكسترا', desc: '', img: 'https://images.unsplash.com/photo-1590004953392-5aba2e72269a?q=80&w=600' },

            // ==================== تصنيف أخرى (others) ====================
            { id: 55, category: 'others', name: 'عسل أمازون', desc: 'عسل أصلي من مناحلنا الأنواع: سدر جيلي - حبة البركة - أعشاب - برسيم - سمسم', img: 'https://images.unsplash.com/photo-1587049352846-4a222e784d38?q=80&w=600' },
            { id: 56, category: 'others', name: 'بسكوت مشكل', desc: 'بسكویت وشوكولا من أجود أنواع المیجا والإیلیت والكوفرتینا', img: 'https://images.unsplash.com/photo-1558961312-50346c099379?q=80&w=600' },
            { id: 57, category: 'others', name: 'سكاكر', desc: 'توفي - جیلي - كرامیلة بأطعمة مختلفة', img: 'https://images.unsplash.com/photo-1581798459219-318e76aecc7b?q=80&w=600' },
            { id: 58, category: 'others', name: 'كاندي اسباني وتركي', desc: 'تشكیلة كبیرة من أجود أنواع الكاندي الإسباني والتركي الساور والسويت والجيلي', img: 'https://images.unsplash.com/photo-1581798459219-318e76aecc7b?q=80&w=600' },
            { id: 59, category: 'others', name: 'عشبة المتة', desc: 'عشبة أرجنتينية فيها كافيين ولها فوائد عديدة ومحفزة للنشاط', img: 'https://images.unsplash.com/photo-1515694346937-94d85e41e6f0?q=80&w=600' },
            { id: 60, category: 'others', name: 'تمور الخضري والسكري', desc: 'تمور خضري وتمور سكري نوع أول فاخر من شركة الطحان المصرية ', img: 'https://images.unsplash.com/photo-1530260626688-048279320445?q=80&w=600' }
        ];

        let currentCategory = 'all';

        // دالة تفعيل الأقسام فور فتح الصفحة مباشرة وبسرعة
        document.addEventListener('DOMContentLoaded', () => {
            document.getElementById('defaultCat').classList.add('active');
            renderProducts(productsData);
        });

        // دالة عرض الكروت داخل الـ Grid
        function renderProducts(productsToShow) {
            const grid = document.getElementById('productsGrid');
            grid.innerHTML = '';

            if(productsToShow.length === 0) {
                grid.innerHTML = `<p style="text-align:center; grid-column: 1/-1; font-size:1.2rem; opacity:0.7; padding: 40px 0;">عذراً، لم نجد أي صنف يطابق بحثك.</p>`;
                return;
            }

            productsToShow.forEach(product => {
                const whatsappMessage = encodeURIComponent(`مرحباً بن أمازون، أريد طلب هذا الصنف: ${product.name}`);
                const whatsappUrl = `https://wa.me/201152277696?text=${whatsappMessage}`;

                const card = document.createElement('div');
                card.className = 'product-card';
                card.innerHTML = `
                    <div class="img-container">
                        <img src="${product.img}" alt="${product.name}" class="product-img" loading="lazy">
                    </div>
                    <div class="product-info">
                        <div>
                            <h3 class="product-name">${product.name}</h3>
                            <p class="product-desc">${product.desc}</p>
                        </div>
                        <a href="${whatsappUrl}" target="_blank" class="order-btn">
                            <i class="fa-brands fa-whatsapp"></i> طلب هذا الصنف
                        </a>
                    </div>
                `;
                grid.appendChild(card);
            });
        }

        // دالة فلترة المنتجات عند الضغط على التصنيفات
        function filterCategory(category, element) {
            currentCategory = category;
            
            // تحديث تصميم الزر النشط
            document.querySelectorAll('.cat-card').forEach(card => card.classList.remove('active'));
            element.classList.add('active');
            
            // إعادة ضبط حقل البحث عند تغيير التصنيف
            document.getElementById('searchInput').value = '';
            
            // تحديث عنوان القسم
            const titles = {
                'all': 'كل المنتجات الفاخرة',
                'coffee': 'ركن القهوة والبن الفاخر',
                'nuts': 'المكسرات العربية المحمصة',
                'seeds': 'تسالي اللب والسوداني',
                'sweets': 'شوكولا وحلويات بن أمازون',
                'savory': 'المقرمشات والحوادق الطازجة',
                'offers': 'العروض الحصرية والمميزة',
                'others': 'منتجاتنا الأخرى المختارة'
            };
            document.getElementById('sectionTitle').innerText = titles[category] || 'منتجاتنا';

            // الفلترة الفعلية للبيانات
            const filtered = category === 'all' ? productsData : productsData.filter(p => p.category === category);
            
            // تطبيق أنيميشن إعادة التحميل الفوري
            const grid = document.getElementById('productsGrid');
            grid.style.animation = 'none';
            grid.offsetHeight; /* تلميح لإعادة تشغيل الأنيميشن */
            grid.style.animation = 'fadeIn 0.6s ease forwards';
            
            renderProducts(filtered);
        }

        // شريط البحث المتقدم الفوري
        function searchProducts() {
            const query = document.getElementById('searchInput').value.trim().toLowerCase();
            
            // فلترة بناء على التصنيف الحالي وبناء على كلمة البحث في الاسم أو الوصف
            const filtered = productsData.filter(product => {
                const matchesCategory = currentCategory === 'all' || product.category === currentCategory;
                const matchesSearch = product.name.toLowerCase().includes(query) || product.desc.toLowerCase().includes(query);
                return matchesCategory && matchesSearch;
            });

            renderProducts(filtered);
        }

        // دالة الوضع الليلي والنهاري الفاخر (Dark Mode)
        function toggleTheme() {
            const currentTheme = document.documentElement.getAttribute('data-theme');
            const targetTheme = currentTheme === 'dark' ? 'light' : 'dark';
            const themeBtn = document.getElementById('themeBtn');

            document.documentElement.setAttribute('data-theme', targetTheme);
            if(targetTheme === 'dark') {
                themeBtn.innerHTML = `<i class="fa-solid fa-sun"></i> المظهر المضيء`;
            } else {
                themeBtn.innerHTML = `<i class="fa-solid fa-moon"></i> المظهر الداكن`;
            }
        }
    </script>
</body>
</html>
