---
zoom: 0.9
---

# Определение визуализации данных (см. [Лекцию 1](https://afonsky.github.io/hse-vis-nn-2026-lecture1))

<div class="mt-3 bg-blue-50 dark:bg-blue-900 rounded p-3 text-sm">

### 📌 Компьютерные системы **визуализации** создают наглядные представления наборов данных, позволяя людям выполнять задачи более эффективно
</div>
<br>

* Визуализации дополняют человеческие возможности
* Существует множество визуальных идиом (концепций)
  * Создание визуализации
  * Взаимодействие с визуализацией
* Визуализации специфичны для конкретных задач
* С визуализацией связаны ограничения:
	* Человека
	* Компьютера
	* Носителя (экрана / бумаги)
* Визуальные идиомы можно анализировать

---

# Что мы визуализируем? (см. [Лекцию 1](https://afonsky.github.io/hse-vis-nn-2026-lecture1))
<br>
<div class="grid grid-cols-[5fr_2fr] gap-15">
<div>
<figure>
  <img src="/textbook/fig_2.1_1.svg" style="width: 650px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -60px; left: 620px;">Источник:<br> <a href="https://www.cs.ubc.ca/~tmm/vadbook/">Рис. 2.1. T. Munzner. Visualization Analysis and Design.<br> A K Peters Visualization Series, CRC Press, 2014</a>
  </figcaption>
</figure>
</div>
<div>
<figure>
<br>
<img src="/textbook/fig_2.1_2.svg" style="width: 150px !important;">
</figure>
</div>
</div>

---
zoom: 0.83
--- 

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-gom2{border-color:inherit;font-size:medium;text-align:center;vertical-align:top}
</style>
<table class="tg"><thead>
  <tr>
    <th class="tg-gom2">JAN</th>
    <th class="tg-gom2">FEB</th>
    <th class="tg-gom2">MAR</th>
    <th class="tg-gom2">APR</th>
    <th class="tg-gom2">MAY</th>
    <th class="tg-gom2">JUN</th>
    <th class="tg-gom2">JUL</th>
    <th class="tg-gom2">AUG</th>
    <th class="tg-gom2">SEP</th>
    <th class="tg-gom2">OCT</th>
    <th class="tg-gom2">NOV<br></th>
    <th class="tg-gom2">DEC</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-gom2">2</td>
    <td class="tg-gom2">10</td>
    <td class="tg-gom2">4</td>
    <td class="tg-gom2">5</td>
    <td class="tg-gom2">6</td>
    <td class="tg-gom2">9</td>
    <td class="tg-gom2">1</td>
    <td class="tg-gom2">3</td>
    <td class="tg-gom2">5</td>
    <td class="tg-gom2">3</td>
    <td class="tg-gom2">4</td>
    <td class="tg-gom2">7</td>
  </tr>
</tbody>
</table>
<br>

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div v-click at="1">
<figure>
  <img src="/year_1.svg" style="width: 450px !important;">
</figure>
</div>
<div v-click at="2">
<figure>
<img src="/year_2.svg" style="width: 450px !important;">
</figure>
</div>
</div>
<br>

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div v-click at="3">
<figure>
  <img src="/year_3.svg" style="width: 450px !important;">
</figure>
</div>
<div v-click at="4">
<figure>
<img src="/year_4.svg" style="width: 450px !important;">
</figure>
</div>
</div>
<br>

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div v-click at="5">
<figure>
  <img src="/year_5.svg" style="width: 450px !important;">
</figure>
</div>
<div v-click at="6">
<figure>
<img src="/year_6.svg" style="width: 450px !important;">
</figure>
</div>
</div>
<br>

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div v-click at="7">
<figure>
  <img src="/year_7.svg" style="width: 450px !important;">
</figure>
</div>
<div v-click at="8">
<figure>
<img src="/year_8.svg" style="width: 450px !important;">
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 7px; left: 250px;">Источник: <a href="https://github.com/eamonnmag/Visualization-Course">Eamonn Maguire</a>
  </figcaption>
</figure>
</div>
</div>

---

<br>
<br>

## И это простой пример визуализации данных низкой размерности

<br>
<br>

### Все эти визуализации кодируют информацию, но ошибка декодирования (интерпретация, сравнение, ...) для каждого графика оказывается своя
<br>
<br>

## Но почему?

---
zoom: 0.96
--- 

# Как оптимально кодировать информацию?

### Если не знать значения слов и не соблюдать грамматические правила, смысл текста может быть утерян
<br>
<center>
<figure>
<img src="/encoder_decoder.svg" style="width: 850px !important;">
</figure>
</center>
<br>
<br>

