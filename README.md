# <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gaming Hub</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#111;
    color:white;
}

header{
    background:#1a1a1a;
    padding:20px;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    font-size:28px;
    color:#00ff99;
    font-weight:bold;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:20px;
}

.hero{
    text-align:center;
    padding:80px 20px;
    background:linear-gradient(to right,#00ff99,#0066ff);
}

.hero h1{
    font-size:50px;
}

.hero p{
    margin-top:10px;
    font-size:20px;
}

.games{
    padding:40px;
}

.games h2{
    text-align:center;
    margin-bottom:30px;
}

.game-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.game-card{
    background:#222;
    padding:20px;
    border-radius:10px;
    text-align:center;
    transition:0.3s;
}

.game-card:hover{
    transform:scale(1.05);
}

button{
    margin-top:10px;
    padding:10px 20px;
    background:#00ff99;
    border:none;
    border-radius:5px;
    cursor:pointer;
    font-weight:bold;
}

footer{
    text-align:center;
    padding:20px;
    background:#1a1a1a;
    margin-top:40px;
}
</style>
</head>
<body>

<header>
    <div class="logo">Gaming Hub</div>
    <nav>
        <a href="#">Home</a>
        <a href="#">Games</a>
        <a href="#">Leaderboard</a>
        <a href="#">Contact</a>
    </nav>
</header>

<section class="hero">
    <h1>Welcome to Gaming Hub</h1>
    <p>Play amazing games online for free!</p>
</section>

<section class="games">
    <h2>Featured Games</h2>

    <div class="game-grid">

        <div class="game-card">
            <h3>Snake Game</h3>
            <p>Classic snake adventure.</p>
            <button onclick="playGame('Snake Game')">
                Play Now
            </button>
        </div>

        <div class="game-card">
            <h3>Space Shooter</h3>
            <p>Defeat enemy spaceships.</p>
            <button onclick="playGame('Space Shooter')">
                Play Now
            </button>
        </div>

        <div class="game-card">
            <h3>Racing Pro</h3>
            <p>Race against opponents.</p>
            <button onclick="playGame('Racing Pro')">
                Play Now
            </button>
        </div>

    </div>
</section>

<footer>
    © 2026 Gaming Hub. All Rights Reserved.
</footer>

<script>
function playGame(gameName){
    alert("Launching " + gameName + "...");
}
</script>

</body>
</html>
