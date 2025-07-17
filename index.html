<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>ジャンプゲーム</title>
  <style>
    canvas {
      background: #eef;
      display: block;
      margin: 0 auto;
    }
  </style>
</head>
<body>
<canvas id="gameCanvas" width="800" height="400"></canvas>

<script>
  const canvas = document.getElementById("gameCanvas");
  const ctx = canvas.getContext("2d");

  let player = { x: 100, y: 300, width: 50, height: 50, vy: 0, gravity: 0.8, jumpPower: -15, onGround: true };
  let obstacle = { x: 800, y: 310, width: 40, height: 40, speed: 5 };
  let score = 0;
  let gameOver = false;

  document.addEventListener("keydown", e => {
    if (e.code === "Space" && player.onGround) {
      player.vy = player.jumpPower;
      player.onGround = false;
    }
  });

  function resetObstacle() {
    obstacle.x = canvas.width + Math.random() * 300;
  }

  function gameLoop() {
    if (gameOver) return;

    // 更新
    player.vy += player.gravity;
    player.y += player.vy;

    if (player.y + player.height >= 350) {
      player.y = 350 - player.height;
      player.vy = 0;
      player.onGround = true;
    }

    obstacle.x -= obstacle.speed;
    if (obstacle.x + obstacle.width < 0) {
      resetObstacle();
      score++;
    }

    // 衝突判定
    if (
      player.x < obstacle.x + obstacle.width &&
      player.x + player.width > obstacle.x &&
      player.y < obstacle.y + obstacle.height &&
      player.y + player.height > obstacle.y
    ) {
      gameOver = true;
    }

    // 描画
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    // プレイヤー
    ctx.fillStyle = "blue";
    ctx.fillRect(player.x, player.y, player.width, player.height);

    // 障害物
    ctx.fillStyle = "red";
    ctx.fillRect(obstacle.x, obstacle.y, obstacle.width, obstacle.height);

    // 地面
    ctx.fillStyle = "black";
    ctx.fillRect(0, 350, canvas.width, 5);

    // スコア
    ctx.fillStyle = "black";
    ctx.font = "24px sans-serif";
    ctx.fillText("Score: " + score, 10, 30);

    if (!gameOver) requestAnimationFrame(gameLoop);
    else {
      ctx.fillStyle = "black";
      ctx.fillText("Game Over", canvas.width / 2 - 60, canvas.height / 2);
    }
  }

  gameLoop();
</script>
</body>
</html>