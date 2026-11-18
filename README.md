# Saloniii
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Princess Day - Saloni</title>
<style>
*{box-sizing:border-box}
body{
 margin:0;min-height:100vh;display:flex;justify-content:center;
 align-items:center;padding:20px;
 background:linear-gradient(135deg,#ffd6e7,#e9d5ff,#fff0d6);
 font-family:Georgia,serif;color:#713d5a;text-align:center
}
.card{
 width:100%;max-width:600px;background:#ffffffed;
 padding:35px 22px;border-radius:28px;
 box-shadow:0 12px 40px #9b668344
}
h1{color:#d34f89;font-size:35px}
p{font-size:18px;line-height:1.8}
.emoji{font-size:55px}
button{
 border:0;border-radius:30px;padding:14px 24px;
 background:#d65391;color:white;font-size:16px;
 margin:10px;cursor:pointer
}
.page{display:none}
.page.active{display:block}
.note{
 background:#fff2f8;padding:20px;border-radius:18px;
 line-height:1.8;margin:20px 0
}
</style>
</head>
<body>
<div class="card">

<section class="page active" id="page1">
<div class="emoji">👑💗</div>
<h1>Happy Princess Day Saloni!</h1>
<p>Welcome to your little surprise, Princess.</p>
<p>Today is all about you and your beautiful smile!</p>
<button onclick="next(2)">Open My Surprise 💌</button>
</section>

<section class="page" id="page2">
<div class="emoji">🌸🦋</div>
<h1>My Beautiful Princess</h1>
<p>Saloni, you make ordinary moments feel special. Keep smiling, keep dreaming and always believe in yourself.</p>
<div class="note">You deserve happiness, love and beautiful memories. 💕</div>
<button onclick="next(1)">Back</button>
<button onclick="next(3)">Next ❤️</button>
</section>

<section class="page" id="page3">
<div class="emoji">🌙✨</div>
<h1>A Little Wish For You</h1>
<p>May your life always be full of happiness, laughter and success. Never stop being the wonderful person you are.</p>
<div class="emoji">💗🌷💗</div>
<button onclick="next(2)">Back</button>
<button onclick="next(4)">Last Surprise 💌</button>
</section>

<section class="page" id="page4">
<div class="emoji">💌</div>
<h1>Dear Saloni</h1>
<div class="note">
Happy Princess Day! ❤️<br><br>
I made this little website just for you.
I hope it brings a smile to your face.
Always stay happy, follow your dreams
and never forget how special you are.
You deserve all the beautiful things in life.<br><br>
With lots of love and wishes,<br>
<strong>Your Ankit 💗</strong>
</div>
<button onclick="next(1)">Read Again ↻</button>
</section>

</div>

<script>
function next(n){
 document.querySelectorAll('.page').forEach(function(p){
  p.classList.remove('active');
 });
 document.getElementById('page'+n).classList.add('active');
}
</script>
</body>
</html>
