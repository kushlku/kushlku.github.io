<h2 id="experience" style="margin: 2px 0px -15px;">Experience</h2>

<div class="experience-timeline">
  <ul class="timeline-list">
  {% for item in site.data.experience.main %}
    <li class="timeline-item">
      <div class="timeline-date">{{ item.date }}</div>
      <div class="timeline-content">
        <div class="exp-title">{{ item.title }}</div>
        <div class="exp-summary">{{ item.summary }}</div>
      </div>
    </li>
  {% endfor %}
  </ul>
</div>

<style>
.experience-timeline {
  padding-left: 10px;
}

.timeline-list {
  list-style: none;
  border-left: 2px solid #ccc;
  margin-left: 20px;
  padding-left: 20px;
}

.timeline-item {
  position: relative;
  margin-bottom: 20px;
}

.timeline-item::before {
  content: "";
  position: absolute;
  left: -11px;
  top: 4px;
  width: 12px;
  height: 12px;
  background: #3498db;
  border-radius: 50%;
}

.timeline-date {
  font-size: 14px;
  font-weight: bold;
  margin-bottom: 5px;
}

.exp-title {
  font-size: 16px;
  font-weight: 600;
}

.exp-summary {
  font-size: 14px;
  color: #555;
}
</style>