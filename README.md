<!DOCTYPE html>
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
