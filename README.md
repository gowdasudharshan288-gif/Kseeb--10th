<!DOCTYPE html>
<html>
<head>
  <title>KSEEB 10th All Subjects Quiz</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      font-family: Arial;
      background: #f2f6ff;
      padding: 15px;
    }
    h1, h2 {
      text-align: center;
    }
    select, button {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      font-size: 16px;
    }
    .option {
      background: white;
      border: 1px solid #ccc;
      padding: 10px;
      margin: 6px 0;
      cursor: pointer;
    }
    .option:hover {
      background: #e6ecff;
    }
  </style>
</head>

<body>

<h1>KSEEB 10th Quiz</h1>

<!-- SUBJECT SELECTION -->
<select id="subjectSelect" onchange="startQuiz()">
  <option value="">-- Select Subject --</option>
  <option value="kannada">Kannada</option>
  <option value="english">English</option>
  <option value="hindi">Hindi</option>
  <option value="maths">Maths</option>
  <option value="science">Science</option>
  <option value="social">Social Science</option>
</select>

<h2 id="question"></h2>

<div id="options"></div>

<h3 id="score"></h3>

<script>
let current = 0;
let score = 0;
let quiz = [];

/* ================= ALL SUBJECT QUESTIONS ================= */

const allQuizzes = {

kannada: [
  { q: "ಕನ್ನಡದ ಆದಿಕವಿ ಯಾರು?", o: ["ಪಂಪ", "ರನ್ನ", "ಜನ್ನ", "ಕುಮಾರವ್ಯಾಸ"], a: 0 },
  { q: "ವಚನ ಸಾಹಿತ್ಯದ ನಾಯಕ ಯಾರು?", o: ["ಬಸವಣ್ಣ", "ಪಂಪ", "ಪುರಂದರದಾಸ", "ರನ್ನ"], a: 0 },
  { q: "ಜ್ಞಾನಪೀಠ ಪ್ರಶಸ್ತಿ ಪಡೆದ ಮೊದಲ ಕನ್ನಡ ಕವಿ?", o: ["ಪಂಪ", "ಕುವೆಂಪು", "ದ.ರಾ.ಬೇಂದ್ರೆ", "ಮಾಸ್ತಿ"], a: 1 },
  // 👉 Add till 30
],

english: [
  { q: "Who wrote 'Romeo and Juliet'?", o: ["Milton", "Shakespeare", "Keats", "Wordsworth"], a: 1 },
  { q: "Plural of 'Child'?", o: ["Childs", "Children", "Childes", "Childrens"], a: 1 },
  { q: "Synonym of Happy?", o: ["Sad", "Joyful", "Angry", "Weak"], a: 1 },
],

hindi: [
  { q: "हिंदी दिवस कब मनाया जाता है?", o: ["14 सितंबर", "26 जनवरी", "15 अगस्त", "2 अक्टूबर"], a: 0 },
  { q: "कबीर किसके भक्त थे?", o: ["राम", "कृष्ण", "शिव", "दुर्गा"], a: 0 },
  { q: "भारत की राष्ट्रभाषा क्या है?", o: ["हिंदी", "संस्कृत", "उर्दू", "अंग्रेज़ी"], a: 0 },
],

maths: [
  { q: "Value of π?", o: ["2.14", "3.14", "4.14", "3.41"], a: 1 },
  { q: "Area of circle formula?", o: ["πr²", "2πr", "r²", "πd"], a: 0 },
  { q: "Square root of 144?", o: ["10", "11", "12", "13"], a: 2 },
],

science: [
  { q: "Chemical formula of water?", o: ["H2O", "CO2", "O2", "H2"], a: 0 },
  { q: "Unit of force?", o: ["Joule", "Newton", "Watt", "Pascal"], a: 1 },
  { q: "Plant process of making food?", o: ["Respiration", "Digestion", "Photosynthesis", "Transpiration"], a: 2 },
],

social: [
  { q: "Capital of Karnataka?", o: ["Mysuru", "Bengaluru", "Hubli", "Mangaluru"], a: 1 },
  { q: "Father of Indian Constitution?", o: ["Gandhi", "Nehru", "Ambedkar", "Patel"], a: 2 },
  { q: "Indian Independence year?", o: ["1945", "1946", "1947", "1950"], a: 2 },
]

};

