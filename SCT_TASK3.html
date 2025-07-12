<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>4K Advanced Tic-Tac-Toe</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #e74c3c;
            --background-color: #f8f9fa;
            --grid-color: #2c3e50;
            --hover-color: rgba(52, 152, 219, 0.2);
            --win-color: #27ae60;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--background-color);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            color: #333;
        }

        .container {
            width: 100%;
            max-width: 800px;
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            position: relative;
        }

        .header {
            background-color: var(--primary-color);
            color: white;
            padding: 20px;
            text-align: center;
            position: relative;
        }

        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 5px;
        }

        .header p {
            font-size: 1rem;
            opacity: 0.9;
        }

        .game-controls {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
            background-color: #f1f2f6;
            border-bottom: 1px solid #e3e6f0;
        }

        .mode-selector {
            display: flex;
            align-items: center;
        }

        .mode-selector label {
            margin-right: 10px;
            font-weight: 600;
        }

        .mode-selector select {
            padding: 8px 15px;
            border-radius: 5px;
            border: 1px solid #ddd;
            background-color: white;
            font-family: inherit;
            font-size: 0.9rem;
        }

        .difficulty-selector {
            display: flex;
            align-items: center;
            margin-left: 20px;
        }

        .difficulty-selector label {
            margin-right: 10px;
            font-weight: 600;
        }

        .btn {
            padding: 8px 16px;
            border: none;
            border-radius: 5px;
            background-color: var(--primary-color);
            color: white;
            font-family: inherit;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            justify-content: center;
        }

        .btn i {
            margin-right: 8px;
        }

        .btn:hover {
            background-color: #2980b9;
            transform: translateY(-2px);
        }

        .btn-reset {
            background-color: #95a5a6;
        }

        .btn-reset:hover {
            background-color: #7f8c8d;
        }

        .game-info {
            display: flex;
            justify-content: space-between;
            padding: 15px 20px;
            background-color: white;
            border-bottom: 1px solid #e3e6f0;
        }

        .player-info {
            display: flex;
            align-items: center;
        }

        .player-x {
            color: var(--primary-color);
            font-weight: 600;
            margin-right: 20px;
        }

        .player-o {
            color: var(--secondary-color);
            font-weight: 600;
        }

        .current-player {
            padding: 5px 10px;
            border-radius: 5px;
            font-weight: 700;
        }

        .current-player.x {
            background-color: rgba(52, 152, 219, 0.2);
            color: var(--primary-color);
        }

        .current-player.o {
            background-color: rgba(231, 76, 60, 0.2);
            color: var(--secondary-color);
        }

        .game-status {
            font-weight: 600;
            color: var(--grid-color);
        }

        .game-board {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
            padding: 20px;
            background-color: white;
            aspect-ratio: 1/1;
            max-width: 500px;
            margin: 0 auto;
        }

        .cell {
            background-color: white;
            border: 2px solid var(--grid-color);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            font-weight: 700;
            cursor: pointer;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .cell:hover {
            background-color: var(--hover-color);
        }

        .cell.x {
            color: var(--primary-color);
        }

        .cell.o {
            color: var(--secondary-color);
        }

        .cell.win {
            background-color: rgba(39, 174, 96, 0.2);
            border-color: var(--win-color);
        }

        .cell::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: radial-gradient(circle, transparent 30%, rgba(0, 0, 0, 0.05) 100%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .cell:hover::before {
            opacity: 1;
        }

        .notification {
            position: fixed;
            top: 20px;
            right: 20px;
            padding: 15px 20px;
            border-radius: 5px;
            background-color: white;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transform: translateX(150%);
            transition: transform 0.3s ease;
            z-index: 1000;
            display: flex;
            align-items: center;
        }

        .notification.show {
            transform: translateX(0);
        }

        .notification.success {
            border-left: 4px solid var(--win-color);
        }

        .notification.info {
            border-left: 4px solid var(--primary-color);
        }

        .notification i {
            margin-right: 10px;
            font-size: 1.2rem;
        }

        .notification.success i {
            color: var(--win-color);
        }

        .notification.info i {
            color: var(--primary-color);
        }

        .game-over-modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 1000;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }

        .game-over-modal.show {
            opacity: 1;
            visibility: visible;
        }

        .modal-content {
            background-color: white;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            max-width: 400px;
            width: 90%;
            transform: scale(0.8);
            transition: transform 0.3s ease;
        }

        .game-over-modal.show .modal-content {
            transform: scale(1);
        }

        .modal-title {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: var(--grid-color);
        }

        .modal-message {
            font-size: 1.2rem;
            margin-bottom: 25px;
            color: #555;
        }

        .modal-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
        }

        .stats {
            padding: 20px;
            background-color: #f8f9fa;
            border-top: 1px solid #e3e6f0;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
        }

        .stat-box {
            background-color: white;
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
        }

        .stat-value {
            font-size: 1.8rem;
            font-weight: 700;
            margin-bottom: 5px;
        }

        .stat-label {
            font-size: 0.9rem;
            color: #777;
        }

        .x-stat .stat-value {
            color: var(--primary-color);
        }

        .o-stat .stat-value {
            color: var(--secondary-color);
        }

        .draw-stat .stat-value {
            color: #7f8c8d;
        }

        @media (max-width: 600px) {
            .header h1 {
                font-size: 1.8rem;
            }
            
            .game-controls {
                flex-direction: column;
                gap: 15px;
            }
            
            .mode-selector, .difficulty-selector {
                width: 100%;
                justify-content: space-between;
            }
            
            .game-board {
                gap: 5px;
                padding: 10px;
            }
            
            .cell {
                font-size: 2rem;
            }
        }

        /* Animation for winning cells */
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        .cell.win {
            animation: pulse 0.6s ease-in-out;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>4K Tic-Tac-Toe</h1>
            <p>The ultimate strategic game</p>
        </div>
        
        <div class="game-controls">
            <div class="mode-selector">
                <label for="game-mode">Game Mode:</label>
                <select id="game-mode">
                    <option value="pvp">Player vs Player</option>
                    <option value="pvc">Player vs Computer</option>
                </select>
                
                <div class="difficulty-selector" id="difficulty-container" style="display: none;">
                    <label for="difficulty">Difficulty:</label>
                    <select id="difficulty">
                        <option value="easy">Easy</option>
                        <option value="medium">Medium</option>
                        <option value="hard">Hard</option>
                    </select>
                </div>
            </div>
            
            <button class="btn btn-reset" id="reset-game">
                <i class="fas fa-redo-alt"></i> Reset Game
            </button>
        </div>
        
        <div class="game-info">
            <div>
                <span class="player-info">
                    <span class="player-x">Player X</span>
                    <span class="current-player x" id="player-x-indicator">Current Turn</span>
                </span>
                <span class="player-info">
                    <span class="player-o">Player O</span>
                    <span class="current-player o" id="player-o-indicator" style="display: none;">Current Turn</span>
                </span>
            </div>
            <div class="game-status" id="game-status">Game in progress...</div>
        </div>
        
        <div class="game-board" id="game-board">
            <div class="cell" data-index="0"></div>
            <div class="cell" data-index="1"></div>
            <div class="cell" data-index="2"></div>
            <div class="cell" data-index="3"></div>
            <div class="cell" data-index="4"></div>
            <div class="cell" data-index="5"></div>
            <div class="cell" data-index="6"></div>
            <div class="cell" data-index="7"></div>
            <div class="cell" data-index="8"></div>
        </div>
        
        <div class="stats">
            <div class="stats-grid">
                <div class="stat-box x-stat">
                    <div class="stat-value" id="x-wins">0</div>
                    <div class="stat-label">Player X Wins</div>
                </div>
                <div class="stat-box o-stat">
                    <div class="stat-value" id="o-wins">0</div>
                    <div class="stat-label">Player O Wins</div>
                </div>
                <div class="stat-box draw-stat">
                    <div class="stat-value" id="draws">0</div>
                    <div class="stat-label">Draws</div>
                </div>
                <div class="stat-box">
                    <div class="stat-value" id="total-games">0</div>
                    <div class="stat-label">Total Games</div>
                </div>
            </div>
        </div>
    </div>
    
    <div class="notification" id="notification">
        <i class="fas fa-info-circle"></i>
        <span id="notification-message"></span>
    </div>
    
    <div class="game-over-modal" id="game-over-modal">
        <div class="modal-content">
            <h2 class="modal-title" id="modal-title">Game Over</h2>
            <p class="modal-message" id="modal-message">Player X wins!</p>
            <div class="modal-buttons">
                <button class="btn" id="play-again-btn">
                    <i class="fas fa-play"></i> Play Again
                </button>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // Game elements
            const gameBoard = document.getElementById('game-board');
            const cells = document.querySelectorAll('.cell');
            const gameModeSelect = document.getElementById('game-mode');
            const difficultySelect = document.getElementById('difficulty');
            const difficultyContainer = document.getElementById('difficulty-container');
            const resetGameBtn = document.getElementById('reset-game');
            const playerXIndicator = document.getElementById('player-x-indicator');
            const playerOIndicator = document.getElementById('player-o-indicator');
            const gameStatus = document.getElementById('game-status');
            const notification = document.getElementById('notification');
            const notificationMessage = document.getElementById('notification-message');
            const gameOverModal = document.getElementById('game-over-modal');
            const modalTitle = document.getElementById('modal-title');
            const modalMessage = document.getElementById('modal-message');
            const playAgainBtn = document.getElementById('play-again-btn');
            
            // Stats elements
            const xWinsElement = document.getElementById('x-wins');
            const oWinsElement = document.getElementById('o-wins');
            const drawsElement = document.getElementById('draws');
            const totalGamesElement = document.getElementById('total-games');
            
            // Game state
            let currentPlayer = 'X';
            let gameBoardState = ['', '', '', '', '', '', '', '', ''];
            let gameActive = true;
            let gameMode = 'pvp'; // 'pvp' or 'pvc'
            let difficulty = 'easy';
            let stats = {
                xWins: 0,
                oWins: 0,
                draws: 0,
                totalGames: 0
            };
            
            // Winning combinations
            const winningCombinations = [
                [0, 1, 2], [3, 4, 5], [6, 7, 8], // Rows
                [0, 3, 6], [1, 4, 7], [2, 5, 8], // Columns
                [0, 4, 8], [2, 4, 6]             // Diagonals
            ];
            
            // Initialize the game
            function initGame() {
                gameBoardState = ['', '', '', '', '', '', '', '', ''];
                gameActive = true;
                currentPlayer = 'X';
                
                // Reset UI
                cells.forEach(cell => {
                    cell.textContent = '';
                    cell.classList.remove('x', 'o', 'win');
                });
                
                updateGameStatus('Game in progress...');
                updatePlayerIndicator();
            }
            
            // Handle cell click
            function handleCellClick(e) {
                const cell = e.target;
                const index = parseInt(cell.getAttribute('data-index'));
                
                // Check if cell is already filled or game is not active
                if (gameBoardState[index] !== '' || !gameActive) {
                    return;
                }
                
                // Update the game state
                makeMove(index);
                
                // If game is still active and in PVC mode, make computer move
                if (gameActive && gameMode === 'pvc' && currentPlayer === 'O') {
                    setTimeout(() => {
                        makeComputerMove();
                    }, 500);
                }
            }
            
            // Make a move
            function makeMove(index) {
                gameBoardState[index] = currentPlayer;
                cells[index].textContent = currentPlayer;
                cells[index].classList.add(currentPlayer.toLowerCase());
                
                // Check for win or draw
                if (checkWin()) {
                    endGame(false);
                } else if (checkDraw()) {
                    endGame(true);
                } else {
                    // Switch player
                    currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
                    updatePlayerIndicator();
                }
            }
            
            // Check for win - FIXED FUNCTION
            function checkWin() {
                for (const combination of winningCombinations) {
                    const [a, b, c] = combination;
                    if (gameBoardState[a] && 
                        gameBoardState[a] === gameBoardState[b] && 
                        gameBoardState[a] === gameBoardState[c]) {
                        
                        // Highlight winning cells
                        cells[a].classList.add('win');
                        cells[b].classList.add('win');
                        cells[c].classList.add('win');
                        
                        return true;
                    }
                }
                return false;
            }
            
            // Check for draw
            function checkDraw() {
                return !gameBoardState.includes('');
            }
            
            // End the game
            function endGame(isDraw) {
                gameActive = false;
                
                if (isDraw) {
                    updateGameStatus('Game ended in a draw!');
                    showNotification('Game ended in a draw!', 'info');
                    stats.draws++;
                    modalTitle.textContent = 'Game Over';
                    modalMessage.textContent = 'The game ended in a draw!';
                } else {
                    updateGameStatus(`Player ${currentPlayer} wins!`);
                    showNotification(`Player ${currentPlayer} wins!`, 'success');
                    
                    if (currentPlayer === 'X') {
                        stats.xWins++;
                    } else {
                        stats.oWins++;
                    }
                    
                    modalTitle.textContent = 'Winner!';
                    modalMessage.textContent = `Player ${currentPlayer} wins!`;
                }
                
                stats.totalGames++;
                updateStats();
                showModal();
            }
            
            // Computer move
            function makeComputerMove() {
                if (!gameActive) return;
                
                let index;
                
                switch (difficulty) {
                    case 'easy':
                        index = makeRandomMove();
                        break;
                    case 'medium':
                        index = makeMediumMove();
                        break;
                    case 'hard':
                        index = makeHardMove();
                        break;
                    default:
                        index = makeRandomMove();
                }
                
                makeMove(index);
            }
            
            // Easy difficulty: Random move
            function makeRandomMove() {
                const availableMoves = [];
                
                for (let i = 0; i < gameBoardState.length; i++) {
                    if (gameBoardState[i] === '') {
                        availableMoves.push(i);
                    }
                }
                
                const randomIndex = Math.floor(Math.random() * availableMoves.length);
                return availableMoves[randomIndex];
            }
            
            // Medium difficulty: Try to win, then block, then random
            function makeMediumMove() {
                // Try to win
                for (let i = 0; i < gameBoardState.length; i++) {
                    if (gameBoardState[i] === '') {
                        gameBoardState[i] = 'O';
                        if (checkWin()) {
                            gameBoardState[i] = '';
                            return i;
                        }
                        gameBoardState[i] = '';
                    }
                }
                
                // Try to block
                for (let i = 0; i < gameBoardState.length; i++) {
                    if (gameBoardState[i] === '') {
                        gameBoardState[i] = 'X';
                        if (checkWin()) {
                            gameBoardState[i] = '';
                            return i;
                        }
                        gameBoardState[i] = '';
                    }
                }
                
                // Make random move
                return makeRandomMove();
            }
            
            // Hard difficulty: Minimax algorithm
            function makeHardMove() {
                // First try to win
                for (let i = 0; i < gameBoardState.length; i++) {
                    if (gameBoardState[i] === '') {
                        gameBoardState[i] = 'O';
                        if (checkWin()) {
                            gameBoardState[i] = '';
                            return i;
                        }
                        gameBoardState[i] = '';
                    }
                }
                
                // Use minimax for best move
                let bestScore = -Infinity;
                let bestMove;
                
                for (let i = 0; i < gameBoardState.length; i++) {
                    if (gameBoardState[i] === '') {
                        gameBoardState[i] = 'O';
                        let score = minimax(gameBoardState, 0, false);
                        gameBoardState[i] = '';
                        
                        if (score > bestScore) {
                            bestScore = score;
                            bestMove = i;
                        }
                    }
                }
                
                return bestMove;
            }
            
            // Minimax algorithm for AI
            function minimax(board, depth, isMaximizing) {
                // Check for terminal states
                if (checkWinForMinimax(board, 'O')) {
                    return 10 - depth;
                }
                
                if (checkWinForMinimax(board, 'X')) {
                    return depth - 10;
                }
                
                if (!board.includes('')) {
                    return 0;
                }
                
                if (isMaximizing) {
                    let bestScore = -Infinity;
                    
                    for (let i = 0; i < board.length; i++) {
                        if (board[i] === '') {
                            board[i] = 'O';
                            let score = minimax(board, depth + 1, false);
                            board[i] = '';
                            bestScore = Math.max(score, bestScore);
                        }
                    }
                    
                    return bestScore;
                } else {
                    let bestScore = Infinity;
                    
                    for (let i = 0; i < board.length; i++) {
                        if (board[i] === '') {
                            board[i] = 'X';
                            let score = minimax(board, depth + 1, true);
                            board[i] = '';
                            bestScore = Math.min(score, bestScore);
                        }
                    }
                    
                    return bestScore;
                }
            }
            
            // Helper function for minimax
            function checkWinForMinimax(board, player) {
                for (const combination of winningCombinations) {
                    const [a, b, c] = combination;
                    if (board[a] === player && 
                        board[a] === board[b] && 
                        board[a] === board[c]) {
                        return true;
                    }
                }
                return false;
            }
            
            // Update game status
            function updateGameStatus(message) {
                gameStatus.textContent = message;
            }
            
            // Update player indicator
            function updatePlayerIndicator() {
                if (currentPlayer === 'X') {
                    playerXIndicator.style.display = 'inline-block';
                    playerOIndicator.style.display = 'none';
                } else {
                    playerXIndicator.style.display = 'none';
                    playerOIndicator.style.display = 'inline-block';
                }
            }
            
            // Show notification
            function showNotification(message, type) {
                notificationMessage.textContent = message;
                notification.className = 'notification';
                notification.classList.add(type);
                notification.classList.add('show');
                
                setTimeout(() => {
                    notification.classList.remove('show');
                }, 3000);
            }
            
            // Update stats
            function updateStats() {
                xWinsElement.textContent = stats.xWins;
                oWinsElement.textContent = stats.oWins;
                drawsElement.textContent = stats.draws;
                totalGamesElement.textContent = stats.totalGames;
            }
            
            // Show game over modal
            function showModal() {
                gameOverModal.classList.add('show');
            }
            
            // Hide game over modal
            function hideModal() {
                gameOverModal.classList.remove('show');
            }
            
            // Event listeners
            cells.forEach(cell => {
                cell.addEventListener('click', handleCellClick);
            });
            
            resetGameBtn.addEventListener('click', () => {
                initGame();
                showNotification('Game has been reset', 'info');
            });
            
            gameModeSelect.addEventListener('change', () => {
                gameMode = gameModeSelect.value;
                difficultyContainer.style.display = gameMode === 'pvc' ? 'flex' : 'none';
                
                if (gameMode === 'pvc') {
                    showNotification('Switched to Player vs Computer mode', 'info');
                } else {
                    showNotification('Switched to Player vs Player mode', 'info');
                }
                
                initGame();
            });
            
            difficultySelect.addEventListener('change', () => {
                difficulty = difficultySelect.value;
                showNotification(`Difficulty set to ${difficulty}`, 'info');
            });
            
            playAgainBtn.addEventListener('click', () => {
                hideModal();
                initGame();
            });
            
            // Initialize the game
            initGame();
        });
    </script>
</body>
</html>
