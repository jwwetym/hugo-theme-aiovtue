---
title: "1什么是真正的艾灸？"
description: "艾灸系列课"
date: 2026-08-25
lastmod: 2026-08-25
cover: "https://yy.ms1.asia/aijiu/1Whatisrealmoxibustion.jpg"
categories:
  - 艾灸课堂
tags:
  - 艾灸课堂
ai: 艾灸非人参般昂贵稀有，却有人参不具备的普惠之德。它以“久火”温阳散寒、通经活络，尤其适合现代人空调冷饮所致的阳虚湿寒体质。其效不在一时神奇，而在日日坚持，平淡中见真章，是贯穿中医治法、安全有效的日常保命良方。
pinned: true
---

<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>视频预览窗口（带全屏）</title>
    <style>
        /* 全局重置与居中 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #f0f2f5;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            font-family: 'Segoe UI', 'PingFang SC', Roboto, sans-serif;
        }

        /* ===== 预览窗口容器（核心约束） ===== */
        .preview-wrapper {
            max-width: 800px;          /* 最大宽度约束，不会撑爆屏幕 */
            width: 100%;
            margin: 0 20px;
            background: #ffffff;
            border-radius: 16px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
            overflow: hidden;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.3);
            backdrop-filter: blur(2px);
        }

        /* ===== 视频窗口（16:9 比例约束） ===== */
        .video-window {
            position: relative;
            width: 100%;
            padding-bottom: 56.25%;      /* 16:9 宽高比 */
            background: #000000;
            cursor: pointer;
            background-color: #1a1a1a;
        }

        .video-window video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            display: block;
            object-fit: contain;         /* 保持比例，不裁剪画面（黑边填充） */
            background: #000;
        }

        /* ===== 中央大播放按钮（预览风格） ===== */
        .center-play-btn {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 70px;
            height: 70px;
            background: rgba(223, 145, 147, 0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #fff;
            font-size: 30px;
            padding-left: 5px; /* 让播放三角形居中 */
            box-shadow: 0 4px 20px rgba(223, 145, 147, 0.4);
            transition: all 0.2s ease;
            pointer-events: none; /* 点击穿透，由video元素接管点击 */
            z-index: 10;
            opacity: 0.85;
            backdrop-filter: blur(4px);
            border: 2px solid rgba(255, 255, 255, 0.3);
        }

        .video-window:hover .center-play-btn {
            opacity: 1;
            transform: translate(-50%, -50%) scale(1.05);
        }

        /* ===== 自定义控制栏（位于窗口底部） ===== */
        .controls-bar {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 12px 20px;
            background: rgba(30, 30, 30, 0.85);
            backdrop-filter: blur(10px);
            border-top: 1px solid rgba(255, 255, 255, 0.08);
            flex-wrap: wrap;
        }

        .controls-bar button {
            background: transparent;
            border: none;
            color: #eee;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            padding: 6px 10px;
            border-radius: 6px;
            transition: all 0.2s;
            display: flex;
            align-items: center;
            gap: 4px;
            white-space: nowrap;
        }

        .controls-bar button:hover {
            background: rgba(255, 255, 255, 0.12);
            color: #fff;
        }

        .controls-bar button:active {
            transform: scale(0.95);
        }

        /* 进度条 */
        .progress-slider {
            flex: 1;
            min-width: 60px;
            height: 4px;
            -webkit-appearance: none;
            appearance: none;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 4px;
            outline: none;
            transition: height 0.2s;
            cursor: pointer;
        }

        .progress-slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            appearance: none;
            width: 14px;
            height: 14px;
            border-radius: 50%;
            background: #DF9193;
            border: 2px solid #fff;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
            transition: 0.1s;
        }

        .progress-slider::-webkit-slider-thumb:hover {
            transform: scale(1.15);
        }

        .progress-slider::-moz-range-thumb {
            width: 14px;
            height: 14px;
            border-radius: 50%;
            background: #DF9193;
            border: 2px solid #fff;
            cursor: pointer;
        }

        .time-display {
            color: #ccc;
            font-size: 13px;
            font-variant-numeric: tabular-nums;
            min-width: 100px;
            text-align: center;
            letter-spacing: 0.5px;
        }

        /* 全屏按钮特殊样式 */
        .fullscreen-btn {
            font-size: 18px;
            background: rgba(255, 255, 255, 0.06) !important;
            border-radius: 8px !important;
            padding: 6px 14px !important;
        }
        .fullscreen-btn:hover {
            background: rgba(223, 145, 147, 0.3) !important;
        }

        /* ===== 全屏模式下的样式适配 ===== */
        .preview-wrapper.fullscreen-mode {
            max-width: 100%;
            max-height: 100vh;
            margin: 0;
            border-radius: 0;
            border: none;
            box-shadow: none;
            background: #000;
        }

        .preview-wrapper.fullscreen-mode .controls-bar {
            background: rgba(0, 0, 0, 0.7);
        }

        .preview-wrapper.fullscreen-mode .video-window {
            padding-bottom: 0; /* 全屏时让视频自适应填满 */
            height: calc(100vh - 70px); /* 减去控制栏高度 */
        }

        /* 响应式微调 */
        @media (max-width: 500px) {
            .controls-bar {
                padding: 8px 12px;
                gap: 6px;
            }
            .controls-bar button {
                font-size: 13px;
                padding: 4px 6px;
            }
            .time-display {
                font-size: 11px;
                min-width: 70px;
            }
            .center-play-btn {
                width: 50px;
                height: 50px;
                font-size: 22px;
            }
        }
    </style>
