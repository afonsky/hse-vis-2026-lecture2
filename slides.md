---
theme: seriph
addons:
  - "@twitwi/slidev-addon-ultracharger"
addonsConfig:
  ultracharger:
    inlineSvg:
      markersWorkaround: false
    disable:
      - metaFooter
      - tocFooter
background: /midjourney_eye.jpg
highlighter: shiki
routerMode: hash
lineNumbers: false

css: unocss
title: Научная визуализация данных
subtitle: Лекция 2. Зрительная система человека
date: 12/11/2026
venue: ВШЭ
author: Алексей Болдырев
---

<br>
<br>

# <span style="font-size:28.0pt" v-html="$slidev.configs.title?.replaceAll(' ', '<br/>')"></span>
# <span style="font-size:28.0pt" v-html="$slidev.configs.subtitle?.replaceAll(' ', '<br/>')"></span>
# <span style="font-size:18.0pt" v-html="$slidev.configs.author?.replaceAll(' ', '<br/>')"></span>

<span style="font-size:18.0pt" v-html="$slidev.configs.date?.replaceAll(' ', '<br/>')"></span>

<br>

<div>
<span style="color:#b3b3b3ff; font-size: 11px; float: right;">Изображение: Midjourney 6.0. Запрос "Eye and data visualization"
</span>
</div>

<style>
  :deep(footer) { padding-bottom: 3em !important; }
</style>

---
src: ./slides/0_outline.md
---

---
src: ./slides/1_learning_outcomes.md
---

---
src: ./slides/0_intro.md
---

---
src: ./slides/1_marks_and_channels.md
---

---
src: ./slides/1_piecharts.md
---

---
src: ./slides/1_piecharts_takeaway.md
---

---
src: ./slides/2_barcharts.md
---

---
src: ./slides/3_mapping_data.md
---

---
src: ./slides/3_perception_takeaway.md
---

---
src: ./slides/4_summary.md
---

---
src: ./slides/0_end.md
---