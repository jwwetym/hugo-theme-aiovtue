---
title: "第九集"
description: "2026年7月31日"
date: 2026-08-26
lastmod: 2026-08-26
cover: "https://yy.ms1.asia/lzyzbsl/lzyzbsl.jpg"
categories:
  - 老中医诊病实录
tags:
  - 老中医诊病实录
ai: 好好学习，实时观摩
pinned: true
---
<a href="https://yy.ms1.asia/lzyzbsl/9/9.mp4" target="_blank" rel="noopener" style="display:inline-block; background:#DF9193; color:#fff; padding:10px 24px; border-radius:8px; text-decoration:none; font-weight:bold; margin:20px 0;">
    ▶ 点击播放视频
</a>

<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>📸 图片画廊</title>
    <style>
        /* ===== 全局重置 & 字体 ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'PingFang SC', Roboto, system-ui, -apple-system, sans-serif;
            background: #f0f2f5;
            color: #1a1a2e;
            padding: 40px 24px;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* ===== 头部 ===== */
        .header {
            text-align: center;
            margin-bottom: 48px;
            max-width: 800px;
        }

        .header h1 {
            font-size: 2.8rem;
            font-weight: 700;
            letter-spacing: -0.5px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: inline-block;
        }

        .header p {
            font-size: 1.1rem;
            color: #555;
            margin-top: 8px;
            font-weight: 400;
            letter-spacing: 0.3px;
        }

        .header .badge {
            display: inline-block;
            margin-top: 12px;
            background: #e8ecf1;
            padding: 6px 20px;
            border-radius: 40px;
            font-size: 0.85rem;
            color: #444;
            font-weight: 500;
        }

        /* ===== 图片网格 ===== */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
            gap: 24px;
            max-width: 1400px;
            width: 100%;
            margin: 0 auto;
        }

        .gallery-item {
            position: relative;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.08);
            background: #fff;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
            aspect-ratio: 1 / 1;
        }

        .gallery-item:hover {
            transform: translateY(-6px);
            box-shadow: 0 16px 48px rgba(0, 0, 0, 0.15);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
            transition: transform 0.5s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.03);
        }

        .gallery-item .overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            padding: 20px 18px 16px;
            background: linear-gradient(transparent, rgba(0, 0, 0, 0.55));
            color: #fff;
            opacity: 0;
            transition: opacity 0.35s ease;
            pointer-events: none;
        }

        .gallery-item:hover .overlay {
            opacity: 1;
        }

        .gallery-item .overlay .title {
            font-size: 1rem;
            font-weight: 600;
            letter-spacing: 0.3px;
        }

        .gallery-item .overlay .sub {
            font-size: 0.8rem;
            opacity: 0.8;
            margin-top: 2px;
        }

        /* ===== 灯箱（Lightbox） ===== */
        .lightbox {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.88);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            z-index: 9999;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            opacity: 0;
            transition: opacity 0.3s ease;
            padding: 24px;
        }

        .lightbox.active {
            display: flex;
            opacity: 1;
        }

        .lightbox .close-btn {
            position: absolute;
            top: 28px;
            right: 36px;
            font-size: 2.6rem;
            color: #fff;
            background: none;
            border: none;
            cursor: pointer;
            transition: transform 0.2s ease, opacity 0.2s ease;
            opacity: 0.7;
            line-height: 1;
            z-index: 10;
        }

        .lightbox .close-btn:hover {
            transform: rotate(90deg);
            opacity: 1;
        }

        .lightbox .lightbox-content {
            position: relative;
            max-width: 90vw;
            max-height: 80vh;
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: 16px;
            overflow: hidden;
            box-shadow: 0 20px 80px rgba(0, 0, 0, 0.6);
            background: #111;
        }

        .lightbox .lightbox-content img {
            width: auto;
            height: auto;
            max-width: 100%;
            max-height: 80vh;
            display: block;
            object-fit: contain;
            border-radius: 16px;
        }

        /* 导航按钮 */
        .lightbox .nav-btn {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(6px);
            -webkit-backdrop-filter: blur(6px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            color: #fff;
            font-size: 2rem;
            width: 56px;
            height: 56px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: background 0.25s ease, transform 0.2s ease;
            z-index: 5;
            user-select: none;
        }

        .lightbox .nav-btn:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-50%) scale(1.05);
        }

        .lightbox .nav-btn.prev {
            left: 20px;
        }
        .lightbox .nav-btn.next {
            right: 20px;
        }

        /* 灯箱底部信息 */
        .lightbox .info {
            position: absolute;
            bottom: 32px;
            left: 50%;
            transform: translateX(-50%);
            color: rgba(255, 255, 255, 0.85);
            font-size: 0.95rem;
            background: rgba(0, 0, 0, 0.4);
            backdrop-filter: blur(6px);
            -webkit-backdrop-filter: blur(6px);
            padding: 10px 28px;
            border-radius: 40px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            text-align: center;
            white-space: nowrap;
            font-weight: 400;
            letter-spacing: 0.3px;
        }

        .lightbox .info span {
            font-weight: 600;
            color: #fff;
        }

        /* ===== 键盘提示（小） ===== */
        .key-hint {
            margin-top: 16px;
            color: rgba(255, 255, 255, 0.35);
            font-size: 0.75rem;
            letter-spacing: 0.5px;
            user-select: none;
        }

        /* ===== 响应式 ===== */
        @media (max-width: 768px) {
            body {
                padding: 24px 16px;
            }
            .header h1 {
                font-size: 2rem;
            }
            .gallery {
                grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
                gap: 14px;
            }
            .lightbox .nav-btn {
                width: 44px;
                height: 44px;
                font-size: 1.4rem;
            }
            .lightbox .nav-btn.prev {
                left: 8px;
            }
            .lightbox .nav-btn.next {
                right: 8px;
            }
            .lightbox .info {
                font-size: 0.8rem;
                padding: 6px 16px;
                bottom: 20px;
                white-space: normal;
            }
            .lightbox .close-btn {
                top: 16px;
                right: 20px;
                font-size: 2rem;
            }
        }

        @media (max-width: 480px) {
            .gallery {
                grid-template-columns: repeat(auto-fill, minmax(130px, 1fr));
                gap: 10px;
            }
            .header h1 {
                font-size: 1.6rem;
            }
        }

        /* ===== 滚动条美化 ===== */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #e8ecf1;
            border-radius: 10px;
        }
        ::-webkit-scrollbar-thumb {
            background: #c0c6d2;
            border-radius: 10px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #a0a8b8;
        }

        /* ===== 加载占位动画 ===== */
        .gallery-item.loading {
            background: #e8ecf1;
            animation: shimmer 1.4s ease-in-out infinite;
        }

        @keyframes shimmer {
            0% {
                background: #e8ecf1;
            }
            50% {
                background: #d5dae3;
            }
            100% {
                background: #e8ecf1;
            }
        }
    </style>
