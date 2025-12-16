---
layout: default
title: Notes and Slides
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


### MAT1011：Honor Caculus
* **2025**
  * [Final Review Lectures](./notes/MAT1011/MAT1011_2025_Final_slides.pptx)


### MAT2060: Honor Mathematical Analysis
* **Additional Exercises**
  * [Professor Li's Problem set](./notes/MAT2060/Li_problem_set.zip)
  * [Additional Problem set](./notes/MAT2060/Wang_problem_set.pdf)

* **2025**
  * [Final Review Lectures](./notes/MAT2060/MAT2060_2025_Final_slides.pdf)
  * [A quick introduction to differential forms](./notes/MAT2060/quick_intro_to_differential_forms_presentation.pdf)


### MAT3006: Real Analysis
* **2025**
  * [Final Review Lectures](./notes/MAT3006/MAT3006_2025_Final_slides.pdf)


### MAT3042: Honor Advanced Linear Algebra
* **Additional Exercises**
  * [Additional Problem set](./notes/MAT3042/Wang_problem_set_linearalgebra.pdf)

### MAT4002: Topology and Geometry
* **Typed Lecture Notes**
  * [MAT4002 note](./notes/MAT4002/MAT4002_note.pdf)

### MAT4033: Differential Geometry
* **Typed Lecture Notes** 
  * [MAT4033 Notes](./notes/MAT4033/MAT4033_note.pdf)
* **2026** 
  * [Final Review Lectures](./notes/MAT4033/MAT4033_2026_Final_slides.pdf)