/* ================= QUIZ LOGIC ================= */

function startQuiz() {
  const subject = document.getElementById("subjectSelect").value;
  if (!subject) return;

  quiz = allQuizzes[subject];
  current = 0;
  score = 0;
  loadQuestion();
}

function loadQuestion() {
  if (current >= quiz.length) {
    document.getElementById("question").innerText =
      "Quiz Finished 🎉 Your Score: " + score + "/" + quiz.length;
    document.getElementById("options").innerHTML = "";
    return;
  }

  document.getElementById("question").innerText =
    (current + 1) + ". " + quiz[current].q;

  const optDiv = document.getElementById("options");
  optDiv.innerHTML = "";

  quiz[current].o.forEach((opt, i) => {
    const div = document.createElement("div");
    div.className = "option";
    div.innerText = opt;
    div.onclick = () => checkAnswer(i);
    optDiv.appendChild(div);
  });

  document.getElementById("score").innerText = "Score: " + score;
}

function checkAnswer(choice) {
  if (choice === quiz[current].a) score++;
  current++;
  loadQuestion();
}
</script>

</body>
</html></body>
</html>index.html<!DOCTYPE html>
<html>
<head>
  <title>KSEEB Hindi Question Papers</title>
</head>
<body>

<h2>Hindi – Previous Year Question Papers</h2>

<h3>2023</h3>
<ul>
  <li>Question Paper: <a href="#">Download PDF</a></li>
  <li>Answer Key: <a href="#">Download Answers</a></li>
</ul>

<h3>2022</h3>
<ul>
  <li>Question Paper: <a href="#">Download PDF</a></li>
  <li>Answer Key: <a href="#">Download Answers</a></li>
</ul>

<a href="index.html">⬅ Back to Home</a>

</body>
</html><!DOCTYPE html>
<html>
<head>
  <title>KSEEB English Question Papers</title>
</head>
<body>

<h2>English – Previous Year Question Papers</h2>

<h3>2023</h3>
<ul>
  <li>Question Paper: <a href="#">Download PDF</a></li>
  <li>Answer Key: <a href="#">Download Answers</a></li>
</ul>

<h3>2022</h3>
<ul>
  <li>Question Paper: <a href="#">Download PDF</a></li>
  <li>Answer Key: <a href="#">Download Answers</a></li>
</ul>

<a href="index.html">⬅ Back to Home</a>

</body>
</html><!DOCTYPE html>
<html>
<head>
  <title>KSEEB Kannada Question Papers</title>
</head>
<body>

<h2>Kannada – Previous Year Question Papers</h2>

<h3>2023</h3>
<ul>
  <li>
    Question Paper:
    <a href="https://kseeb.karnataka.gov.in" target="_blank">Download PDF</a>
  </li>
  <li>
    Answer Key:
    <a href="#">Download Answers</a>
  </li>
</ul>

<h3>2022</h3>
<ul>
  <li>Question Paper: <a href="#">Download PDF</a></li>
  <li>Answer Key: <a href="#">Download Answers</a></li>
</ul>

<a href="index.html">⬅ Back to Home</a>

</body>
</html><!DOCTYPE html>
<html>
<head>
  <title>KSEEB 10th Previous Year Papers</title>
</head>
<body>

<h1>KSEEB 10th Class</h1>
<p>Previous Year Question Papers with Answers</p>

<ul>
  <li><a href="kannada.html">Kannada</a></li>
  <li><a href="english.html">English</a></li>
  <li><a href="hindi.html">Hindi</a></li>
</ul>

</body>
</html>body {
  font-family: Arial;
  background: #f2f7ff;
  padding: 20px;
}

header {
  background: #004aad;
  color: white;
  padding: 15px;
  text-align: center;
}

