---
layout: single
author_profile: true
title: ""
hide_title: true
show_recent_posts: false   # hides Recent Posts in sidebar
---

<!-- Tabs -->
<div class="tabs">
  <button class="tablink active" onclick="openTab(event,'about')">About</button>  
  <button class="tablink" onclick="openTab(event,'projects')">Projects</button>
  <button class="tablink" onclick="openTab(event,'publications')">Publications</button>
  <button class="tablink" onclick="openTab(event,'education')">Education</button>
  <button class="tablink" onclick="openTab(event,'hobbies')">Hobbies</button>
</div>

<div id="about" class="tabcontent" markdown="1">
  {% include about.md %}
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
..tabs {
  display: flex;
  gap: 8px;
  margin-bottom: 20px;
  flex-wrap: wrap;
}

.tablink {
  background: #f5f5f5;      /* light neutral background */
  border: 1px solid #ccc;   /* subtle border */
  padding: 8px 14px;
  cursor: pointer;
  border-radius: 4px;
  font-weight: 500;          /* semi-bold text */
  transition: background 0.2s, color 0.2s;
  color: #333;               /* dark text for readability */
}

.tablink:hover {
  background: #e0e0e0;       /* slightly darker on hover */
}

.tablink.active {
  color: white;              /* white text for contrast */
  border-color: #1a2a36;     /* slightly darker border */
}

</style>
