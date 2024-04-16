### Hi there 👋

<!--
**chienthan2vn/chienthan2vn** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Text Animation</title>
    <style>
        *{
           margin: 0;
           padding: 0;
           box-sizing: border-box;
           font-size: 'poppins', sans-serif;
        }
        .container{
          width: 100;
          height: 100vh;
          background: #1b1f29;
        }
        svg{
          font-size: 150px;
          padding-top: 10%;
        }
        .copy-text{
          fill: none;
          stroke: #fff;
          stroke-width: 3px;
          stroke-dasharray: 8% 30%;
          stroke-dashoffset: 0%;
          animation: textanimation 6s linear infinite;
        }
        @keyframes textanimation{
          100%{
               stroke-dashoffset: -35%;
            }
         }
        .copy-text1{
           stroke: #f66335;
           animation-delay: -1s;
        }
        .copy-text2{
           stroke: #ff9f1c;
           animation-delay: -2s;
        }
        .copy-text3{
           stroke: #8ac926;
           animation-delay: -3s;
        }
        .copy-text4{
           stroke: #1982c4;
           animation-delay: -4s;
        }
        .copy-text5{
           stroke: #8338ec;
           animation-delay: -5s;
        }
    </style>
</head>
<body>
   <div class="container">
      <svg viewbox="0 0 1000 400">
          <text id="text" x="50%" y="50%" fill="none" text-anchor="middle">
              Cosas Learning
          </text>
          <use xlink:href="#text" class="copy-text copy-text1"></use>
          <use xlink:href="#text" class="copy-text copy-text2"></use>
          <use xlink:href="#text" class="copy-text copy-text3"></use>
          <use xlink:href="#text" class="copy-text copy-text4"></use>
          <use xlink:href="#text" class="copy-text copy-text5"></use>
      </svg> 
   </div>
</body>
</html>