</head>
<body>

    <!-- ===== 头部 ===== -->
    <header class="header">
        <h1>🖼️ 图片展示</h1>
        <p>点击任意图片 · 沉浸式浏览</p>
        <span class="badge">✨ 共 6 张 · 支持键盘导航</span>
    </header>

    <!-- ===== 图片网格 ===== -->
    <div class="gallery" id="gallery"></div>

    <!-- ===== 灯箱 ===== -->
    <div class="lightbox" id="lightbox" role="dialog" aria-modal="true" aria-label="图片预览">
        <button class="close-btn" id="closeBtn" aria-label="关闭预览">&times;</button>

        <div class="lightbox-content" id="lightboxContent">
            <img id="lightboxImg" src="" alt="预览大图" />
            <button class="nav-btn prev" id="prevBtn" aria-label="上一张">‹</button>
            <button class="nav-btn next" id="nextBtn" aria-label="下一张">›</button>
        </div>

        <div class="info" id="lightboxInfo">
            <span id="currentIndex">1</span> / <span id="totalCount">12</span>
            &nbsp;·&nbsp; <span id="imageTitle">图片名称</span>
        </div>

        <div class="key-hint">←  /  →  切换 &nbsp;·&nbsp;  ESC 关闭</div>
    </div>

    <script>
        // ============================================================
        //  数据：图片列表（使用 picsum.photos 占位图，确保每张不同）
        // ============================================================
        const images = [
            { id: 1, title: '🏔️ 1', url: 'https://yy.ms1.asia/lzyzbsl/9/1.webp' },
            { id: 2, title: '🌊 2', url: 'https://yy.ms1.asia/lzyzbsl/9/2.webp' },
            { id: 3, title: '🌲 3', url: 'https://yy.ms1.asia/lzyzbsl/9/3.webp' },
            { id: 4, title: '🌅 4', url: 'https://yy.ms1.asia/lzyzbsl/9/4.webp' },
            { id: 5, title: '🏜️ 5', url: 'https://yy.ms1.asia/lzyzbsl/9/5.webp' },
            { id: 6, title: '🌺 6', url: 'https://yy.ms1.asia/lzyzbsl/9/6.webp' },
           
        ];

        // ============================================================
        //  DOM 引用
        // ============================================================
        const gallery = document.getElementById('gallery');
        const lightbox = document.getElementById('lightbox');
        const lightboxImg = document.getElementById('lightboxImg');
        const closeBtn = document.getElementById('closeBtn');
        const prevBtn = document.getElementById('prevBtn');
        const nextBtn = document.getElementById('nextBtn');
        const currentIndexEl = document.getElementById('currentIndex');
        const totalCountEl = document.getElementById('totalCount');
        const imageTitleEl = document.getElementById('imageTitle');

        let currentIdx = 0;
        const total = images.length;

        // ============================================================
        //  渲染网格
        // ============================================================
        function renderGallery() {
            gallery.innerHTML = '';
            images.forEach((img, index) => {
                const item = document.createElement('div');
                item.className = 'gallery-item loading';
                item.dataset.index = index;

                const imgEl = document.createElement('img');
                imgEl.src = img.url;
                imgEl.alt = img.title;
                imgEl.loading = 'lazy';

                // 图片加载完成后移除 loading 状态
                imgEl.addEventListener('load', () => {
                    item.classList.remove('loading');
                });
                // 如果图片加载失败，也移除 loading（避免永久闪烁）
                imgEl.addEventListener('error', () => {
                    item.classList.remove('loading');
                });

                const overlay = document.createElement('div');
                overlay.className = 'overlay';
                overlay.innerHTML = `
                    <div class="title">${img.title}</div>
                    <div class="sub">点击查看大图</div>
                `;

                item.appendChild(imgEl);
                item.appendChild(overlay);

                // 点击打开灯箱
                item.addEventListener('click', () => {
                    openLightbox(index);
                });

                gallery.appendChild(item);
            });

            totalCountEl.textContent = total;
        }

        // ============================================================
        //  灯箱控制
        // ============================================================
        function openLightbox(index) {
            currentIdx = index;
            updateLightbox();
            lightbox.classList.add('active');
            document.body.style.overflow = 'hidden';
            // 聚焦到灯箱（便于键盘事件）
            lightbox.focus();
        }

        function closeLightbox() {
            lightbox.classList.remove('active');
            document.body.style.overflow = '';
        }

        function goPrev() {
            currentIdx = (currentIdx - 1 + total) % total;
            updateLightbox();
        }

        function goNext() {
            currentIdx = (currentIdx + 1) % total;
            updateLightbox();
        }

        function updateLightbox() {
            const img = images[currentIdx];
            lightboxImg.src = img.url;
            lightboxImg.alt = img.title;
            currentIndexEl.textContent = currentIdx + 1;
            imageTitleEl.textContent = img.title;
        }

        // ============================================================
        //  事件绑定
        // ============================================================
        // 关闭
        closeBtn.addEventListener('click', closeLightbox);

        // 点击灯箱背景关闭（点击内容区不关）
        lightbox.addEventListener('click', (e) => {
            if (e.target === lightbox) {
                closeLightbox();
            }
        });

        // 导航按钮
        prevBtn.addEventListener('click', (e) => {
            e.stopPropagation();
            goPrev();
        });
        nextBtn.addEventListener('click', (e) => {
            e.stopPropagation();
            goNext();
        });

        // 键盘事件
        document.addEventListener('keydown', (e) => {
            if (!lightbox.classList.contains('active')) return;

            switch (e.key) {
                case 'ArrowLeft':
                    e.preventDefault();
                    goPrev();
                    break;
                case 'ArrowRight':
                    e.preventDefault();
                    goNext();
                    break;
                case 'Escape':
                    e.preventDefault();
                    closeLightbox();
                    break;
                default:
                    break;
            }
        });

        // 窗口大小变化时，图片自适应（无额外操作，仅靠 CSS）

        // ============================================================
        //  初始化
        // ============================================================
        renderGallery();

        // 控制台提示
        console.log('🖼️ 图片画廊已加载 — 点击图片浏览，键盘 ← → 切换，ESC 关闭');
    </script>

</body>
</html>