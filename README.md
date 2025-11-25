<!DOCTYPE html>
<html lang="mn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Покерын Вэб Аппликейшн (Туршилт Бэлэн)</title>
    <link rel="stylesheet" href="style.css"> 
</head>
<body>
    <div id="poker-table">
        <div id="pot">Нийт Бооцоо: $<span id="pot-amount">0</span></div>
        
        <div id="board-cards">
            </div>

        <div id="players">
            <div class="player my-player" id="player-0">
                <div class="name-tag"><span class="name">Та (Player 1)</span></div>
                <div class="chips-info">Үлдэгдэл: $<span class="chips">0</span></div>
                <div class="bet-info">Бооцоо: $<span class="bet">0</span></div>
                <div class="card-area"></div>
                <div class="status-message"></div>
            </div>
            
            <div class="player opponent-player" id="player-1">
                <div class="name-tag"><span class="name">Player 2</span></div>
                <div class="chips-info">Үлдэгдэл: $<span class="chips">0</span></div>
                <div class="bet-info">Бооцоо: $<span class="bet">0</span></div>
                <div class="card-area"></div>
                <div class="status-message"></div>
            </div>
        </div>

        <div id="action-panel" class="hidden">
            <button id="fold-btn" class="action-btn red">ФОЛТ</button>
            <button id="check-call-btn" class="action-btn green">ЧЕК/КОЛЛ ($0)</button>
            
            <input type="range" id="raise-slider" min="0" max="1000" value="0" step="10">
            <span id="raise-amount-display">$0</span>
            <button id="raise-btn" class="action-btn orange">РЭЙЗ</button>
        </div>
        
        <div id="game-message" class="hidden"></div>
    </div>

    <script src="script.js"></script>
</body>
</html>
