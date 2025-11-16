<h2 id="experience" style="margin: 2px 0px -15px;">Timeline</h2>

<div class="experience-timeline">
  <ul class="timeline-list" style="margin-top: 25px;">
  {% for item in site.data.timeline.main %}
    <li class="timeline-item">
      <div class="timeline-date">{{ item.date }}</div>
      <div class="timeline-content">
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
  padding-left: 25px;
}

.timeline-item {
  position: relative;
  margin-bottom: 5px;
}

.timeline-item::before {
  content: "";
  position: absolute;
  left: -12px;
  top: 8px;
  width: 7px;
  height: 7px;
  background: #666;
  border-radius: 50%;
}

.timeline-date {
  font-size: 17px;
  margin-bottom: 5px;
  margin-left: 10px;
  color: #555;
}

.exp-summary {
  font-size: 16px;
  color: #db7093;
  margin-left: 25px;
  font-style: italic;
}
</style>