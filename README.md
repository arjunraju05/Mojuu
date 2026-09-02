<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Press When You Miss Me ❤️</title>

<style>
body{
    margin:0;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background:linear-gradient(135deg,#ff758c,#ff7eb3);
    font-family:Arial,sans-serif;
    text-align:center;
    color:white;
}

.container{
    padding:30px;
    max-width:700px;
}

h1{
    font-size:3rem;
}

button{
    margin-top:30px;
    padding:20px 40px;
    font-size:1.3rem;
    border:none;
    border-radius:50px;
    cursor:pointer;
    background:white;
    color:#ff4f81;
    font-weight:bold;
    transition:0.3s;
}

button:hover{
    transform:scale(1.05);
}

.message{
    margin-top:30px;
    font-size:1.7rem;
    min-height:80px;
    background:rgba(255,255,255,0.15);
    padding:20px;
    border-radius:20px;
}
</style>
</head>
<body>

<div class="container">
    <h1>PRESS WHEN YOU MISS ME ❤️</h1>

    <button onclick="showMessage()">
        ❤️ PRESS ME ❤️
    </button>

    <div class="message" id="message">
        Your surprise message will appear here...
    </div>
</div>

<script>
const messages = [
    "📞 Call me.",
    "🤳 Send me a selfie.",
    "🤫 Tell me something you haven't told me before.",
    "🎥 5-minute video call. No excuses.",
    "🤗 Close your eyes. Imagine I'm hugging you.",
    "❤️ I love you. That's it. That's today's message.",
    "🎵 Send me the song you're listening to right now.",
    "💭 What's the first thing you thought about today?",
    "😂 Send me your funniest photo.",
    "💌 Tell me one thing you love about us.",
    "🌙 Voice note challenge. Go!",
    "🥰 Smile. I know you look cute right now."
];

function showMessage(){
    const random =
        messages[Math.floor(Math.random() * messages.length)];

    document.getElementById("message").innerText = random;
}
</script>

</body>
</html>
