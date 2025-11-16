<h2 id="experience" style="margin: 2px 0px -15px;">Experience</h2>

<div class="experience-timeline">
  <ul class="timeline-list">
  {% for item in site.data.timeline.main %}
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
  padding-left: 0;
  margin-left: 0;
}

.timeline-list {
  list-style: none;
  border-left: 3px solid #ccc;
  margin-left: 20px;
  padding-left: 30px;
}

.timeline-item {
  position: relative;
  margin-bottom: 40px;
}

.timeline-item::before {
  content: "";
  position: absolute;
  left: -11px;
  top: 6px;
  width: 14px;
  height: 14px;
  background: #1f77b4;
  border-radius: 50%;
  border: 2px solid white;
  box-shadow: 0 0 0 2px #1f77b4;
}

.timeline-date {
  font-size: 16px;
  font-weight: 700;
  margin-bottom: 8px;
  margin-left: -5px;
}

.exp-title {
  font-size: 20px;
  font-weight: 700;
  margin-bottom: 6px;
}

.exp-summary {
  font-size: 16px;
  color: #555;
  max-width: 90%;
}
</style>