</head>
<body>

<div class="preview-wrapper" id="previewWrapper">
    <!-- 视频预览窗口 -->
    <div class="video-window" id="videoWindow">
        <video id="myVideo" 
               src="https://yy.ms1.asia/aijiu/1Whatisrealmoxibustion.mp4"
               preload="metadata"
               playsinline
        ></video>
        <!-- 中央悬浮播放按钮（纯装饰 + 交互提示） -->
        <div class="center-play-btn" id="centerPlayIcon">▶</div>
    </div>

    <!-- 自定义控制栏 -->
    <div class="controls-bar">
        <button id="playBtn" title="播放 / 暂停">
            <span id="playIcon">▶</span> <span id="playText">播放</span>
        </button>

        <input type="range" class="progress-slider" id="progressBar" value="0" min="0" max="100" step="0.1" title="拖动进度">

        <span class="time-display" id="timeDisplay">00:00 / 00:00</span>

        <button class="fullscreen-btn" id="fullscreenBtn" title="全屏预览">
            ⛶ 全屏
        </button>
    </div>
</div>

<script>
    (function() {
        const video = document.getElementById('myVideo');
        const wrapper = document.getElementById('previewWrapper');
        const windowDiv = document.getElementById('videoWindow');

        const playBtn = document.getElementById('playBtn');
        const playIcon = document.getElementById('playIcon');
        const playText = document.getElementById('playText');
        const centerIcon = document.getElementById('centerPlayIcon');
        const progressBar = document.getElementById('progressBar');
        const timeDisplay = document.getElementById('timeDisplay');
        const fullscreenBtn = document.getElementById('fullscreenBtn');

        // ---------- 辅助函数 ----------
        function formatTime(seconds) {
            if (isNaN(seconds)) return '00:00';
            const m = Math.floor(seconds / 60);
            const s = Math.floor(seconds % 60);
            return `${String(m).padStart(2, '0')}:${String(s).padStart(2, '0')}`;
        }

        function updatePlayButton() {
            if (video.paused) {
                playIcon.textContent = '▶';
                playText.textContent = '播放';
                centerIcon.textContent = '▶';
            } else {
                playIcon.textContent = '⏸';
                playText.textContent = '暂停';
                centerIcon.textContent = '⏸';
            }
        }

        function updateProgressAndTime() {
            if (video.duration > 0 && !isNaN(video.duration)) {
                const percent = (video.currentTime / video.duration) * 100;
                progressBar.value = percent;
                timeDisplay.textContent = `${formatTime(video.currentTime)} / ${formatTime(video.duration)}`;
            } else {
                timeDisplay.textContent = '00:00 / 00:00';
            }
        }

        // ---------- 核心交互 ----------
        // 1. 播放/暂停切换（按钮 + 点击视频）
        function togglePlay() {
            if (video.paused) {
                video.play().catch(err => {
                    // 自动播放被阻止或网络错误时忽略
                    console.warn('播放失败:', err);
                });
            } else {
                video.pause();
            }
            // 状态由事件驱动更新，但为了即时反馈也调用一次
            updatePlayButton();
        }

        playBtn.addEventListener('click', togglePlay);
        windowDiv.addEventListener('click', togglePlay); // 点击视频画面切换

        // 2. 视频事件监听（同步状态）
        video.addEventListener('play', () => {
            updatePlayButton();
        });
        video.addEventListener('pause', () => {
            updatePlayButton();
        });
        video.addEventListener('ended', () => {
            updatePlayButton();
            progressBar.value = 0;
            timeDisplay.textContent = `00:00 / ${formatTime(video.duration)}`;
        });

        video.addEventListener('timeupdate', () => {
            updateProgressAndTime();
        });

        // 3. 进度条拖动
        progressBar.addEventListener('input', function() {
            if (video.duration > 0 && !isNaN(video.duration)) {
                const seekTime = (this.value / 100) * video.duration;
                video.currentTime = seekTime;
                // 拖动时更新时间显示
                timeDisplay.textContent = `${formatTime(seekTime)} / ${formatTime(video.duration)}`;
            }
        });

        // 4. 加载元数据后更新进度条总时长
        video.addEventListener('loadedmetadata', () => {
            updateProgressAndTime();
        });

        // 处理视频加载失败
        video.addEventListener('error', () => {
            timeDisplay.textContent = '⚠️ 视频链接无效或网络错误';
            console.error('视频加载失败');
        });

        // ---------- 全屏功能（核心需求） ----------
        function toggleFullscreen() {
            // 如果当前已经是全屏状态，则退出
            if (document.fullscreenElement || document.webkitFullscreenElement) {
                if (document.exitFullscreen) {
                    document.exitFullscreen();
                } else if (document.webkitExitFullscreen) {
                    document.webkitExitFullscreen();
                }
                return;
            }

            // 否则让预览窗口进入全屏
            const element = wrapper;
            if (element.requestFullscreen) {
                element.requestFullscreen();
            } else if (element.webkitRequestFullscreen) {
                element.webkitRequestFullscreen();
            } else {
                alert('您的浏览器不支持全屏 API，请尝试使用 Chrome/Edge/Firefox 最新版。');
            }
        }

        fullscreenBtn.addEventListener('click', toggleFullscreen);

        // 监听全屏变化事件，切换样式和按钮文字
        function onFullscreenChange() {
            const isFull = !!(document.fullscreenElement || document.webkitFullscreenElement);
            if (isFull) {
                wrapper.classList.add('fullscreen-mode');
                fullscreenBtn.innerHTML = '⛶ 退出';
            } else {
                wrapper.classList.remove('fullscreen-mode');
                fullscreenBtn.innerHTML = '⛶ 全屏';
                // 退出全屏后，恢复窗口约束样式
                wrapper.style.maxWidth = '';
                wrapper.style.maxHeight = '';
            }
            // 重新调整视频尺寸（触发浏览器重绘）
            setTimeout(() => {
                window.dispatchEvent(new Event('resize'));
            }, 100);
        }

        document.addEventListener('fullscreenchange', onFullscreenChange);
        document.addEventListener('webkitfullscreenchange', onFullscreenChange);

        // 键盘快捷键：空格键切换播放（可选）
        document.addEventListener('keydown', (e) => {
            if (e.target === document.body && e.key === ' ') {
                e.preventDefault();
                togglePlay();
            }
        });

        // 初始化显示
        updatePlayButton();
        updateProgressAndTime();

        console.log('✅ 预览播放器已启动，点击视频或按钮播放，点击“全屏”放大预览。');
    })();
