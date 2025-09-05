<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flappy Spaceship</title>
    <style>
        @import url('https://fonts.fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap');

        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #000;
            margin: 0;
            font-family: 'Orbitron', sans-serif;
            color: #fff;
            overflow: hidden;
        }

        #game-container {
            position: relative;
            background: radial-gradient(circle, #0a0a20, #000);
            border: 3px solid #00f;
            box-shadow: 0 0 20px #00f;
            border-radius: 12px;
            overflow: hidden;
        }
        
        canvas {
            display: block;
        }

        .ui-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: rgba(0, 0, 0, 0.7);
            transition: opacity 0.5s ease;
            z-index: 10;
            gap: 20px;
        }

        #start-screen {
            display: flex;
        }

        #score-display {
            position: absolute;
            top: 10px;
            right: 10px;
            font-size: 2em;
            text-shadow: 2px 2px 5px #000;
            z-index: 5;
        }

        #high-score-display {
            position: absolute;
            top: 10px;
            left: 10px;
            font-size: 1.2em;
            text-shadow: 2px 2px 5px #000;
            z-index: 5;
        }
        
        #pause-button {
            position: absolute;
            top: 10px;
            left: 10px;
            background: rgba(0, 0, 0, 0.5);
            color: #00ffff;
            border: 2px solid #00ffff;
            padding: 5px 10px;
            font-size: 1.2em;
            cursor: pointer;
            border-radius: 5px;
            z-index: 5;
            transition: background 0.2s;
        }

        #pause-button:hover {
            background: rgba(0, 0, 0, 0.8);
        }

        h1, h2, h3 {
            margin: 0.5em 0;
            text-shadow: 0 0 10px #00f, 0 0 20px #00f;
        }
        
        button {
            background: linear-gradient(145deg, #00c, #007);
            color: #fff;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            font-family: 'Orbitron', sans-serif;
            cursor: pointer;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 255, 0.5);
            transition: transform 0.2s, box-shadow 0.2s;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin: 10px;
        }

        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 7px 20px rgba(0, 0, 255, 0.7);
        }

        button:active {
            transform: translateY(0);
            box-shadow: 0 5px 15px rgba(0, 0, 255, 0.5);
        }

        .star {
            position: absolute;
            background-color: #fff;
            border-radius: 50%;
            opacity: 0;
            animation: twinkle linear infinite;
        }

        @keyframes twinkle {
            0% { opacity: 0; }
            50% { opacity: 1; transform: scale(1.2); }
            100% { opacity: 0; }
        }

        .message-box {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: rgba(0, 0, 0, 0.9);
            border: 2px solid #00f;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 0 20px #00f;
            z-index: 20;
            display: none;
            text-align: center;
        }
        .message-box p {
            margin: 0 0 10px 0;
        }
        .message-box button {
            margin-top: 10px;
        }

        #speed-control-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            margin-top: 20px;
        }

        #speed-control-container label {
            font-size: 1.2em;
            text-shadow: 0 0 5px #0ff;
        }

        #speed-slider {
            width: 200px;
            -webkit-appearance: none;
            appearance: none;
            height: 8px;
            background: #00c;
            outline: none;
            border-radius: 4px;
            box-shadow: 0 0 5px #00f;
        }

        #speed-slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            appearance: none;
            width: 20px;
            height: 20px;
            background: linear-gradient(45deg, #00ffff, #00ff00);
            border: 2px solid #fff;
            border-radius: 50%;
            cursor: pointer;
            box-shadow: 0 0 10px #00f;
        }
        #speed-value {
            font-size: 1.2em;
            margin-top: -10px;
        }

        #skins-menu-container {
            width: 100%;
            height: 100%;
            overflow-y: auto;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: flex-start;
            gap: 10px;
            padding-top: 20px;
        }

        .skin-button {
            width: 80px;
            height: 80px;
            background: #222;
            border: 2px solid #555;
            border-radius: 8px;
            cursor: pointer;
            display: flex;
            justify-content: center;
            align-items: center;
            transition: transform 0.2s, border-color 0.2s;
            position: relative;
        }

        .skin-button:hover {
            transform: scale(1.1);
            border-color: #00f;
        }

        .skin-button.active {
            border-color: #00ffff;
            box-shadow: 0 0 10px #00ffff;
        }

        .skin-button.locked {
            opacity: 0.5;
            cursor: not-allowed;
        }

        .skin-button.locked::after {
            content: 'LOCKED';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: #fff;
            background: rgba(0, 0, 0, 0.7);
            padding: 5px;
            border-radius: 5px;
            font-size: 0.8em;
        }

        .skin-preview {
            width: 60px;
            height: 60px;
        }
        
        .back-button {
            position: absolute;
            bottom: 20px;
            background: #555;
            border: 2px solid #888;
            padding: 10px 20px;
            font-size: 1em;
            z-index: 11;
        }

        #shop-menu .shop-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 20px;
        }

        #shop-menu .shop-item img {
            width: 100px;
            height: 100px;
            border-radius: 10px;
            border: 2px solid #00f;
            margin-bottom: 10px;
        }

        .currency-display {
            position: absolute;
            top: 10px;
            right: 10px;
            font-size: 1.2em;
            text-shadow: 2px 2px 5px #000;
            z-index: 5;
        }

        #cheat-message {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: rgba(0, 0, 0, 0.8);
            padding: 15px;
            border: 2px solid #00ff00;
            color: #00ff00;
            font-size: 1.5em;
            border-radius: 10px;
            box-shadow: 0 0 20px #00ff00;
            z-index: 100;
            display: none;
            opacity: 0;
            transition: opacity 0.5s ease;
        }
    </style>
