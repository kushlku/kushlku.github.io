---
layout: home
author_profile: true
title: "Home"
---

## Welcome

Hi, I’m Kushal Kumar. Applied Scientist at Amazon, working on AI/ML research. This page summarizes my projects, publications, education, and hobbies.

---

<!-- Tabs -->
<div class="tabs">
  <button class="tablink active" onclick="openTab(event,'projects')">Projects</button>
  <button class="tablink" onclick="openTab(event,'publications')">Publications</button>
  <button class="tablink" onclick="openTab(event,'education')">Education</button>
  <button class="tablink" onclick="openTab(event,'hobbies')">Hobbies</button>
</div>

<div id="projects" class="tabcontent" markdown="1">
  {% include projects.md %}
</div>

<div id="publications" class="tabcontent" markdown="1">
  {% include publications.md %}
</div>

<div id="education" class="tabcontent" markdown="1">
  {% include education.md %}
</div>

<div id="hobbies" class="tabcontent" markdown="1">
  {% include hobbies.md %}
</div>

<script>
function openTab(evt, tabName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].classList.remove("active");
  }
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.classList.add("active");
}

// Optional: activate first tab on page load
document.addEventListener("DOMContentLoaded", function(){
  document.querySelector(".tablink.active").click();
});
</script>

<style>
.tabs {
  display: flex;
  gap: 10px;
  margin-bottom: 20px;
  flex-wrap: wrap;
}
.tablink {
  background: #eee;
  border: none;
  padding: 10px 15px;
  cursor: pointer;
  border-radius: 4px;
}
.tablink.active {
  background: #007acc;
  color: white;
}
.tabcontent {
  display: none;
  padding-top: 1rem;
}
</style>
