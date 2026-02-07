<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Propose Day Kusum 💌</title>

<style>
body{
    margin:0;
    font-family:Arial, sans-serif;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background:linear-gradient(135deg,#ff9a9e,#fecfef);
    text-align:center;
}

.container{
    background:white;
    padding:40px;
    border-radius:20px;
    width:330px;
    box-shadow:0 10px 25px rgba(0,0,0,0.2);
}

h1{ color:#ff4d6d; }

.name{
    font-size:22px;
    font-weight:bold;
    color:#ff4d6d;
}

button{
    padding:10px 20px;
    margin:10px;
    border:none;
    border-radius:10px;
    cursor:pointer;
    font-size:16px;
}

.yes{ background:#ff4d6d; color:white; }
.no{ background:#ddd; }

#letter{
    display:none;
    margin-top:20px;
    font-size:15px;
}

.heart{
    font-size:42px;
    animation:beat 1s infinite;
}

@keyframes beat{
    0%{transform:scale(1);}
    50%{transform:scale(1.25);}
    100%{transform:scale(1);}
}
</style>
</head>

<body>

<div class="container">

    <h1>Happy Propose Day 💌</h1>
    <div class="name">Kusum ❤️</div>

    <p id="question">Will you be mine?</p>

    <button class="yes" onclick="sayYes()">Yes ❤️</button>
    <button class="no" onclick="sayNo()">No 🙈</button>

    <div id="letter">
        <div class="heart">❤️ 👫 ❤️</div>
        <p>
        Dear Kusum,<br><br>
        You make my days happier and my smile brighter.  
        Being with you feels special and peaceful.  
        I just want to stay by your side and make beautiful memories together.<br><br>
        Will you be mine forever? 💖
        </p>
    </div>

</div>

<script>

// 🔥 Different pickup lines
const lines = [
"Heyy 😝 My heart only goes forward… it doesn't understand NO!",
"Are you magic? Because my world changes when you smile ✨",
"I think you clicked the wrong button… try YES ❤️",
"My heart already selected YES for you 😌",
"Error 404: NO option not found 😆",
"You can't escape, destiny says YES only 💘",
"Even Google can't find someone better than you 😉",
"Stop pressing NO… you're already mine ❤️"
];

function sayNo(){
    let random = lines[Math.floor(Math.random() * lines.length)];
    alert(random);
}

function sayYes(){
    document.getElementById("question").style.display="none";
    document.querySelector(".yes").style.display="none";
    document.querySelector(".no").style.display="none";
    document.getElementById("letter").style.display="block";
}

</script>

</body>
</html>