</head>
<body>
    <div id="game-container">
        <canvas id="gameCanvas"></canvas>
        <div id="score-display">0</div>
        <div id="high-score-display">High Score: 0</div>
        <div class="currency-display">Points: <span id="point-display">0</span></div>
        <button id="pause-button" style="display: none;">||</button>
        
        <div id="start-screen" class="ui-overlay">
            <h1>Flappy Spaceship</h1>
            <h3 id="start-high-score"></h3>
            <h2>Click or press Space to start!</h2>
            <button id="selectModeButton">Select Mode</button>
            <button id="skinsButton">Skins</button>
            <button id="shopButton">Shop</button>
        </div>

        <div id="mode-selection-menu" class="ui-overlay" style="display: none; opacity: 0;">
            <h1>Select Speed Mode</h1>
            <button id="slowModeButton" data-speed="1.5">Slow</button>
            <button id="normalModeButton" data-speed="2.5">Normal</button>
            <button id="fastModeButton" data-speed="3.5">Fast</button>
            <button id="xGamesModeButton" data-speed="6.0">X Games</button>
            <button class="back-button" id="backFromModeButton">Back</button>
        </div>

        <div id="skins-menu" class="ui-overlay" style="display: none; opacity: 0;">
            <h1>Select Your Ship</h1>
            <div id="skins-menu-container"></div>
            <button class="back-button" id="backFromSkinsButton">Back</button>
        </div>

        <div id="shop-menu" class="ui-overlay" style="display: none; opacity: 0;">
            <h1>Shop</h1>
            <div class="shop-item">
                <button id="buySkinPackButton">Buy Random Skin Pack (50 Points)</button>
                <p id="buy-status"></p>
            </div>
            <button class="back-button" id="backFromShopButton">Back</button>
        </div>

        <div id="game-over-screen" class="ui-overlay" style="display: none; opacity: 0;">
            <h1>Game Over</h1>
            <h2 id="final-score"></h2>
            <h3 id="end-high-score"></h3>
            <button id="restartButton">Restart</button>
        </div>

        <div id="pause-menu" class="ui-overlay" style="display: none; opacity: 0;">
            <h1>Paused</h1>
            <div id="speed-control-container">
                <label for="speed-slider">Pipe Speed</label>
                <input type="range" id="speed-slider" min="1" max="6" value="2.5" step="0.1">
                <div id="speed-value">2.5</div>
            </div>
            <button id="resumeButton">Resume</button>
            <button id="restartFromMenuButton">Restart</button>
        </div>
        <div id="cheat-message" style="display: none; opacity: 0;"></div>
    </div>
    
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const canvas = document.getElementById('gameCanvas');
            const ctx = canvas.getContext('2d');
            const selectModeButton = document.getElementById('selectModeButton');
            const skinsButton = document.getElementById('skinsButton');
            const shopButton = document.getElementById('shopButton');
            const modeSelectionMenu = document.getElementById('mode-selection-menu');
            const skinsMenu = document.getElementById('skins-menu');
            const skinsMenuContainer = document.getElementById('skins-menu-container');
            const shopMenu = document.getElementById('shop-menu');
            const backFromModeButton = document.getElementById('backFromModeButton');
            const backFromSkinsButton = document.getElementById('backFromSkinsButton');
            const backFromShopButton = document.getElementById('backFromShopButton');
            const buySkinPackButton = document.getElementById('buySkinPackButton');
            const buyStatus = document.getElementById('buy-status');
            const slowModeButton = document.getElementById('slowModeButton');
            const normalModeButton = document.getElementById('normalModeButton');
            const fastModeButton = document.getElementById('fastModeButton');
            const xGamesModeButton = document.getElementById('xGamesModeButton');
            const restartButton = document.getElementById('restartButton');
            const restartFromMenuButton = document.getElementById('restartFromMenuButton');
            const startScreen = document.getElementById('start-screen');
            const gameOverScreen = document.getElementById('game-over-screen');
            const scoreDisplay = document.getElementById('score-display');
            const finalScoreDisplay = document.getElementById('final-score');
            const pauseButton = document.getElementById('pause-button');
            const pauseMenu = document.getElementById('pause-menu');
            const resumeButton = document.getElementById('resumeButton');
            const speedSlider = document.getElementById('speed-slider');
            const speedValueDisplay = document.getElementById('speed-value');
            const highScoreDisplay = document.getElementById('high-score-display');
            const startHighScoreDisplay = document.getElementById('start-high-score');
            const endHighScoreDisplay = document.getElementById('end-high-score');
            const pointDisplay = document.getElementById('point-display');
            const cheatMessage = document.getElementById('cheat-message');
            
            let points = parseInt(localStorage.getItem('flappyPoints')) || 0;

            const resizeCanvas = () => {
                const width = Math.min(window.innerWidth * 0.9, 600);
                const height = Math.min(window.innerHeight * 0.8, 800);
                canvas.width = width;
                canvas.height = height;
            };
            window.addEventListener('resize', resizeCanvas);
            resizeCanvas();
            
            const stars = [];
            function createStars() {
                for (let i = 0; i < 100; i++) {
                    const star = document.createElement('div');
                    star.className = 'star';
                    const size = Math.random() * 3 + 1;
                    star.style.width = star.style.height = `${size}px`;
                    star.style.left = `${Math.random() * 100}%`;
                    star.style.top = `${Math.random() * 100}%`;
                    star.style.animationDuration = `${Math.random() * 2 + 1}s`;
                    document.body.appendChild(star);
                    stars.push(star);
                }
            }
            createStars();

            let score = 0;
            let gameMode = 'ready';
            let highScore = localStorage.getItem('flappyHighScore') || 0;
            let ownedSkins = JSON.parse(localStorage.getItem('ownedSkins')) || ['standard'];
            let selectedSkin = localStorage.getItem('selectedSkin') || 'standard';

            const skins = {
                'standard': (ctx) => {
                    ctx.fillStyle = '#00ffff';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                },
                'red_racer': (ctx) => {
                    ctx.fillStyle = '#ff0000';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'gold_knight': (ctx) => {
                    ctx.fillStyle = '#ffc800';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'green_horn': (ctx) => {
                    ctx.fillStyle = '#00ff00';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'purple_prowler': (ctx) => {
                    ctx.fillStyle = '#800080';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'black_ops': (ctx) => {
                    ctx.fillStyle = '#000000';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'silver_streak': (ctx) => {
                    ctx.fillStyle = '#c0c0c0';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'pink_power': (ctx) => {
                    ctx.fillStyle = '#ff69b4';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'orange_blaze': (ctx) => {
                    ctx.fillStyle = '#ff4500';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'cyan_cyclone': (ctx) => {
                    ctx.fillStyle = '#00ffff';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'lime_light': (ctx) => {
                    ctx.fillStyle = '#bfff00';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'maroon_marauder': (ctx) => {
                    ctx.fillStyle = '#800000';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'navy_nomad': (ctx) => {
                    ctx.fillStyle = '#000080';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'teal_tracker': (ctx) => {
                    ctx.fillStyle = '#008080';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'brown_bomber': (ctx) => {
                    ctx.fillStyle = '#a52a2a';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'gray_ghost': (ctx) => {
                    ctx.fillStyle = '#808080';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'indigo_intercept': (ctx) => {
                    ctx.fillStyle = '#4b0082';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'magenta_manta': (ctx) => {
                    ctx.fillStyle = '#ff00ff';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'olive_operator': (ctx) => {
                    ctx.fillStyle = '#808000';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'silver_sentry': (ctx) => {
                    ctx.fillStyle = '#c0c0c0';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                },
                'turquoise_typhoon': (ctx) => {
                    ctx.fillStyle = '#40e0d0';
                    ctx.beginPath();
                    ctx.moveTo(-20, -15);
                    ctx.lineTo(20, 0);
                    ctx.lineTo(-20, 15);
                    ctx.lineTo(-20, -15);
                    ctx.fill();
                    ctx.fillStyle = '#fff';
                    ctx.fillRect(-15, -5, 5, 10);
                }
            };
            
            function updatePointDisplay() {
                pointDisplay.textContent = points;
                localStorage.setItem('flappyPoints', points);
            }

            function showCheatMessage(message) {
                cheatMessage.textContent = message;
                cheatMessage.style.display = 'block';
                setTimeout(() => {
                    cheatMessage.style.opacity = 1;
                }, 10);
                setTimeout(() => {
                    cheatMessage.style.opacity = 0;
                    setTimeout(() => {
                        cheatMessage.style.display = 'none';
                    }, 500);
                }, 2000);
            }

            function buyRandomSkin() {
                const skinPackCost = 50;
                if (points < skinPackCost) {
                    buyStatus.textContent = 'Not enough points!';
                    setTimeout(() => buyStatus.textContent = '', 2000);
                    return;
                }
                
                points -= skinPackCost;
                updatePointDisplay();
                
                const allSkins = Object.keys(skins);
                const randomSkinIndex = Math.floor(Math.random() * allSkins.length);
                const newSkin = allSkins[randomSkinIndex];

                if (!ownedSkins.includes(newSkin)) {
                    ownedSkins.push(newSkin);
                    localStorage.setItem('ownedSkins', JSON.stringify(ownedSkins));
                    buyStatus.textContent = `You got a new skin: ${newSkin.replace('_', ' ').toUpperCase()}!`;
                } else {
                    buyStatus.textContent = `You got a duplicate of: ${newSkin.replace('_', ' ').toUpperCase()}.`;
                }
                
                setTimeout(() => buyStatus.textContent = '', 2000);
            }

            function createSkinButtons() {
                skinsMenuContainer.innerHTML = '';
                Object.keys(skins).forEach(skinName => {
                    const button = document.createElement('div');
                    button.classList.add('skin-button');
                    button.dataset.skin = skinName;
                    
                    const isOwned = ownedSkins.includes(skinName);
                    if (!isOwned) {
                        button.classList.add('locked');
                    } else if (skinName === selectedSkin) {
                        button.classList.add('active');
                    }

                    const canvasSkin = document.createElement('canvas');
                    canvasSkin.width = 60;
                    canvasSkin.height = 60;
                    const ctxSkin = canvasSkin.getContext('2d');
                    ctxSkin.translate(30, 30);
                    skins[skinName](ctxSkin);
                    button.appendChild(canvasSkin);

                    if (isOwned) {
                        button.addEventListener('click', () => {
                            selectedSkin = skinName;
                            localStorage.setItem('selectedSkin', selectedSkin);
                            document.querySelectorAll('.skin-button').forEach(btn => btn.classList.remove('active'));
                            button.classList.add('active');
                        });
                    }

                    skinsMenuContainer.appendChild(button);
                });
            }

            const ship = {
                x: 50,
                y: canvas.height / 2,
                width: 40,
                height: 30,
                velocity: 0,
                gravity: 0.25,
                lift: -6,
                rotation: 0,
                shielded: false,
                shieldTimer: null,
                shieldStartTime: 0,
                draw() {
                    ctx.save();
                    ctx.translate(this.x + this.width / 2, this.y + this.height / 2);
                    
                    if (this.shielded) {
                        const elapsedTime = Date.now() - this.shieldStartTime;
                        const blink = elapsedTime > 5000 && Math.floor(elapsedTime / 100) % 2 === 0;

                        if (!blink) {
                            ctx.beginPath();
                            ctx.arc(0, 0, Math.max(this.width, this.height) * 0.8, 0, Math.PI * 2);
                            ctx.fillStyle = 'rgba(0, 255, 255, 0.3)';
                            ctx.strokeStyle = '#00ffff';
                            ctx.lineWidth = 2;
                            ctx.fill();
                            ctx.stroke();
                        }
                    }

                    ctx.rotate(this.rotation);
                    skins[selectedSkin](ctx);
                    ctx.restore();
                },
                update() {
                    this.velocity += this.gravity;
                    this.y += this.velocity;
                    this.rotation = Math.max(Math.min(this.velocity * 0.05, Math.PI / 2), -Math.PI / 4);

                    if (this.y + this.height > canvas.height) {
                        this.y = canvas.height - this.height;
                        this.velocity = 0;
                        gameOver();
                    }
                    if (this.y < 0) {
                        this.y = 0;
                        this.velocity = 0;
                    }
                },
                flap() {
                    this.velocity = this.lift;
                },
                activateShield() {
                    this.shielded = true;
                    this.shieldStartTime = Date.now();
                    clearTimeout(this.shieldTimer);
                    this.shieldTimer = setTimeout(() => {
                        this.shielded = false;
                    }, 8000);
                }
            };

            let pipes = [];
            let lastPipeHeight = canvas.height / 2;
            const pipeWidth = 60;
            const pipeGap = 200;
            const pipeMinHeight = 50;
            const maxPipeHeightChange = 120;
            let pipeSpeed = 2.5;
            let basePipeSpeed = 2.5;
            const speedStep = 0.1;
            const minSpeed = 1.0;
            const maxSpeed = 6.0;
            let originalPipeSpeed = pipeSpeed;
            let slowMoTimer = null;
            let pipeExplosionTimer = null;

            class Pipe {
                constructor(previousHeight) {
                    this.x = canvas.width;
                    let minHeight = previousHeight - maxPipeHeightChange;
                    let maxHeight = previousHeight + maxPipeHeightChange;
                    
                    minHeight = Math.max(minHeight, pipeMinHeight);
                    maxHeight = Math.min(maxHeight, canvas.height - pipeGap - pipeMinHeight);

                    this.height = Math.random() * (maxHeight - minHeight) + minHeight;
                    lastPipeHeight = this.height;

                    this.passed = false;
                    this.moveDirection = Math.random() < 0.5 ? 'up' : 'down';
                    this.moveLimit = Math.random() * (canvas.height * 0.5) + canvas.height * 0.1;
                }

                draw() {
                    ctx.fillStyle = '#0f0';
                    ctx.fillRect(this.x, 0, pipeWidth, this.height);
                    ctx.fillRect(this.x - 5, this.height, pipeWidth + 10, 20);
                    ctx.fillRect(this.x, this.height + pipeGap, pipeWidth, canvas.height - (this.height + pipeGap));
                    ctx.fillRect(this.x - 5, this.height + pipeGap - 20, pipeWidth + 10, 20);
                }

                update() {
                    this.x -= pipeSpeed;
                    
                    if (this.moveDirection === 'up') {
                        this.height -= 0.5;
                        if (this.height < pipeMinHeight + 5) {
                            this.moveDirection = 'down';
                        }
                    } else if (this.moveDirection === 'down') {
                        this.height += 0.5;
                        if (this.height > canvas.height - pipeGap - pipeMinHeight - 5) {
                            this.moveDirection = 'up';
                        }
                    }
                }
                
                collides(ship) {
                    const topPipeY = this.height;
                    const bottomPipeY = this.height + pipeGap;
                    const shipRight = ship.x + ship.width;
                    const shipBottom = ship.y + ship.height;

                    if (shipRight > this.x && ship.x < this.x + pipeWidth) {
                        if (ship.y < topPipeY || shipBottom > bottomPipeY) {
                            return true;
                        }
                    }
                    return false;
                }
            }

            let powerups = [];
            const powerupSize = 20;

            class Powerup {
                constructor() {
                    this.x = canvas.width + Math.random() * 200;
                    this.y = Math.random() * (canvas.height - powerupSize * 2) + powerupSize;
                    
                    const rand = Math.random();
                    if (rand < 0.6) {
                        this.type = 'slowmo';
                    } else if (rand < 0.9) {
                        this.type = 'explode';
                    } else {
                        this.type = 'hidden';
                    }
                    this.passed = false;
                }

                draw() {
                    ctx.save();
                    ctx.beginPath();
                    if (this.type === 'slowmo') {
                        ctx.fillStyle = '#00ff00';
                        ctx.arc(this.x, this.y, powerupSize, 0, Math.PI * 2);
                        ctx.fill();
                    } else if (this.type === 'explode') {
                        ctx.fillStyle = '#ff0000';
                        ctx.moveTo(this.x, this.y - powerupSize);
                        for (let i = 0; i < 5; i++) {
                            ctx.lineTo(this.x + Math.sin(i * Math.PI * 0.8) * powerupSize * 0.5, this.y + Math.cos(i * Math.PI * 0.8) * powerupSize * 0.5);
                            ctx.lineTo(this.x + Math.sin(i * Math.PI * 0.8 + Math.PI * 0.2) * powerupSize, this.y + Math.cos(i * Math.PI * 0.8 + Math.PI * 0.2) * powerupSize);
                        }
                        ctx.closePath();
                        ctx.fill();
                    } else if (this.type === 'hidden') {
                        ctx.fillStyle = '#ffc800';
                        ctx.moveTo(this.x, this.y - powerupSize);
                        for (let i = 0; i < 5; i++) {
                            ctx.lineTo(this.x + Math.sin(i * Math.PI * 0.8) * powerupSize * 0.5, this.y + Math.cos(i * Math.PI * 0.8) * powerupSize * 0.5);
                            ctx.lineTo(this.x + Math.sin(i * Math.PI * 0.8 + Math.PI * 0.2) * powerupSize, this.y + Math.cos(i * Math.PI * 0.8 + Math.PI * 0.2) * powerupSize);
                        }
                        ctx.closePath();
                        ctx.fill();
                    }
                    ctx.restore();
                }

                update() {
                    this.x -= pipeSpeed;
                }
                
                collides(ship) {
                    const dx = this.x - (ship.x + ship.width / 2);
                    const dy = this.y - (ship.y + ship.height / 2);
                    const distance = Math.sqrt(dx * dx + dy * dy);
                    return distance < powerupSize + Math.max(ship.width, ship.height) / 2;
                }
            }
            
            function gameLoop() {
                if (gameMode !== 'playing') {
                    return;
                }

                ctx.clearRect(0, 0, canvas.width, canvas.height);

                if (pipeExplosionTimer > 0) {
                    pipeExplosionTimer--;
                }
                
                if (!pipeExplosionTimer && (pipes.length === 0 || pipes[pipes.length - 1].x < canvas.width - 250)) {
                    pipes.push(new Pipe(lastPipeHeight));
                    if (Math.random() < 0.2) {
                        powerups.push(new Powerup());
                    }
                }

                for (let i = pipes.length - 1; i >= 0; i--) {
                    const pipe = pipes[i];
                    pipe.update();
                    pipe.draw();

                    if (!ship.shielded && pipe.collides(ship)) {
                        gameOver();
                        return;
                    }

                    if (pipe.x + pipeWidth < ship.x && !pipe.passed) {
                        pipe.passed = true;
                        score++;
                        scoreDisplay.textContent = score;
                    }

                    if (pipe.x < -pipeWidth) {
                        pipes.splice(i, 1);
                    }
                }
                
                for (let i = powerups.length - 1; i >= 0; i--) {
                    const powerup = powerups[i];
                    powerup.update();
                    powerup.draw();

                    if (powerup.collides(ship)) {
                        if (powerup.type === 'hidden') {
                            ship.activateShield();
                        } else if (powerup.type === 'slowmo') {
                            pipeSpeed = originalPipeSpeed / 2;
                            clearTimeout(slowMoTimer);
                            slowMoTimer = setTimeout(() => {
                                pipeSpeed = originalPipeSpeed;
                            }, 5000);
                        } else if (powerup.type === 'explode') {
                            pipes = [];
                            pipeExplosionTimer = 7 * 60;
                            score += 5;
                            scoreDisplay.textContent = score;
                        }
                        powerups.splice(i, 1);
                    }

                    if (powerup.x < -powerupSize) {
                        powerups.splice(i, 1);
                    }
                }

                ship.update();
                ship.draw();

                requestAnimationFrame(gameLoop);
            }

            function updateSpeedValue() {
                speedValueDisplay.textContent = parseFloat(speedSlider.value).toFixed(1);
            }

            speedSlider.addEventListener('input', () => {
                pipeSpeed = parseFloat(speedSlider.value);
                originalPipeSpeed = pipeSpeed;
                updateSpeedValue();
            });

            function updateHighScoreDisplay() {
                highScoreDisplay.textContent = `High Score: ${highScore}`;
                startHighScoreDisplay.textContent = `High Score: ${highScore}`;
                endHighScoreDisplay.textContent = `High Score: ${highScore}`;
            }

            function startGame() {
                gameMode = 'playing';
                score = 0;
                scoreDisplay.textContent = score;
                pipes = [];
                powerups = [];
                ship.y = canvas.height / 2;
                ship.velocity = 0;
                ship.shielded = false;
                clearTimeout(ship.shieldTimer);
                clearTimeout(slowMoTimer);
                
                lastPipeHeight = canvas.height / 2;
                pipeSpeed = basePipeSpeed;
                originalPipeSpeed = pipeSpeed;
                speedSlider.value = basePipeSpeed;
                updateSpeedValue();

                pipeExplosionTimer = null;

                startScreen.style.opacity = 0;
                startScreen.style.pointerEvents = 'none';
                modeSelectionMenu.style.opacity = 0;
                modeSelectionMenu.style.pointerEvents = 'none';
                shopMenu.style.opacity = 0;
                shopMenu.style.pointerEvents = 'none';
                skinsMenu.style.opacity = 0;
                skinsMenu.style.pointerEvents = 'none';
                gameOverScreen.style.opacity = 0;
                gameOverScreen.style.pointerEvents = 'none';
                pauseMenu.style.opacity = 0;
                pauseMenu.style.pointerEvents = 'none';
                pauseButton.style.display = 'block';

                updateHighScoreDisplay();
                updatePointDisplay();
                requestAnimationFrame(gameLoop);
            }

            function gameOver() {
                gameMode = 'gameOver';
                finalScoreDisplay.textContent = `Score: ${score}`;
                pauseButton.style.display = 'none';
                if (score > highScore) {
                    highScore = score;
                    localStorage.setItem('flappyHighScore', highScore);
                }
                points += score;
                updateHighScoreDisplay();
                updatePointDisplay();
                gameOverScreen.style.display = 'flex';
                setTimeout(() => {
                    gameOverScreen.style.opacity = 1;
                    gameOverScreen.style.pointerEvents = 'auto';
                }, 100);
            }

            function pauseGame() {
                gameMode = 'paused';
                pauseMenu.style.display = 'flex';
                setTimeout(() => {
                    pauseMenu.style.opacity = 1;
                    pauseMenu.style.pointerEvents = 'auto';
                }, 100);
            }

            function resumeGame() {
                gameMode = 'playing';
                pauseMenu.style.opacity = 0;
                pauseMenu.style.pointerEvents = 'none';
                requestAnimationFrame(gameLoop);
            }

            function restartGame() {
                pauseMenu.style.opacity = 0;
                pauseMenu.style.pointerEvents = 'none';
                gameOverScreen.style.opacity = 0;
                gameOverScreen.style.pointerEvents = 'none';
                startScreen.style.display = 'flex';
                setTimeout(() => {
                    startScreen.style.opacity = 1;
                    startScreen.style.pointerEvents = 'auto';
                }, 100);
                gameMode = 'ready';
            }

            function showMenu(menu) {
                const allMenus = [startScreen, modeSelectionMenu, skinsMenu, shopMenu, gameOverScreen, pauseMenu];
                allMenus.forEach(m => {
                    m.style.opacity = 0;
                    m.style.pointerEvents = 'none';
                });
                menu.style.display = 'flex';
                setTimeout(() => {
                    menu.style.opacity = 1;
                    menu.style.pointerEvents = 'auto';
                }, 100);
            }

            function goBackToStartScreen() {
                showMenu(startScreen);
            }

            function showModeSelectionMenu() {
                showMenu(modeSelectionMenu);
            }

            function showSkinsMenu() {
                createSkinButtons();
                showMenu(skinsMenu);
            }

            function showShopMenu() {
                showMenu(shopMenu);
            }

            function selectModeAndStart(event) {
                basePipeSpeed = parseFloat(event.target.dataset.speed);
                startGame();
            }

            // Event Listeners
            selectModeButton.addEventListener('click', showModeSelectionMenu);
            skinsButton.addEventListener('click', showSkinsMenu);
            shopButton.addEventListener('click', showShopMenu);
            buySkinPackButton.addEventListener('click', buyRandomSkin);
            
            backFromModeButton.addEventListener('click', goBackToStartScreen);
            backFromSkinsButton.addEventListener('click', goBackToStartScreen);
            backFromShopButton.addEventListener('click', goBackToStartScreen);
            
            slowModeButton.addEventListener('click', selectModeAndStart);
            normalModeButton.addEventListener('click', selectModeAndStart);
            fastModeButton.addEventListener('click', selectModeAndStart);
            xGamesModeButton.addEventListener('click', selectModeAndStart);

            restartButton.addEventListener('click', restartGame);
            restartFromMenuButton.addEventListener('click', restartGame);
            pauseButton.addEventListener('click', pauseGame);
            resumeButton.addEventListener('click', resumeGame);

            let cheatCode = '';
            const unlockCheatSequence = 'gay';
            const removeCheatSequence = 'art';

            document.addEventListener('keydown', (e) => {
                if (gameMode === 'playing') {
                    if (e.code === 'Space') {
                        ship.flap();
                    } else if (e.code === 'Escape') {
                        pauseGame();
                    }
                } else if (gameMode === 'ready') {
                    if (e.code === 'Space') {
                        showModeSelectionMenu();
                    }
                } else if (gameMode === 'gameOver') {
                    if (e.code === 'Space') {
                        restartGame();
                    }
                } else if (gameMode === 'paused') {
                    if (e.code === 'Space' || e.code === 'Escape') {
                        resumeGame();
                    }
                }
                
                if (gameMode === 'playing' || gameMode === 'paused') {
                    if (e.code === 'ArrowUp') {
                        speedSlider.value = Math.min(parseFloat(speedSlider.value) + speedStep, maxSpeed).toFixed(1);
                        pipeSpeed = parseFloat(speedSlider.value);
                        originalPipeSpeed = pipeSpeed;
                        updateSpeedValue();
                    } else if (e.code === 'ArrowDown') {
                        speedSlider.value = Math.max(parseFloat(speedSlider.value) - speedStep, minSpeed).toFixed(1);
                        pipeSpeed = parseFloat(speedSlider.value);
                        originalPipeSpeed = pipeSpeed;
                        updateSpeedValue();
                    }
                }

                if (e.key) {
                    cheatCode += e.key.toLowerCase();
                    if (cheatCode.length > Math.max(unlockCheatSequence.length, removeCheatSequence.length)) {
                        cheatCode = cheatCode.slice(-Math.max(unlockCheatSequence.length, removeCheatSequence.length));
                    }

                    if (cheatCode.includes(unlockCheatSequence)) {
                        ownedSkins = Object.keys(skins);
                        localStorage.setItem('ownedSkins', JSON.stringify(ownedSkins));
                        showCheatMessage("ALL SKINS UNLOCKED!");
                        cheatCode = '';
                    } else if (cheatCode.includes(removeCheatSequence)) {
                        ownedSkins = ['standard'];
                        selectedSkin = 'standard';
                        localStorage.setItem('ownedSkins', JSON.stringify(ownedSkins));
                        localStorage.setItem('selectedSkin', selectedSkin);
                        showCheatMessage("ALL SKINS REMOVED!");
                        cheatCode = '';
                    }
                }
            });

            document.addEventListener('mousedown', (e) => {
                if (e.target.closest('#gameCanvas') && gameMode === 'playing') {
                    ship.flap();
                } else if (gameMode === 'ready' && e.target.id === 'game-container') {
                    showModeSelectionMenu();
                }
            });
            
            document.addEventListener('touchstart', (e) => {
                if (e.target.closest('#gameCanvas') && gameMode === 'playing') {
                    ship.flap();
                } else if (gameMode === 'ready' && e.target.id === 'game-container') {
                    showModeSelectionMenu();
                }
            });

            ctx.fillStyle = '#111';
            ctx.fillRect(0, 0, canvas.width, canvas.height);
            updateSpeedValue();
            updateHighScoreDisplay();
            updatePointDisplay();
        });
    </script>
</body>
</html>