nav a {
  margin: 10px;
  text-decoration: none;
  color: #004aad;
  font-weight: bold;
}

button {
  display: block;
  margin: 5px;
  padding: 10px;
  width: 200px;
}body {
  font-family: Arial;
  background: #f2f7ff;
  padding: 20px;
}

header {
  background: #004aad;
  color: white;
  padding: 15px;
  text-align: center;
}

nav a {
  margin: 10px;
  text-decoration: none;
  color: #004aad;
  font-weight: bold;
}

button {
  display: block;
  margin: 5px;
  padding: 10px;
  width: 200px;
}const quizData = [
  {
    question: "Value of π (pi) is?",
    a: "2.14",
    b: "3.14",
    c: "4.14",
    d: "3.41",
    correct: "b"
  },
  {
    question: "Formula of Area of Circle?",
    a: "2πr",
    b: "πr²",
    c: "r²",
    d: "πd",
    correct: "b"
  }
];

let index = 0;

function loadQuiz() {
  const q = quizData[index];
  document.getElementById("question").innerText = q.question;
  document.getElementById("a").innerText = q.a;
  document.getElementById("b").innerText = q.b;
  document.getElementById("c").innerText = q.c;
  document.getElementById("d").innerText = q.d;
}

function checkAnswer(ans) {
  if (ans === quizData[index].correct) {
    document.getElementById("result").innerText = "Correct ✅";
  } else {
    document.getElementById("result").innerText = "Wrong ❌";
  }
  index++;
  if (index < quizData.length) {
    loadQuiz();
  } else {
    document.getElementById("result").innerText += " | Quiz Finished 🎉";
  }
}

loadQuiz();<!DOCTYPE html>
<html>
<head>
  <title>KSEEB Quiz</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<h2>Maths Quiz – Class 10</h2>

<div id="quiz">
  <p id="question"></p>
  <button onclick="checkAnswer('a')" id="a"></button>
  <button onclick="checkAnswer('b')" id="b"></button>
  <button onclick="checkAnswer('c')" id="c"></button>
  <button onclick="checkAnswer('d')" id="d"></button>
</div>

<p id="result"></p>

<script src="quiz.js"></script>

</body>
</html><!DOCTYPE html>
<html>
<head>
  <title>Previous Year Question Papers</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<h2>Previous Year Question Papers (KSEEB 10th)</h2>

<ul>
  <li>
    Mathematics 2023 –
    <a href="https://kseeb.karnataka.gov.in" target="_blank">Download PDF</a>
  </li>
  <li>
    Science 2023 –
    <a href="https://kseeb.karnataka.gov.in" target="_blank">Download PDF</a>
  </li>
  <li>
    Social Science 2022 –
    <a href="https://kseeb.karnataka.gov.in" target="_blank">Download PDF</a>
  </li>
</ul>

<p>👉 Replace links with real PDF links when available.</p>

</body>
</html><!DOCTYPE html>
<html>
<head>
  <title>KSEEB Quiz</title>
</head>
<body>

<h2>Maths Quiz</h2>

<p>1. Value of π?</p>
<p>A) 3.14</p>
<p>B) 2.14</p>
<p>C) 4.14</p>

</body>
</html><!DOCTYPE html>
<html>
<head>
  <title>KSEEB Question Papers</title>
</head>
<body>

<h2>Previous Year Question Papers</h2>

<ul>
  <li>Maths – 2023 (PDF)</li>
  <li>Science – 2023 (PDF)</li>
  <li>Social Science – 2022 (PDF)</li>
</ul>

<a href="index.html">Back to Home</a>

</body>
</html><!DOCTYPE html>
<html>
<head>
  <title>KSEEB 10th Class</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
<body>

<h1>Welcome to KSEEB 10th Class</h1>
<p>Free Previous Year Question Papers & Quizzes</p>

<ul>
  <li><a href="papers.html">Question Papers</a></li>
  <li><a href="quiz.html">Online Quiz</a></li>
</ul>

</body>
</html># Kseeb--10th
10th class learning resources for kseeb board
