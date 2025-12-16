---
layout: default
title: Exams
---

[← Back to Home](./index.html)

<div class="search-box">
  <input type="text" id="searchInput" onkeyup="filterCourses()" placeholder="🔍 Search by course code (e.g., MAT2060)...">
</div>

<script>
function filterCourses() {
  // 1. Get the input
  var input = document.getElementById('searchInput');
  var filter = input.value.toUpperCase();
  
  // 2. Get all headers (h3) and lists (ul)
  var mainContent = document.querySelector('.main-content') || document.body;
  var headers = mainContent.getElementsByTagName('h3');
  
  // 3. Loop through headers
  for (var i = 0; i < headers.length; i++) {
    var h3 = headers[i];
    var ul = h3.nextElementSibling; // The list immediately following the header
    var textValue = h3.textContent || h3.innerText;

    // 4. Check if text matches
    if (textValue.toUpperCase().indexOf(filter) > -1) {
      h3.style.display = "";
      if (ul && ul.tagName === 'UL') ul.style.display = "";
    } else {
      h3.style.display = "none";
      // Hide the list following the header as well
      if (ul && ul.tagName === 'UL') ul.style.display = "none";
    }
  }
}
</script>

<style>
.search-box input {
  width: 100%;
  padding: 12px;
  margin-bottom: 20px;
  font-size: 16px;
  border: 2px solid #6c5ce7; /* Light Purple border */
  border-radius: 8px;
  background-color: #f8f9fa;
}
</style>


### MAT1012: Honor Calculus II
* **2024**
  * [Midterm Exam Paper](./exams/MAT1012/MAT1012_2024_Midterm.pdf)
* **2022**
  * [Midterm Exam Paper](./exams/MAT1012/MAT1012_2022_Midterm.pdf).


### MAT2060: Honor Mathematical Analysis
* **2024**
  * [Midterm Exam Paper](./exams/MAT2060/MAT2060_2024_Midterm.pdf)
* **2022**
  * [Midterm Exam Paper](./exams/MAT2060/MAT2060_2022_Midterm.pdf)


### MAT3006: Real Analysis
* **2025**
  * [Midterm Exam Paper](./exams/MAT3006/MAT3006_2025_Midterm.pdf).
  * [Final Exam Paper](./exams/MAT3006/MAT3006_2025_Final.pdf)


### MAT3040: Linear Algebra
* **2024**
  * [Midterm Exam Paper](./exams/MAT3040/MAT3040_2024_Midterm.pdf)
  * [Final Exam Paper](./exams/MAT3040/MAT3040_2024_Final.pdf)


### MAT4002: Topology and Geometry
* **2024**
  * [Midterm Exam Paper](./exams/MAT4002/Mat4002%20Year%202024%20Midterm.pdf)
  * [Midterm Exam Paper](./exams/MAT4002/Previous%20MAT4002_Final_Examination.pdf)
* **2022**
  * [Midterm Exam Paper](./exams/MAT4002/MAT4002_2022_Midterm.pdf)
  * [Final Exam Paper](./exams/MAT4002/MAT4002_2022_Final.pdf)


### MAT4033: Differential Geometry
* **2024**
  * [Midterm Exam Paper](./exams/MAT4033/MAT4033_2024_Midterm.pdf)
  * [Final Exam Paper](./exams/MAT4033/MAT4033_2024_Final.pdf)
* **2023**
  * [Midterm Exam Paper](./exams/MAT4033/MAT4033_2023_Midterm.pdf)
  * [Midterm Exam Paper](./exams/MAT4033/MAT4033_2023_Final.pdf)


### LongFeng Math Contest
* **2024**
  * [Paper for Math major](./exams/Contest/2024_math.pdf)
  * [Paper for Non-Math major](./exams/Contest/2024_nonmath.pdf)