### Это касается и визуализаций. Мы можем создавать визуальные образы, используя **словарь** (формы, цвет, текстура...) и **грамматику**. Если мы выучим их, то сможем добиться большего в визуальной коммуникации

---
zoom: 0.9
---

# Как оптимально кодировать информацию?

<v-clicks depth="2">

* Важность <span v-mark="{ at: 2, color: 'orange', type: 'underline' }">ошибки восприятия</span> всегда должна быть сбалансирована с целью и задачей
* Часто нам не требуются точные значения, а особенности восприятия не имеют значения
  * Но иногда они важны
</v-clicks>
<br>
<v-click>
<div class="grid grid-cols-[5fr_5fr] gap-25">
<div>

#### Шрифт Helvetica
<SPAN style="font-family:'Helvetica';font-size:250%;background-color:cornsilk">x14l38I0nO</SPAN>

</div>
<div>


#### Шрифт Liberation
<SPAN style="font-family:'Liberation Mono';font-size:250%;background-color:cornsilk">x14l38I0nO</SPAN>
</div>
</div>
</v-click>
<br>

<v-clicks depth="2">

* Если это мой пароль, то ОК (нужно просто его запомнить)
* Если это пароль Wi-Fi для посетителей кофейни, то, возможно, нет
  * Есть путаница между верхним регистром `i` и нижним регистром `L`
  * Расстояние между символами может привести к ошибкам в интерпретации, что вызывает
разочарование клиентов кофейни
</v-clicks>

<!--
В каких ещё символах может возникнуть путаница?
-->

---
zoom: 0.96
---

# Как оптимально кодировать информацию?
<br>
<center>
<figure>
  <img src="/textbook/fig_3.7_1.svg" style="width: 850px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 20px; left: 150px;">Источник: <a href="https://www.cs.ubc.ca/~tmm/vadbook/">Рис. 3.7. T. Munzner. Visualization Analysis and Design. A K Peters Visualization Series, CRC Press, 2014</a>
  </figcaption>
</figure>
</center>
<!--
Давайте начнём с мостика между данными и их отображением. Это организация данных.
-->

---
zoom: 0.9
---

# Наше восприятие нелинейно

### Некоторые стимулы воспринимаются сильнее либо слабее, чем мы ожидаем
<br>
<div class="grid grid-cols-[5fr_5fr] gap-10">
<div>
<figure>
  <img src="/Stevens_law.svg" style="width: 370px">
</figure>
</div>
<div>
<div class="grid grid-cols-[5fr_5fr] gap-10">
<div>
<figure>
  <img src="/midjourney_handle.jpg" style="height: 220px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 5px; left: 0px;">Midjourney 6, запрос: "handle of 1950s electronic equipment"
  </figcaption>
</figure>
</div>
<div>
<figure>
  <img src="/SmittyStevens.jpg" style="height: 220px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;">Стэнли Стивенс (1906-1973)
</figcaption>
</figure>
</div>
</div>
<br>


#### [Психофизический закон Стивенса (1957)](https://ru.wikipedia.org/wiki/%D0%97%D0%B0%D0%BA%D0%BE%D0%BD_%D0%A1%D1%82%D0%B8%D0%B2%D0%B5%D0%BD%D1%81%D0%B0):
* Длина воспринимается линейно
* Прочие ощущения воспринимаются<br> по степенному закону $S = I^n$
</div>
</div>

---

# Следствия закона Стивенса для визуализации
<br>
<br>
<br>
<v-click>

### 1. Нужно внимательно сопоставлять данные с их восприятием
</v-click>
<br>
<br>
<br>
<v-click>

### 2. Некоторые **визуальные каналы** более эффективны<br> для одних типов данных, чем для других
</v-click>

---

<figure>
  <img src="/Suitability_1.svg" style="width: 810px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -80px; left: 550px;">Источники данных:<br>
  <a href="http://euclid.psych.yorku.ca/www/psy6135/papers/ClevelandMcGill1984.pdf">Cleveland and McGill (1984)</a><br>
  <a href="http://vis.stanford.edu/files/2010-MTurk-CHI.pdf">Heer and Bostock (2010)</a><br>
  <a href="https://dl.acm.org/doi/10.1145/22949.22950">MacKinley (1986)</a><br>
  <a href="https://github.com/eamonnmag/Visualization-Course">Eamonn Maguire (агрегация)</a>
  </figcaption>
</figure>

---

<figure>
  <img src="/Suitability_2.svg" style="width: 810px !important;">
</figure>

---

<figure>
  <img src="/Suitability_3.svg" style="width: 810px !important;">
</figure>

---
zoom: 0.85
--- 