</script>
</body>
</html>



  今天和大家聊一个更年期心脏病的案子。这个案子的患者49岁，女性，更年期阶段，主诉一大堆——月经乱、心悸胸闷、乳腺胀痛、小腹痛、脸上瘀斑、烘热汗出、手脚凉、睡不好、胃口差。更年期的常见症状她几乎占全了。

如果按照常规思路，烘热汗出、舌尖郁热，是不是很容易想到阴虚火旺、清热滋阴？但这位医家的诊断非常独特，他抓住的是脉象——右手脉浮取微浮、沉取细紧滞弱，命门脉火弱，尺脉不足；左手脉同样沉取细滞紧，尺弱。舌象是两边齿痕、胃区横纹，舌根略腻厚。

这个信息告诉我们什么？表面是烘热，底下是阳虚精亏、虚阳上浮。那点火是飘在上面的虚火，真正的根在下焦，是坎中真阳不够了、精血亏了，兜不住这团火。

所以治法不是清热，是引火归元、益肾填精。把下焦的炉子烧旺，浮在上面的虚火自然就下来了。

这个案子的精彩之处，在于治疗的**五个步骤**，每一步的换挡都很清晰。

### 第一步
不治心，先治神。方子是硃茯神法镇八方。用硃茯神、琥珀安神定志，让君主之官先稳下来。然后用砂仁、藿香、青皮、厚朴疏通气机，白芷、天麻化浊息风，九香虫、瓦楞子降逆制酸，党参、鹿角片填补下元。这一诊的核心，是从无形的神入手，气机一通，有形的心脏症状自然松动。

