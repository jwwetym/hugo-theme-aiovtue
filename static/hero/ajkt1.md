
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
ai: 艾灸非人参般昂贵稀有，却有人参不具备的普惠之德。它以"久火"温阳散寒、通经活络，尤其适合现代人空调冷饮所致的阳虚湿寒体质。其效不在一时神奇，而在日日坚持，平淡中见真章，是贯穿中医治法、安全有效的日常保命良方。
pinned: true
---

<style>
/* ===== 视频播放器样式（添加 .post 或 .content 前缀避免冲突） ===== */
.video-preview-wrapper {
    max-width: 800px;
    width: 100%;
    margin: 30px auto;
    background: #ffffff;
    border-radius: 16px;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
    overflow: hidden;
    border: 1px solid rgba(255, 255, 255, 0.3);
}

.video-window {
    position: relative;
    width: 100%;
    padding-bottom: 56.25%;
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
    object-fit: contain;
    background: #000;
}

.video-center-play-btn {
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
    padding-left: 5px;
    box-shadow: 0 4px 20px rgba(223, 145, 147, 0.4);
    transition: all 0.2s ease;
    pointer-events: none;
    z-index: 10;
    opacity: 0.85;
    backdrop-filter: blur(4px);
    border: 2px solid rgba(255, 255, 255, 0.3);
}

.video-window:hover .video-center-play-btn {
    opacity: 1;
    transform: translate(-50%, -50%) scale(1.05);
}

.video-controls-bar {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 12px 20px;
    background: rgba(30, 30, 30, 0.85);
    backdrop-filter: blur(10px);
    border-top: 1px solid rgba(255, 255, 255, 0.08);
    flex-wrap: wrap;
}

