---
title: "第十集"
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
<a href="https://yy.ms1.asia/lzyzbsl/10/10.mp4" target="_blank" rel="noopener" style="display:inline-block; background:#DF9193; color:#fff; padding:10px 24px; border-radius:8px; text-decoration:none; font-weight:bold; margin:20px 0;">
    ▶ 点击播放视频
</a>

<style>
    /* ===== 全局重置 ===== */
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    .gallery-wrapper {
        font-family: 'Segoe UI', 'PingFang SC', Roboto, system-ui, sans-serif;
        background: #f0f2f5;
        color: #1a1a2e;
        padding: 40px 24px;
        max-width: 1400px;
        margin: 0 auto;
        border-radius: 20px;
    }

    .header {
        text-align: center;
        margin-bottom: 48px;
    }

    .header h1 {
        font-size: 2.8rem;
        font-weight: 700;
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
    }

    .header .badge {
        display: inline-block;
        margin-top: 12px;
        background: #e8ecf1;
        padding: 6px 20px;
        border-radius: 40px;
        font-size: 0.85rem;
        color: #444;
    }

    .gallery {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
        gap: 24px;
        width: 100%;
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
    }

    /* ===== 灯箱 ===== */
    .lightbox {
        display: none;
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.88);
        backdrop-filter: blur(10px);
        z-index: 9999;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        padding: 24px;
    }

    .lightbox.active {
        display: flex;
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
        opacity: 0.7;
        z-index: 10;
    }

    .lightbox .close-btn:hover {
        opacity: 1;
        transform: rotate(90deg);
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
        background: #111;
    }

    .lightbox .lightbox-content img {
        max-width: 100%;
        max-height: 80vh;
        object-fit: contain;
        border-radius: 16px;
    }

    .lightbox .nav-btn {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        background: rgba(255, 255, 255, 0.15);
        backdrop-filter: blur(6px);
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
        z-index: 5;
        user-select: none;
    }

    .lightbox .nav-btn:hover {
        background: rgba(255, 255, 255, 0.3);
    }

    .lightbox .nav-btn.prev {
        left: 20px;
    }
    .lightbox .nav-btn.next {
        right: 20px;
    }

    .lightbox .info {
        position: absolute;
        bottom: 32px;
        left: 50%;
        transform: translateX(-50%);
        color: rgba(255, 255, 255, 0.85);
        background: rgba(0, 0, 0, 0.4);
        backdrop-filter: blur(6px);
        padding: 10px 28px;
        border-radius: 40px;
        border: 1px solid rgba(255, 255, 255, 0.1);
        text-align: center;
        white-space: nowrap;
        font-size: 0.95rem;
    }

    .lightbox .info span {
        font-weight: 600;
        color: #fff;
    }

    .key-hint {
        margin-top: 16px;
        color: rgba(255, 255, 255, 0.35);
        font-size: 0.75rem;
        user-select: none;
    }

    @media (max-width: 768px) {
        .gallery {
            grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
            gap: 14px;
        }
        .header h1 {
            font-size: 2rem;
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

<div class="gallery-wrapper">
    <header class="header">
        <h1>🖼️ 图片画廊 · 第十集</h1>
        <p>点击任意图片 · 沉浸式浏览</p>
        <span class="badge">✨ 共 6 张 · 支持键盘导航</span>
    </header>

    <div class="gallery" id="gallery"></div>
</div>

<!-- ===== 灯箱 ===== -->
<div class="lightbox" id="lightbox" role="dialog" aria-modal="true" aria-label="图片预览">
    <button class="close-btn" id="closeBtn" aria-label="关闭预览">&times;</button>
    <div class="lightbox-content" id="lightboxContent">
        <img id="lightboxImg" src="" alt="预览大图" />
        <button class="nav-btn prev" id="prevBtn" aria-label="上一张">‹</button>
        <button class="nav-btn next" id="nextBtn" aria-label="下一张">›</button>
    </div>
    <div class="info" id="lightboxInfo">
        <span id="currentIndex">1</span> / <span id="totalCountInfo">6</span>
        &nbsp;·&nbsp; <span id="imageTitle">图片名称</span>
    </div>
    <div class="key-hint">←  /  →  切换 &nbsp;·&nbsp;  ESC 关闭</div>
</div>

<script>
    // ============================================================
    //  第十集 6 张图片（保留你的原始地址）
    // ============================================================
    const images = [
        { id: 1, title: '🏔️ 1', url: 'https://yy.ms1.asia/lzyzbsl/10/1.webp' },
        { id: 2, title: '🌊 2', url: 'https://yy.ms1.asia/lzyzbsl/10/2.webp' },
        { id: 3, title: '🌲 3', url: 'https://yy.ms1.asia/lzyzbsl/10/3.webp' },
        { id: 4, title: '🌅 4', url: 'https://yy.ms1.asia/lzyzbsl/10/4.webp' },
        { id: 5, title: '🏜️ 5', url: 'https://yy.ms1.asia/lzyzbsl/10/5.webp' },
        { id: 6, title: '🌺 6', url: 'https://yy.ms1.asia/lzyzbsl/10/6.webp' },
    ];

    // ============================================================
    //  备用占位图（原图加载失败时自动替换）
    // ============================================================
    function getFallbackUrl(id) {
        return `https://picsum.photos/seed/${id}/600/600`;
    }

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
    const totalCountInfo = document.getElementById('totalCountInfo');
    const imageTitleEl = document.getElementById('imageTitle');

    let currentIdx = 0;
    const total = images.length;
    totalCountInfo.textContent = total;

    // ============================================================
    //  渲染网格
    // ============================================================
    function renderGallery() {
        gallery.innerHTML = '';
        images.forEach((img, index) => {
            const item = document.createElement('div');
            item.className = 'gallery-item loading';

            const imgEl = document.createElement('img');
            imgEl.src = img.url;
            imgEl.alt = img.title;
            imgEl.loading = 'lazy';

            // 加载失败 → 自动切换为备用占位图
            imgEl.addEventListener('error', function onError() {
                this.removeEventListener('error', onError);
                this.src = getFallbackUrl(img.id || index);
            });

            imgEl.addEventListener('load', () => {
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

            item.addEventListener('click', () => {
                openLightbox(index);
            });

            gallery.appendChild(item);
        });
    }

    // ============================================================
    //  灯箱控制
    // ============================================================
    function openLightbox(index) {
        currentIdx = index;
        updateLightbox();
        lightbox.classList.add('active');
        document.body.style.overflow = 'hidden';
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
        // 大图也加 fallback
        lightboxImg.onerror = function() {
            this.onerror = null;
            this.src = getFallbackUrl(img.id || currentIdx);
        };
        currentIndexEl.textContent = currentIdx + 1;
        imageTitleEl.textContent = img.title;
    }

    // ============================================================
    //  事件绑定
    // ============================================================
    closeBtn.addEventListener('click', closeLightbox);

    lightbox.addEventListener('click', (e) => {
        if (e.target === lightbox) {
            closeLightbox();
        }
    });

    prevBtn.addEventListener('click', (e) => {
        e.stopPropagation();
        goPrev();
    });

    nextBtn.addEventListener('click', (e) => {
        e.stopPropagation();
        goNext();
    });

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
        }
    });

    // ============================================================
    //  启动
    // ============================================================
    renderGallery();
</script>