### 第二步
开表建中。方子换成桂枝二陈法。用桂枝拨动太阳、透达少阴，把表打开，给邪气一条出路。白术运脾，小茴香理肝脾，陈皮半夏厚朴降胃逆，硃茯神分清浊。表一开、中一运，病人就能承接收后面的温补药了。

### 第三步
表里同温。用附子桂枝法，制附片壮先天元阳，桂枝通心阳，白术炙甘草运脾，再加上瓜蒌壳、薤白宽胸开膈，吴茱萸、茵陈温肝降胆，党参鹿角片阿胶填精。到了这一步，才真正开始处理心脏的胸闷胀痛。

### 第四步
透邪通络。用川乌法，川乌这个药是附子之母，阴阳未分之物，专门破阴阳凝对、透达深层瘀滞。配合黄芪通冲脉，红参阿胶养阴，半夏郁金硃茯神解郁安神，鹿角片水牛角通督清神，锁阳紫石英温藏下元。这一步处理的是更深层的络脉瘀堵和神志郁结。

### 第五步
收功固本。用附子肉桂法，加党参黄芪丹参补气活血，银杏叶红景天宽胸通窍，鹿角片龟板通任督、填精髓。这个方子要坚持三个月，目的是把根基彻底稳住。

病人吃到第五方10剂的时候，几乎所有症状都消失了。但医家说，至少还要坚持三个月，因为脸上黑斑还没完全退，根基还没牢。

这个案子的启示是什么？面对更年期的心脏问题，不要一上来就活血化瘀、清热滋阴。先看根在哪。根在少阴精亏、坎阳不足，就老老实实从下焦入手。五个方子，从治神到开表到建中到温通到填精，步步为营，次第不乱。这就是中医治慢病的程序性思维。

如果你身边也有更年期被烘热汗出、心悸失眠困扰的朋友，不妨把这个案子转给ta看看。很多时候，烘热不是火太旺，是底下的炉子快灭了。