# Измерение восприятия визуализации
<div class="grid grid-cols-[5fr_3fr] gap-10">
<div>
<br>
<figure>
  <img src="/Optimal_encoding.svg" style="width: 650px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 430px;"><br>Источники данных:<br>
  <a href="http://euclid.psych.yorku.ca/www/psy6135/papers/ClevelandMcGill1984.pdf">Cleveland and McGill (1984)</a><br>
  <a href="http://vis.stanford.edu/files/2010-MTurk-CHI.pdf">Heer and Bostock (2010)</a><br>
  </figcaption>
</figure>
</div>
<div>

#### Детали эксперимента (2010):

* Использовалась краудсорсинговая площадка [Amazon Mechanical
Turk](https://ru.wikipedia.org/wiki/Amazon_Mechanical_Turk)
* 550 исполнителей-"туркеров"
  * Проходили квалификацию
  * Получали награду от $0.02 до $0.05 за действие

<center>
<figure>
  <img src="/2010_MTurk.png" style="width: 250px !important;">
</figure>
</center>
</div>
</div>

<!--
Для каждой диаграммы N=50 испытуемым предлагалось сначала определить меньшее из двух отмеченных значений, а затем «быстрым взглядом» оценить, какой процент меньшее составляет от большего. Первый вопрос служил лишь для проверки ответов; только 14 из 3481 испытуемых ответили неверно (0,4%).
-->

---

# Оптические иллюзии

<br>
<div class="grid grid-cols-[5fr_5fr] gap-20">
<div>
<figure>
  <img src="/Mond-vergleich.svg" style="width: 300px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;"><a href="https://ru.wikipedia.org/wiki/%D0%98%D0%BB%D0%BB%D1%8E%D0%B7%D0%B8%D1%8F_%D0%AD%D0%B1%D0%B1%D0%B8%D0%BD%D0%B3%D0%B0%D1%83%D0%B7%D0%B0">Иллюзия Эббингауза</a>
  </figcaption>
</figure>
<br>
<figure>
  <img src="/Ponzo_illusion.gif" style="width: 200px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;"><a href="https://ru.wikipedia.org/wiki/%D0%98%D0%BB%D0%BB%D1%8E%D0%B7%D0%B8%D1%8F_%D0%9F%D0%BE%D0%BD%D1%86%D0%BE">Иллюзия Понцо</a>
  </figcaption>
</figure>
</div>
<div>
<figure>
  <img src="/Delboeuf_illusion.svg" style="width: 300px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;"><a href="https://ru.wikipedia.org/wiki/%D0%98%D0%BB%D0%BB%D1%8E%D0%B7%D0%B8%D1%8F_%D0%94%D0%B5%D0%BB%D1%8C%D0%B1%D1%91%D1%84%D0%B0">Иллюзия Дельбёфа</a>
  </figcaption>
</figure>
<br>
<figure>
  <img src="/rails.png" style="width: 400px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;"><a href="https://ru.wikipedia.org/wiki/%D0%98%D0%BB%D0%BB%D1%8E%D0%B7%D0%B8%D1%8F_%D0%BD%D0%B0%D0%BA%D0%BB%D0%BE%D0%BD%D0%BD%D0%BE%D0%B9_%D0%B1%D0%B0%D1%88%D0%BD%D0%B8">Иллюзия наклонной башни</a>
  </figcaption>
</figure>
</div>
</div>

---

<center>
<figure>
  <img src="/9_purple_dots.png" style="width: 330px !important; position: relative; top: -30px">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -60px; left: 300px;">Источник изображения:<br><a href="https://arxiv.org/abs/2509.11582">arXiv:2509.11582</a>
  </figcaption>
</figure>
</center>

---

# Оптические иллюзии

<center>
<figure>
  <img src="/9_purple_dots_2.png" style="width: 900px !important">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 300px;">Источник изображений:<a href="https://arxiv.org/abs/2509.11582">arXiv:2509.11582</a>
  </figcaption>
</figure>
</center>

---

# Оптические иллюзии: шкатулка
<div class="grid grid-cols-[5fr_4fr] gap-5">
<div>
<figure>
  <img src="/Coffer_illusion.jpg" style="width: 400px !important">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 20px; left: 0px;">Источник изображения:<a href="https://illusionoftheyear.com/2006/05/coffer-illusion/">https://illusionoftheyear.com/2006/05/coffer-illusion/</a>
  </figcaption>
</figure>
</div>
<div>

<div v-click at="1">

##### Восприятие зависит от культурных различий
<br>
<br>
<figure>
  <img src="/Coffer_illusion_2.png" style="width: 400px !important">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 20px; left: 0px;">Источник изображения:<a href="https://osf.io/preprints/psyarxiv/2pu6f_v1">https://osf.io/preprints/psyarxiv/2pu6f_v1</a>
  </figcaption>
</figure>
</div>
</div>
</div>