.video-controls-bar button {
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

.video-controls-bar button:hover {
    background: rgba(255, 255, 255, 0.12);
    color: #fff;
}

.video-controls-bar button:active {
    transform: scale(0.95);
}

.video-progress-slider {
    flex: 1;
    min-width: 60px;
    height: 4px;
    -webkit-appearance: none;
    appearance: none;
    background: rgba(255, 255, 255, 0.2);
    border-radius: 4px;
    outline: none;
    cursor: pointer;
}

.video-progress-slider::-webkit-slider-thumb {
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

.video-progress-slider::-webkit-slider-thumb:hover {
    transform: scale(1.15);
}

.video-progress-slider::-moz-range-thumb {
    width: 14px;
    height: 14px;
    border-radius: 50%;
    background: #DF9193;
    border: 2px solid #fff;
    cursor: pointer;
}

.video-time-display {
    color: #ccc;
    font-size: 13px;
    font-variant-numeric: tabular-nums;
    min-width: 100px;
    text-align: center;
    letter-spacing: 0.5px;
}

.video-fullscreen-btn {
    font-size: 18px;
    background: rgba(255, 255, 255, 0.06) !important;
    border-radius: 8px !important;
    padding: 6px 14px !important;
}

.video-fullscreen-btn:hover {
    background: rgba(223, 145, 147, 0.3) !important;
}

.video-preview-wrapper.fullscreen-mode {
    max-width: 100%;
    max-height: 100vh;
    margin: 0;
    border-radius: 0;
    border: none;
    box-shadow: none;
    background: #000;
}

.video-preview-wrapper.fullscreen-mode .video-controls-bar {
    background: rgba(0, 0, 0, 0.7);
}

.video-preview-wrapper.fullscreen-mode .video-window {
    padding-bottom: 0;
    height: calc(100vh - 70px);
}

@media (max-width: 500px) {
    .video-controls-bar {
        padding: 8px 12px;
        gap: 6px;
    }
    .video-controls-bar button {
        font-size: 13px;
        padding: 4px 6px;
    }
    .video-time-display {
        font-size: 11px;
        min-width: 70px;
    }
    .video-center-play-btn {
        width: 50px;
        height: 50px;
        font-size: 22px;
    }
}
</style>

<!-- ===== 视频播放器 HTML 嵌入 ===== -->
<div class="video-preview-wrapper" id="videoPreviewWrapper">
    <div class="video-window" id="videoWindow">
        <video id="myVideo" 
               src="https://yy.ms1.asia/aijiu/1Whatisrealmoxibustion.mp4"
               preload="metadata"
               playsinline
        ></video>
        <div class="video-center-play-btn" id="centerPlayIcon">▶</div>
    </div>

    <div class="video-controls-bar">
        <button id="playBtn" title="播放 / 暂停">
            <span id="playIcon">▶</span> <span id="playText">播放</span>
        </button>

        <input type="range" class="video-progress-slider" id="progressBar" value="0" min="0" max="100" step="0.1" title="拖动进度">

        <span class="video-time-display" id="timeDisplay">00:00 / 00:00</span>

        <button class="video-fullscreen-btn" id="fullscreenBtn" title="全屏预览">
            ⛶ 全屏
        </button>
    </div>
</div>

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

<script>
(function() {
    // 确保 DOM 完全加载后再执行
    if (document.readyState === 'loading') {
        document.addEventListener('DOMContentLoaded', initVideoPlayer);
    } else {
        initVideoPlayer();
    }

    function initVideoPlayer() {
        const video = document.getElementById('myVideo');
        const wrapper = document.getElementById('videoPreviewWrapper');
        const windowDiv = document.getElementById('videoWindow');

        if (!video || !wrapper || !windowDiv) {
            console.warn('视频播放器元素未找到');
            return;
        }

        const playBtn = document.getElementById('playBtn');
        const playIcon = document.getElementById('playIcon');
        const playText = document.getElementById('playText');
        const centerIcon = document.getElementById('centerPlayIcon');
        const progressBar = document.getElementById('progressBar');
        const timeDisplay = document.getElementById('timeDisplay');
        const fullscreenBtn = document.getElementById('fullscreenBtn');

        function formatTime(seconds) {
            if (isNaN(seconds) || !isFinite(seconds)) return '00:00';
            const m = Math.floor(seconds / 60);
            const s = Math.floor(seconds % 60);
            return `${String(m).padStart(2, '0')}:${String(s).padStart(2, '0')}`;
        }

        function updatePlayButton() {
            if (video.paused) {
                playIcon.textContent = '▶';
                playText.textContent = '播放';
                if (centerIcon) centerIcon.textContent = '▶';
            } else {
                playIcon.textContent = '⏸';
                playText.textContent = '暂停';
                if (centerIcon) centerIcon.textContent = '⏸';
            }
        }

        function updateProgressAndTime() {
            if (video.duration > 0 && !isNaN(video.duration)) {
                const percent = (video.currentTime / video.duration) * 100;
                progressBar.value = percent;
                timeDisplay.textContent = `${formatTime(video.currentTime)} / ${formatTime(video.duration)}`;
            }
        }

        function togglePlay() {
            if (video.paused) {
                video.play().catch(err => console.warn('播放失败:', err));
            } else {
                video.pause();
            }
            updatePlayButton();
        }

        // 事件绑定
        playBtn.addEventListener('click', togglePlay);
        windowDiv.addEventListener('click', togglePlay);

        video.addEventListener('play', updatePlayButton);
        video.addEventListener('pause', updatePlayButton);
        video.addEventListener('ended', function() {
            updatePlayButton();
            progressBar.value = 0;
            timeDisplay.textContent = `00:00 / ${formatTime(video.duration)}`;
        });
        video.addEventListener('timeupdate', updateProgressAndTime);

        progressBar.addEventListener('input', function() {
            if (video.duration > 0 && !isNaN(video.duration)) {
                const seekTime = (this.value / 100) * video.duration;
                video.currentTime = seekTime;
                timeDisplay.textContent = `${formatTime(seekTime)} / ${formatTime(video.duration)}`;
            }
        });

        video.addEventListener('loadedmetadata', updateProgressAndTime);
        video.addEventListener('error', function() {
            timeDisplay.textContent = '⚠️ 视频链接无效或网络错误';
        });

        // 全屏功能
        function toggleFullscreen() {
            if (document.fullscreenElement || document.webkitFullscreenElement) {
                if (document.exitFullscreen) {
                    document.exitFullscreen();
                } else if (document.webkitExitFullscreen) {
                    document.webkitExitFullscreen();
                }
                return;
            }

            const element = wrapper;
            if (element.requestFullscreen) {
                element.requestFullscreen();
            } else if (element.webkitRequestFullscreen) {
                element.webkitRequestFullscreen();
            } else {
                alert('您的浏览器不支持全屏 API');
            }
        }

        if (fullscreenBtn) {
            fullscreenBtn.addEventListener('click', toggleFullscreen);
        }

        function onFullscreenChange() {
            const isFull = !!(document.fullscreenElement || document.webkitFullscreenElement);
            if (isFull) {
                wrapper.classList.add('fullscreen-mode');
                if (fullscreenBtn) fullscreenBtn.innerHTML = '⛶ 退出';
            } else {
                wrapper.classList.remove('fullscreen-mode');
                if (fullscreenBtn) fullscreenBtn.innerHTML = '⛶ 全屏';
                wrapper.style.maxWidth = '';
                wrapper.style.maxHeight = '';
            }
        }

        document.addEventListener('fullscreenchange', onFullscreenChange);
        document.addEventListener('webkitfullscreenchange', onFullscreenChange);

        document.addEventListener('keydown', function(e) {
            if (e.target === document.body && e.key === ' ') {
                e.preventDefault();
                togglePlay();
            }
        });

        updatePlayButton();
        updateProgressAndTime();
    }
})();
</script>