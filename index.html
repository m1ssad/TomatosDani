<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Viewer Attack - Twitch Extension</title>
    <style>
        body {
            background: linear-gradient(135deg, #6441a5, #2a0845);
            color: white;
            font-family: Arial, sans-serif;
            padding: 15px;
            margin: 0;
        }
        
        .items {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            margin-bottom: 15px;
        }
        
        .item {
            background: rgba(255,255,255,0.2);
            padding: 12px;
            text-align: center;
            border-radius: 10px;
            cursor: pointer;
            font-size: 24px;
            transition: transform 0.2s;
        }
        
        .item:hover {
            transform: scale(1.05);
            background: rgba(255,255,255,0.3);
        }
        
        .item.selected {
            background: #9147ff;
            box-shadow: 0 0 15px #9147ff;
        }
        
        button {
            background: #ff4444;
            color: white;
            border: none;
            padding: 15px;
            width: 100%;
            font-size: 20px;
            border-radius: 10px;
            cursor: pointer;
            font-weight: bold;
            transition: transform 0.1s;
        }
        
        button:active {
            transform: scale(0.95);
        }
        
        .stats {
            margin-top: 15px;
            text-align: center;
            font-size: 14px;
            background: rgba(0,0,0,0.5);
            padding: 8px;
            border-radius: 8px;
        }
        
        .cooldown {
            margin-top: 10px;
            text-align: center;
            font-size: 12px;
            color: #ffaa00;
        }
    </style>
</head>
<body>
    <div class="items">
        <div class="item selected" data-item="tomato">🍅 Помидор</div>
        <div class="item" data-item="cake">🎂 Торт</div>
        <div class="item" data-item="egg">🥚 Яйцо</div>
        <div class="item" data-item="shoe">👞 Туфель</div>
    </div>
    
    <button id="attackBtn">КИНУТЬ В СТРИМЕРА!</button>
    
    <div class="stats">
        🎯 Всего атак: <span id="attackCount">0</span>
    </div>
    <div class="cooldown" id="cooldownMsg">✅ Готов к атаке!</div>

    <script>
        let selectedItem = 'tomato';
        let attackCount = 0;
        let lastAttack = 0;
        const COOLDOWN = 3000; // 3 секунды
        
        // Выбор предмета
        document.querySelectorAll('.item').forEach(item => {
            item.onclick = () => {
                document.querySelectorAll('.item').forEach(i => i.classList.remove('selected'));
                item.classList.add('selected');
                selectedItem = item.dataset.item;
            };
        });
        
        // Атака
        document.getElementById('attackBtn').onclick = () => {
            const now = Date.now();
            if (now - lastAttack < COOLDOWN) {
                const wait = Math.ceil((COOLDOWN - (now - lastAttack)) / 1000);
                document.getElementById('cooldownMsg').innerHTML = `⏳ Подожди ${wait} сек...`;
                return;
            }
            
            lastAttack = now;
            attackCount++;
            document.getElementById('attackCount').innerText = attackCount;
            document.getElementById('cooldownMsg').innerHTML = '🍅 ПОМИДОР ЛЕТИТ!';
            
            // Создаём эффект на странице
            showFlyingTomato();
            
            setTimeout(() => {
                document.getElementById('cooldownMsg').innerHTML = '✅ Готов к атаке!';
            }, COOLDOWN);
        };
        
        function showFlyingTomato() {
            // Эффект летящего помидора
            const tomato = document.createElement('div');
            tomato.innerHTML = selectedItem === 'tomato' ? '🍅' :
                              selectedItem === 'cake' ? '🎂' :
                              selectedItem === 'egg' ? '🥚' : '👞';
            tomato.style.position = 'fixed';
            tomato.style.bottom = '20px';
            tomato.style.right = '20px';
            tomato.style.fontSize = '60px';
            tomato.style.zIndex = '999999';
            tomato.style.animation = 'fly 1s ease-out forwards';
            tomato.style.pointerEvents = 'none';
            document.body.appendChild(tomato);
            
            setTimeout(() => tomato.remove(), 1000);
        }
        
        // Добавляем анимацию
        const style = document.createElement('style');
        style.textContent = `
            @keyframes fly {
                0% {
                    transform: translate(0, 0) rotate(0deg);
                    opacity: 1;
                }
                100% {
                    transform: translate(-200px, -300px) rotate(360deg);
                    opacity: 0;
                }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
