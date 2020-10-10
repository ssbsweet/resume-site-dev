<template>
  <div class="card-panel grey lighten-5 z-depth-3 col s12 m3">
    <div class="section-headline">ЗНАНИЯ</div>
    <div class="progress-first">Atlassian products</div>
    <div class="progress">
      <div class="determinate" style="width: 90%"></div>
    </div>
    <div>Java</div>
    <div class="progress">
      <div class="determinate" style="width: 55%"></div>
    </div>
    <div>Python</div>
    <div class="progress">
      <div class="determinate" style="width: 50%"></div>
    </div>
    <div>WebApi</div>
    <div class="progress">
      <div class="determinate" style="width: 75%"></div>
    </div>
    <div>SQL</div>
    <div class="progress">
      <div class="determinate" style="width: 78%"></div>
    </div>
    <div>Selenium</div>
    <div class="progress">
      <div class="determinate" style="width: 70%"></div>
    </div>
    <div>HTML+CSS+JS</div>
    <div class="progress">
      <div class="determinate" style="width: 60%"></div>
    </div>
    <div class="item">
      <i class="material-icons">calendar_today</i>
      <a>{{ new Date().getFullYear() -1989 }} год</a>
    </div>
    <div class="item">
      <i class="material-icons">location_city</i>
      <a href="https://yandex.ru/maps/-/CGDcMRI~">Россия г.Санкт-Петербург</a>
    </div>
    <div class="item">
      <i class="material-icons">phone</i>
      <a href="tel:+79043320230">+79043320230</a>
    </div>
    <div class="item">
      <i class="material-icons">email</i>
      <a href="mailto:ssbsweet56@gmail.com">ssbsweet56@gmail.com</a>
    </div>
    <div class="item">
      <i class="material-icons">storage</i>
      <a href="https://github.com/ssbsweet?tab=repositories" target="_blank">GitHub</a>
    </div>
  </div>
</template>

<style scoped>
.card-panel.grey.lighten-5.z-depth-3.col.s12.m3 {
  margin-top: 7px;
  padding-bottom: 15px;
}

.progress-first {
  margin-top: 20px;
}

.progress {
  width: 95%;
  height: 8px;
}

.progress .determinate {
  background-color: #29c5e6;
}

.item {
  padding-top: 10px;
}

.item a {
  font-size: 15px;
}

.material-icons {
  float: left;
  font-size: 20px;
  margin-right: 10px;
}

.section-headline {
    width: 100px;
    float: right;
    color: rgba(92, 92, 92, 0.85);
    box-shadow: 2px 3px 3px rgba(0,0,0,0.5);
    padding: 5px 15px;
    margin-bottom: 12px;
    margin-right: -12px;
    border-radius: 5px 0 0 5px;
    background: #7e7e7e;
    color: #fff;
    font-size: 17px;
}

.section-headline:before, .section-headline:after {
    position:absolute;
    content: '';
    display: block;
}

.section-headline:before {
    width: 10px;
    height: 45px;
    margin-left: 85px;
    margin-top: -5px;
    background:inherit;
    border-radius: 0 7px 7px 0;
}

.section-headline:after {
    width: 7px;
    height: 7px;
    margin-left: 85px;
    margin-top: 5px;
    background: rgba(0,0,0,0.35);
    border-radius: 0 6px 6px 0;
    box-shadow: inset -1px 2px 2px rgba(0,0,0,0.3);
}
</style>
