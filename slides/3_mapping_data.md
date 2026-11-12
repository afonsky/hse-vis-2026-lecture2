# Сопоставление данных с визуализациями

<br>
<br>
<v-click at="1">

### Некоторые визуальные каналы более эффективны для одних типов данных, чем для других
</v-click>

<br>
<br>
<br>
<v-click at="2">

### Некоторые данные предполагают <span v-mark="{ at: 3, color: 'green', type: 'underline' }">привычное</span> отображение, которое наш мозг ожидает увидеть в контексте этих данных
</v-click>

---

<figure>
  <img src="/natural_mappings.svg" style="width: 685px !important">
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -20px; left: 750px;">Источник: <a href="https://github.com/eamonnmag/Visualization-Course">Eamonn Maguire</a>
  </figcaption>
</figure>

---

# Popout эффект

#### Когда мы осматриваем изображения, некоторые визуальные элементы выделяются больше других. Почему?

* Параллельная обработка визуальной информации по многим каналам
	* скорость не зависит от количества отвлекающих элементов
	* скорость зависит от канала и степени его отличия от остального
* Последовательный поиск (многих) комбинаций
	* скорость значительно зависит от количества отвлекающих элементов

---

<center>
<div class="grid grid-cols-[5fr_5fr] gap-10">
<div v-click at="1">
<figure>
  <img src="/popout_1.svg" style="width: 240px !important;">
</figure>
</div>
<div v-click at="2">
<figure>
<img src="/popout_2.svg" style="width: 240px !important;">
</figure>
</div>
</div>
<br>
<br>

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div v-click at="3">
<figure>
  <img src="/popout_3.svg" style="width: 240px !important;">
</figure>
</div>
<div v-click at="4">
<figure>
<img src="/popout_4.svg" style="width: 240px !important;">
</figure>
</div>
</div>
<br>
</center>

---

# Popout эффект

<center>
<figure>
<img src="/popout_6_examples.svg" style="width: 750px !important;">
</figure>
</center>

---

# Popout эффект

<br>
<figure>
<img src="/food_tracker.png" style="width: 520px !important;">
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -50px; left: 550px;">Источник:<br> <a href="https://www.nytimes.com/interactive/2015/11/17/health/wiredwell-food-diary-super-tracker.html">https://www.nytimes.com/interactive/2015/11/17/<br>health/wiredwell-food-diary-super-tracker.html</a>
</figcaption>
</figure>

---

# Сопоставление

<center>
<figure>
<img src="/relative_comparison_1.svg" style="width: 750px !important;">
</figure>
</center>

#### Помните про иллюзию [Эббингауза](https://ru.wikipedia.org/wiki/%D0%98%D0%BB%D0%BB%D1%8E%D0%B7%D0%B8%D1%8F_%D0%AD%D0%B1%D0%B1%D0%B8%D0%BD%D0%B3%D0%B0%D1%83%D0%B7%D0%B0)?

---

# Сопоставление

<center>
<figure>
<img src="/relative_comparison_2.svg" style="width: 750px !important;">
</figure>
</center>

---

# Сопоставление

<center>
<figure>
<img src="/alignment_1.svg" style="width: 750px !important;">
</figure>
</center>

---

# Сопоставление

<center>
<figure>
<img src="/alignment_2.svg" style="width: 750px !important;">
</figure>
</center>

---

# Сопоставление

<center>
<figure>
<img src="/relative_comparison_4.svg" style="width: 600px !important;">
</figure>
</center>

---

<figure>
<img src="/countries_health_wealth_2025.png" style="width: 730px !important;">
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -10px; left: 550px;">Источник: <a href="https://www.gapminder.org/fw/world-health-chart/whc2025/">https://www.gapminder.org/fw/world-health-chart/whc2025/</a>
</figcaption>
</figure>

---

# Сопоставление

<center>
<figure>
<img src="/relative_comparison_5.svg" style="height: 350px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 20px; left: 130px;">Источник данных:  <a href="http://vis.stanford.edu/files/2010-MTurk-CHI.pdf">Heer and Bostock (2010)</a><br>
  </figcaption>
</figure>
</center>

---
zoom: 1.1
--- 
# Факторы влияния на точность сопоставления

<br>

* Выровнены ли сравниваемые объекты?
* Есть ли вокруг отвлекающие объекты?
	* Сколько их?
* Расстояние между сравниваемыми обектами
* Общий масштаб изображения
