---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{: style="text-align: justify" }
I am currently employed at LiveTSE, where I have been working on the development of an automated technical trading system for the Tehran Stock Market. Furthermore, I have a strong academic background and experience in managing electrical and computer engineering projects, with a focus on solving mathematical and engineering problems using Deep Reinforcement Learning. My research focuses on machine learning and its applications in signal processing, image processing, bioinformatics, and communications. I am also proficient in several programming languages, including Python, MATLAB, Mathcad, and C.

Education
======
**Sharif University of Technology**
* M.S. in Electrical Engineering - Communication Systems, 2019-2022
* **CGPA**: 17.11/20 (3.7/4)
* **Thesis Title**: Algorithmic Trading Using Deep Reinforcement Learning
* **Supervisor**: [Prof. Farokh Marvasti](https://scholar.google.com/citations?user=QqZjvMoAAAAJ&hl=en)

**Isfahan University of Technology**
* B.S. in Electrical Engineering, 2015-2019
* **CGPA**: 17.77/20 (3.87/4.0)
* **Final Project**: Implementing Portable ECG Monitor on Arduino
* **Supervisor**: [Prof. Behzad Nazari](https://scholar.google.com/citations?user=OQVDaXMAAAAJ&hl=en)

Work experience
======
* June 2022 - Current: Data Scientist
  * Arya Sarmaye Algo. Company
  * [LiveTSE](https://livetse.ir/)
  * Developing an "Automated Technical Analyzer" on the Tehran Stock Market
 
Research Interests
======
* Machine Learning
  * Deep Learning
  * Reinforcement Learning
  * Graph Neural Network
* Medical Image Analysis
* Communication Systems
* Computer Vision
* Signal Processing
* Bioinformatics
* Causal Inference

Selected Projects
======
* [Stock Market Predictor Using Conv-Gru](https://nasehmajidi.github.io//portfolio/Stock%20Market%20Predictor/)
* [Vector Quantization](https://nasehmajidi.github.io//portfolio/Vector%20Quantization/)

  
[**More**](/portfolio/)
  
Skills
======
* Machine Learning in Python
  * PyTorch
  * Scikit-learn
  * Keras
* Python Programming
* MATLAB/Simulink
* LATEX
* Arduino Programming


Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Toggleable Lists</title>
  <style>
    body {
      font-family: sans-serif;
    }

    .list-container {
      margin: 20px;
      padding: 20px;
      background-color: white;
      border-radius: 5px;
      border-bottom: 5px solid white;
    }

    ul {
      list-style: none;
      margin: 0;
      padding: 0;
    }

    li {
      margin-bottom: 10px;
    }

    .button {
      background-color: #007bff;
      color: white;
      padding: 10px 20px;
      border-radius: 5px;
      cursor: pointer;
    }

    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <div class="list-container">
    <h2>List 1</h2>
    <ul id="list1">
      <li>Item 1</li>
      <li>Item 2</li>
      <li class="hidden">Item 3</li>
      <li class="hidden">Item 4</li>
      <li class="hidden">Item 5</li>
    </ul>
    <button id="toggle-button1" class="button">Show More</button>

    <h2>List 2</h2>
    <ul id="list2">
      <li>Item 6</li>
      <li>Item 7</li>
      <li class="hidden">Item 8</li>
      <li class="hidden">Item 9</li>
      <li class="hidden">Item 10</li>
    </ul>
    <button id="toggle-button2" class="button">Show More</button>

    <h2>List 3</h2>
    <ul id="list3">
      <li>Item 11</li>
      <li>Item 12</li>
      <li class="hidden">Item 13</li>
      <li class="hidden">Item 14</li>
      <li class="hidden">Item 15</li>
    </ul>
    <button id="toggle-button3" class="button">Show More</button>
  </div>

  <script>
    const toggleButtons = document.querySelectorAll('.button');
    const hiddenItems = document.querySelectorAll('.hidden');

    for (const toggleButton of toggleButtons) {
      const listId = toggleButton.id.replace('toggle-button', 'list');
      const listItems = document.getElementById(listId).querySelectorAll('li');

      let isExpanded = false;

      toggleButton.addEventListener('click', () => {
        if (isExpanded) {
          for (let i = 2; i < listItems.length; i++) {
            listItems[i].classList.add('hidden');
          }
          toggleButton.textContent = 'Show More';
          isExpanded = false;
        } else {
          for (let i = 2; i < listItems.length; i++) {
            listItems[i].classList.remove('hidden');
          }
          toggleButton.textContent = 'Show Less';
          isExpanded = true;
        }
      });
    }
  </script>
</body>
</html>
