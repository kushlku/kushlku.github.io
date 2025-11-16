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
  border-left: 2px solid #999;
  margin-left: 20px;
  padding-left: 25px;
}

.timeline-item {
  position: relative;
  margin-bottom: 32px;
}

.timeline-item::before {
  content: "";
  position: absolute;
  left: -10px;
  top: 4px;
  width: 10px;
  height: 10px;
  background: #000;
  border-radius: 50%;
}

.timeline-date {
  font-size: 15px;
  font-weight: 600;
  margin-bottom: 10px;
  margin-left: -2px;
  color: #000;
}

.exp-title {
  font-size: 17px;
  font-weight: 700;
  margin-bottom: 6px;
  color: #000;
}

.exp-summary {
  font-size: 15px;
  color: #333;
  line-height: 1.5;
}
</style>