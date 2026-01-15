[cause.css](https://github.com/user-attachments/files/24650564/cause.css)
@import url('https://fonts.googleapis.com/css2?family=Bubblegum+Sans&family=Comic+Neue:wght@700&family=Quicksand:wght@500&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    cursor: none;
}

body {
    min-height: 100vh;
    background: linear-gradient(-45deg, #ffe6e6, #e6e6ff, #ffebf5);
    background-size: 400% 400%;
    animation: gradientBG 15s ease infinite;
    font-family: 'Quicksand', sans-serif;
    overflow-x: hidden;
    padding: 2rem;
}

.custom-cursor {
    width: 30px;[cause.html](https://github.com/user-attachments/files/24650572/cause.html)<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Why You're My Best Friend! 💖</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <link rel="stylesheet" href="./cause.css">
    <style>
       
    </style>
</head>
<body>
    <div class="custom-cursor">
        <svg viewBox="0 0 24 24">
            <path fill="#ff69b4" d="M12 21.35l-1.45-1.32C5.4 15.36 2 12.28 2 8.5 2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 4.5 2.09C13.09 3.81 14.76 3 16.5 3 19.58 3 22 5.42 22 8.5c0 3.78-3.4 6.86-8.55 11.54L12 21.35z"/>
        </svg>
    </div>

    <div class="container">
        <h1>Happy Birthday chittiluuuu 💖</h1>
        
        <div id="reasons-container"></div>
        
        <button class="shuffle-button">Click Here... 💕</button>
        <div class="reason-counter"></div>

        <div class="ending-section">
            <div class="teddy-hug">
                <img src="./d1.jpg" alt="Teddy Hug">
            </div>
            <div class="ending-text">You're the BESTEST ! 💖</div>
        </div>
    </div>

    <script src="cause.js">
       
    </script>
</body>
</html>

    height: 30px;
    position: fixed;
    pointer-events: none;
    z-index: 9999;
    mix-blend-mode: difference;
    transition: transform 0.1s;
}

.custom-cursor svg {
    width: 100%;
    height: 100%;
    filter: drop-shadow(0 0 5px rgba(255, 182, 193, 0.5));
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    text-align: center;
    position: relative;
    z-index: 1;
}

h1 {
    font-family: 'Bubblegum Sans', cursive;
    font-size: 3rem;
    color: #ff69b4;
    text-shadow: 2px 2px 4px rgba(255, 105, 180, 0.3);
    margin-bottom: 2rem;
    animation: bounce 1s ease infinite;
}

.reason-card {
    background: rgba(255, 255, 255, 0.9);
    border-radius: 20px;
    padding: 2rem;
    margin: 1.5rem;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s, box-shadow 0.3s;
    cursor: pointer;
    position: relative;
    overflow: hidden;
}

.reason-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 25px rgba(255, 105, 180, 0.2);
}

.reason-text {
    font-size: 1.2rem;
    margin-bottom: 1rem;
    position: relative;
    z-index: 2;
}

.gif-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(255, 255, 255, 0.95);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.3s;
    z-index: 1;
}

.reason-card:hover .gif-overlay {
    opacity: 1;
}

.shuffle-button {
    background: linear-gradient(45deg, #ff69b4, #ff99cc);
    border: none;
    border-radius: 50px;
    padding: 1rem 2rem;
    font-size: 1.2rem;
    color: white;
    margin: 2rem 0;
    cursor: pointer;
    transition: transform 0.3s;
    font-family: 'Comic Neue', cursive;
    box-shadow: 0 5px 15px rgba(255, 105, 180, 0.3);
}

.shuffle-button:hover {
    transform: scale(1.1);
}

.floating {
    position: fixed;
    pointer-events: none;
    animation: float 3s ease-in-out infinite;
}

.ending-section {
    margin-top: 4rem;
    padding: 2rem;
    text-align: center;
}

.ending-text {
    font-family: 'Bubblegum Sans', cursive;
    font-size: 2rem;
    color: #ff69b4;
    margin-bottom: 2rem;
    opacity: 0;
    transform: translateY(20px);
}

.teddy-hug {
    width: 200px;
    margin: 0 auto;
    transform: scale(0);
}

@keyframes gradientBG {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}

@keyframes float {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-20px); }
}

@keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
}

@media (max-width: 768px) {
    h1 { font-size: 2rem; }
    .reason-card { margin: 1rem; }
    .reason-text { font-size: 1rem; }
}
.shuffle-button {
    background: linear-gradient(45deg, #ff69b4, #ff99cc);
    border: none;
    border-radius: 50px;
    padding: 1rem 2rem;
    font-size: 1.2rem;
    color: white;
    margin: 2rem 0;
    cursor: pointer;
    transition: all 0.3s;
    font-family: 'Comic Neue', cursive;
    box-shadow: 0 5px 15px rgba(255, 105, 180, 0.3);
}

.shuffle-button.story-mode {
    background: linear-gradient(45deg, #9b6dff, #ff6dc7);
    transform: scale(1.1);
}

.shuffle-button:hover {
    transform: scale(1.1);
}

.shuffle-button.story-mode:hover {
    transform: scale(1.2);
}

.reason-counter {
    font-size: 0.9rem;
    color: #ff69b4;[cause.html](https://github.com/user-attachments/files/24650582/cause.html)

    margin-top: 1rem;
    opacity: 0.7;[Uploading cause.html…]()

}[Uploading cause.html…]()
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Why You're My Best Friend! 💖</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <link rel="stylesheet" href="./cause.css">
    <style>
       
    </style>
</head>
<body>
    <div class="custom-cursor">
        <svg viewBox="0 0 24 24">
            <path fill="#ff69b4" d="M12 21.35l-1.45-1.32C5.4 15.36 2 12.28 2 8.5 2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 4.5 2.09C13.09 3.81 14.76 3 16.5 3 19.58 3 22 5.42 22 8.5c0 3.78-3.4 6.86-8.55 11.54L12 21.35z"/>
        </svg>
    </div>

    <div class="container">
        <h1>Happy Birthday chittiluuuu 💖</h1>
        
        <div id="reasons-container"></div>
        
        <button class="shuffle-button">Click Here... 💕</button>
        <div class="reason-counter"></div>

        <div class="ending-section">
            <div class="teddy-hug">
                <img src="./d1.jpg" alt="Teddy Hug">
            </div>
            <div class="ending-text">You're the BESTEST ! 💖</div>
        </div>
    </div>

    <script src="cause.js">
       
    </script>
</body>
</html>[cause.js](https://github.com/user-attachments/files/24650588/cause.js)
 // Reasons database
 const reasons = [
    { 
        text: "You’re such a kind and wonderful person, and I feel lucky to share such a good bond with you. 💖", 
        emoji: "🌟",
        gif: "gif1.gif"
    },
    { 
        text: "May your day be filled with love, laughter, and endless joy. 🌸 ", 
        emoji: "💗",
        gif: "gif2.gif"
    },
    { 
        text: "Wishing you success, happiness, and everything your heart desires. ✨ ", 
        emoji: "💕",
        gif: "gif1.gif"
    },
    { 
        text: "Stay the amazing girl you are—always spreading positivity around. Have the happiest year ahead! 🥳 ", 
        emoji: "🌟",
        gif: "gif2.gif"
    }
];

// State management
let currentReasonIndex = 0;
const reasonsContainer = document.getElementById('reasons-container');
const shuffleButton = document.querySelector('.shuffle-button');
const reasonCounter = document.querySelector('.reason-counter');
let isTransitioning = false;

// Create reason card with gif
function createReasonCard(reason) {
    const card = document.createElement('div');
    card.className = 'reason-card';
    
    const text = document.createElement('div');
    text.className = 'reason-text';
    text.innerHTML = `${reason.emoji} ${reason.text}`;
    
    const gifOverlay = document.createElement('div');
    gifOverlay.className = 'gif-overlay';
    gifOverlay.innerHTML = `<img src="${reason.gif}" alt="Friendship Memory">`;
    
    card.appendChild(text);
    card.appendChild(gifOverlay);
    
    gsap.from(card, {
        opacity: 0,
        y: 50,
        duration: 0.5,
        ease: "back.out"
    });

    return card;
}

// Display new reason
function displayNewReason() {
    if (isTransitioning) return;
    isTransitioning = true;

    if (currentReasonIndex < reasons.length) {
        const card = createReasonCard(reasons[currentReasonIndex]);
        reasonsContainer.appendChild(card);
        
        // Update counter
        reasonCounter.textContent = `Reason ${currentReasonIndex + 1} of ${reasons.length}`;
        
        currentReasonIndex++;

        // Check if we should transform the button
        if (currentReasonIndex === reasons.length) {
            gsap.to(shuffleButton, {
                scale: 1.1,
                duration: 0.5,
                ease: "elastic.out",
                onComplete: () => {
                    shuffleButton.textContent = "Enter Our Storylane 💫";
                    shuffleButton.classList.add('story-mode');
                    shuffleButton.addEventListener('click', () => {
                        gsap.to('body', {
                            opacity: 0,
                            duration: 1,
                            onComplete: () => {
                                window.location.href = 'last.html'; // Replace with the actual URL of the next page
                            }
                        });
                    });
                }
            });
        }

        // Create floating elements
        createFloatingElement();
        
        setTimeout(() => {
            isTransitioning = false;
        }, 500);
    } else {
        // Handle navigation to new page or section
        window.location.href = "#storylane";
        // Or trigger your next page functionality
    }
}

// Initialize button click
shuffleButton.addEventListener('click', () => {
    gsap.to(shuffleButton, {
        scale: 0.9,
        duration: 0.1,
        yoyo: true,
        repeat: 1
    });
    displayNewReason();
});

// Floating elements function (same as before)
function createFloatingElement() {
    const elements = ['🌸', '✨', '💖', '🦋', '⭐'];
    const element = document.createElement('div');
    element.className = 'floating';
    element.textContent = elements[Math.floor(Math.random() * elements.length)];
    element.style.left = Math.random() * window.innerWidth + 'px';
    element.style.top = Math.random() * window.innerHeight + 'px';
    element.style.fontSize = (Math.random() * 20 + 10) + 'px';
    document.body.appendChild(element);

    gsap.to(element, {
        y: -500,
        duration: Math.random() * 10 + 10,
        opacity: 0,
        onComplete: () => element.remove()
    });
}

// Custom cursor (same as before)
const cursor = document.querySelector('.custom-cursor');
document.addEventListener('mousemove', (e) => {
    gsap.to(cursor, {
        x: e.clientX - 15,
        y: e.clientY - 15,
        duration: 0.2
    });
});

// Create initial floating elements
setInterval(createFloatingElement, 2000);![d1](https://github.com/user-attachments/assets/500251ac-6344-4b3f-b5ed-b5e54d1a57d6)
![d2](https://github.com/user-attachments/assets/13fefaf4-c052-4494-b281-a660b64dc3f0)
![d3](https://github.com/user-attachments/assets/8316d96b-ed13-4028-a63d-ed496a3a530c)![gif1](https://github.com/user-attachments/assets/daf381b3-0e88-4ddf-af17-0e46cf4317fd)

![gif2](https://github.com/user-attachments/assets/12724521-517c-489f-8a9f-15e4a2cf4d78)
[index.html](https://github.com/user-attachments/files/24650608/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <link rel="stylesheet" href="style.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    
</head>
<body>
    <div class="cursor"></div>
    <div class="container">
        <h1>Happy Birthday chittiluuuu💗</h1>
        <div class="greeting"></div>
        <button class="cta-button">Click to Enter Our World 💕</button>
    </div>

    <script src="script.js">
        
    </script>
</body>
</html>[last.html](https://github.com/user-attachments/files/24650613/last.html)
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Our Beautiful Memories ✨</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Quicksand:wght@300;400;500;600&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            background: linear-gradient(135deg,
                    #ffd1dc 0%,
                    #e6e6fa 25%,
                    #ffefd5 50%,
                    #e6e6fa 75%,
                    #ffd1dc 100%);
            background-size: 400% 400%;
            animation: gradientFlow 15s ease infinite;
            font-family: 'Quicksand', sans-serif;
            overflow-x: hidden;
            color: #4a4a4a;
        }

        @keyframes gradientFlow {
            0% {
                background-position: 0% 50%;
            }

            50% {
                background-position: 100% 50%;
            }

            100% {
                background-position: 0% 50%;
            }
        }

        /* Enhanced Sparkle Effect */
        .magic-sparkles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .sparkle {
            position: absolute;
            width: 6px;
            height: 6px;
            border-radius: 50%;
            background-color: white;
            animation: twinkle var(--duration, 4s) ease-in-out infinite;
            opacity: 0;
        }

        @keyframes twinkle {

            0%,
            100% {
                opacity: 0;
                transform: scale(0.5);
            }

            50% {
                opacity: 0.8;
                transform: scale(1);
            }
        }

        /* Generate 50 sparkles with different positions and animations */
        .magic-sparkles::before,
        .magic-sparkles::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: radial-gradient(circle, white 1px, transparent 1px);
            background-size: 50px 50px;
            animation: sparkleLayer 8s linear infinite;
            opacity: 0.5;
        }

        .magic-sparkles::after {
            animation-delay: -4s;
            transform: rotate(45deg);
        }

        @keyframes sparkleLayer {
            0% {
                transform: translateY(0);
            }

            100% {
                transform: translateY(-50px);
            }
        }

        /* Floating Hearts */
        .floating-hearts {
            position: fixed;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 2;
        }

        .heart {
            position: absolute;
            font-size: 1.5rem;
            color: rgba(255, 105, 180, 0.6);
            animation: floatHeart var(--float-duration, 6s) ease-in-out infinite;
            animation-delay: var(--delay, 0s);
        }

        @keyframes floatHeart {
            0% {
                transform: translate(0, 100vh) rotate(0deg);
            }

            100% {
                transform: translate(var(--translate-x, 0), -100vh) rotate(360deg);
            }
        }

        /* Welcome Section */
        .welcome {
            text-align: center;
            padding: 4rem 2rem;
            position: relative;
            z-index: 3;
        }

        .welcome h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 4rem;
            color: #ff69b4;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
            animation: fadeInScale 2s ease;
        }

        .welcome p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 1.5rem auto;
            line-height: 1.6;
            animation: fadeIn 2s ease 0.5s both;
        }

        /* Enhanced Memory Cards */
        .memory-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            z-index: 3;
            position: relative;
        }

        .memory-card {
            background: rgba(255, 255, 255, 0.9);
            border-radius: 20px;
            padding: 1.5rem;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .memory-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .memory-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.4), transparent);
            transform: translateX(-100%);
            transition: 0.5s;
        }

        .memory-card:hover::before {
            transform: translateX(100%);
        }

        .memory-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 15px;
            margin-bottom: 1rem;
            transition: transform 0.5s ease;
        }

        .memory-card:hover .memory-img {
            transform: scale(1.05);
        }

        .memory-date {
            font-family: 'Dancing Script', cursive;
            color: #ff69b4;
            font-size: 1.3rem;
            margin-bottom: 0.5rem;
        }

        .memory-caption {
            font-size: 1rem;
            line-height: 1.5;
            color: #666;
        }

        /* Final Message Section */
        .final-message {
            text-align: center;
            padding: 4rem 2rem;
            background: rgba(255, 255, 255, 0.3);
            backdrop-filter: blur(10px);
            margin-top: 3rem;
            position: relative;
            z-index: 3;
        }

        .final-message h2 {
            font-family: 'Dancing Script', cursive;
            font-size: 3rem;
            color: #ff69b4;
            margin-bottom: 2rem;
            animation: heartbeat 2s infinite;
        }

        @keyframes heartbeat {

            0%,
            100% {
                transform: scale(1);
            }

            50% {
                transform: scale(1.1);
            }
        }

        .final-message p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
            line-height: 1.8;
        }

        .goodbye-btn {
            display: inline-block;
            padding: 1rem 2rem;
            font-size: 1.2rem;
            background: linear-gradient(45deg, #ff69b4, #da70d6);
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            text-decoration: none;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(255, 105, 180, 0.4);
            animation: float 3s infinite ease-in-out;
        }

        .goodbye-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(255, 105, 180, 0.6);
        }

        @keyframes float {

            0%,
            100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-10px);
            }
        }

        /* Animations */
        @keyframes fadeInScale {
            0% {
                opacity: 0;
                transform: scale(0.8);
            }

            100% {
                opacity: 1;
                transform: scale(1);
            }
        }

        @keyframes fadeIn {
            0% {
                opacity: 0;
            }

            100% {
                opacity: 1;
            }
        }

        /* Generate Hearts */
        .js-generate-hearts {
            position: fixed;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 2;
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 12px;
        }

        ::-webkit-scrollbar-track {
            background: rgba(255, 255, 255, 0.4);
        }

        ::-webkit-scrollbar-thumb {
            background: linear-gradient(45deg, #ff69b4, #da70d6);
            border-radius: 6px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .welcome h1 {
                font-size: 3rem;
            }

            .memory-container {
                grid-template-columns: 1fr;
            }

            .final-message h2 {
                font-size: 2.5rem;
            }
        }
    </style>
</head>

<body>
    <div class="magic-sparkles"></div>
    <div class="floating-hearts">
        <!-- Hearts will be generated via CSS -->
        <div class="heart" style="--float-duration: 6s; --delay: 0s; --translate-x: 20px;">💝</div>
        <div class="heart" style="--float-duration: 8s; --delay: 1s; --translate-x: -30px;">💖</div>
        <div class="heart" style="--float-duration: 7s; --delay: 2s; --translate-x: 40px;">💗</div>
        <div class="heart" style="--float-duration: 9s; --delay: 3s; --translate-x: -20px;">💓</div>
        <div class="heart" style="--float-duration: 5s; --delay: 4s; --translate-x: 30px;">💕</div>
    </div>

    <section class="welcome">
        <h1>Our Beautiful Moments Together</h1>
        <p>Every moment spent with you has been magical. Let's cherish these precious memories ...</p>
    </section>

    <div class="memory-container">
        <div class="memory-card">
            <img src="./d1.jpg" alt="First Date" class="memory-img">
            <div class="memory-date">Her Smile Says It All</div>
            <div class="memory-caption">You’re truly one of the sweetest girls I know, and I feel lucky to have a sis
                like you.❤️</div>
        </div>
        <div class="memory-card">
            <img src="./d2.jpg" alt="Beach Day" class="memory-img">
            <div class="memory-date">Together Vibes</div>
            <div class="memory-caption">May your journey ahead be filled with happiness, success, and endless
                smiles.😊💕</div>
        </div>
        <div class="memory-card">
            <img src="./d3.jpg" alt="Movie Night" class="memory-img">
            <div class="memory-date">Pretty Soul</div>
            <div class="memory-caption">Keep being the amazing person you are—you make every moment brighter.🌸💖</div>
        </div>

    </div>

    <section class="final-message">
        <h2>Thank You for the Memories</h2>
        <p>Every laugh, every chat, and every moment we’ve shared has been truly special.💫<br>
            I’m so grateful for the bond we have, and for the positivity you always bring into my life.<br>
            On your birthday, I just wish for endless happiness, love, and success to come your way.🌸</p>
        <p>You deserve all the joy in the world—keep shining and spreading your beautiful energy.✨</p>
        <a href="#" class="goodbye-btn">Until We Meet Again 💝</a>
    </section>
</body>

</html>[README.md](https://github.com/user-attachments/files/24650620/README.md)[script.js](https://github.com/user-attachments/files/24650627/script.js)

// Cursor following effect
const cursor = document.querySelector('.cursor');
document.addEventListener('mousemove', (e) => {
    cursor.style.left = e.clientX + 'px';
    cursor.style.top = e.clientY + 'px';
});

// Typing effect for greeting
const greetingText = "Hey You Know What! You're the most adorable human i ever met! 💖";
const greetingElement = document.querySelector('.greeting');
let charIndex = 0;

function typeGreeting() {
    if (charIndex < greetingText.length) {
        greetingElement.textContent += greetingText.charAt(charIndex);
        charIndex++;
        setTimeout(typeGreeting, 100);
    }
}

// Create floating elements
const floatingElements = ['💖', '✨', '🌸', '💫', '💕'];
function createFloating() {
    const element = document.createElement('div');
    element.className = 'floating';
    element.textContent = floatingElements[Math.floor(Math.random() * floatingElements.length)];
    element.style.left = Math.random() * 100 + 'vw';
    element.style.top = Math.random() * 100 + 'vh';
    element.style.fontSize = (Math.random() * 20 + 20) + 'px';
    document.body.appendChild(element);

    gsap.to(element, {
        y: -500,
        x: Math.random() * 100 - 50,
        rotation: Math.random() * 360,
        duration: Math.random() * 5 + 5,
        opacity: 1,
        ease: "none",
        onComplete: () => element.remove()
    });
}

// Initialize animations
window.addEventListener('load', () => {
    // Title animation
    gsap.to('h1', {
        opacity: 1,
        duration: 1,
        y: 20,
        ease: "bounce.out"
    });

    // Button animation
    gsap.to('.cta-button', {
        opacity: 1,
        duration: 1,
        y: -20,
        ease: "back.out"
    });

    // Start typing effect
    typeGreeting();

    // Create floating elements periodically
    setInterval(createFloating, 1000);
});

// Hover effects
       // Hover effects
       document.querySelectorAll('.cta-button').forEach(button => {
        button.addEventListener('mouseenter', () => {
            gsap.to(button, {
                scale: 1.1,
                duration: 0.3
            });
        });

        button.addEventListener('mouseleave', () => {
            gsap.to(button, {
                scale: 1,
                duration: 0.3
            });
        });

        // Smooth page transition on click
        button.addEventListener('click', () => {
            gsap.to('body', {
                opacity: 0,
                duration: 1,
                onComplete: () => {
                    window.location.href = 'cause.html'; // Replace with the actual URL of the next page
                }
            });
        });
    });[style.css](https://github.com/user-attachments/files/24650629/style.css)
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    cursor: none;
}

body {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: linear-gradient(-45deg, #fee9f7, #e8f5fe, #fef2e8, #f0ffe8);
    background-size: 400% 400%;
    animation: gradientBG 15s ease infinite;
    font-family: 'Arial Rounded MT Bold', Arial, sans-serif;
    overflow: hidden;
    position: relative;
}

.cursor {
    width: 20px;
    height: 20px;
    background: pink;
    border-radius: 50%;
    position: fixed;
    pointer-events: none;
    mix-blend-mode: difference;
    transition: transform 0.2s;
}

.container {
    text-align: center;
    z-index: 1;
}

h1 {
    font-size: 3.5rem;
    color: #ff69b4;
    text-shadow: 0 0 10px rgba(255, 105, 180, 0.5);
    margin-bottom: 2rem;
    opacity: 0;
}

.greeting {
    font-size: 1.5rem;
    color: #8a2be2;
    margin-bottom: 3rem;
    min-height: 2em;
}

.cta-button {
    padding: 1rem 2rem;
    font-size: 1.2rem;
    background: linear-gradient(45deg, #ff69b4, #ff99cc);
    border: none;
    border-radius: 50px;
    color: white;
    cursor: pointer;
    box-shadow: 0 0 15px rgba(255, 105, 180, 0.5);
    transition: transform 0.3s, box-shadow 0.3s;
    opacity: 0;
}

.cta-button:hover {
    transform: scale(1.1);
    box-shadow: 0 0 25px rgba(255, 105, 180, 0.7);
}

.floating {
    position: absolute;
    pointer-events: none;
    opacity: 0;
}

@keyframes gradientBG {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}

@media (max-width: 768px) {
    h1 { font-size: 2rem; }
    .greeting { font-size: 1.2rem; }
    .cta-button { font-size: 1rem; }
}
