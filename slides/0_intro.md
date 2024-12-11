---
zoom: 0.94
--- 

# Для чего нужна визуализация данных? (см. [Лекцию 1](https://afonsky.github.io/hse-vis-2024-lecture1))

### Компьютерные системы **визуализации** создают наглядные представления наборов данных, позволяя людям выполнять задачи более эффективно
<br>

* Визуализация подходит, когда необходимо дополнить человеческие возможности, а не заменить людей алгоритмическими методами принятия решений
* Пространство возможных визуальных идиом большое, включает в себя задачи создания визуализаций и взаимодействия человека с визуализациями
* Многие визуализации специфичны для конкретных задач, а для других задач неэффективны
* С визуализацией связаны ограничения:
  * Человека
  * Компьютера
  * Дисплея / бумаги
* Визуальные идиомы можно анализировать

---

# Что мы визуализируем? (см. [Лекцию 2](https://afonsky.github.io/hse-vis-2024-lecture2))
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

# Как мы визуализируем? (см. [Лекцию 3](https://afonsky.github.io/hse-vis-2024-lecture3))
<br>
<div class="grid grid-cols-[5fr_2fr] gap-15">
<div>
<figure>
  <img src="/textbook/fig_3.7_1.svg" style="width: 650px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 40px; left: 0px;">Источники данных:<br>
  <a href="https://www.cs.ubc.ca/~tmm/vadbook/">Рис. 3.7. T. Munzner. Visualization Analysis and Design.<br> A K Peters Visualization Series, CRC Press, 2014</a>
  <a href="http://euclid.psych.yorku.ca/www/psy6135/papers/ClevelandMcGill1984.pdf">Cleveland and McGill (1984)</a><br>
  <a href="http://vis.stanford.edu/files/2010-MTurk-CHI.pdf">Heer and Bostock (2010)</a><br>
  <a href="https://dl.acm.org/doi/10.1145/22949.22950">MacKinley (1986)</a><br>
  <a href="https://github.com/eamonnmag/Visualization-Course">Eamonn Maguire (агрегация)</a>
  </figcaption>
</figure>
</div>
<div>
<v-click>
<figure>
<br>
<img src="/Suitability_1_crop.svg" style="width: 250px !important;">
</figure>
</v-click>
</div>
</div>

---
zoom: 0.97
---

# Как использовать цвет? (см. [Лекцию 4](https://afonsky.github.io/hse-vis-2024-lecture4))

<div class="grid grid-cols-[5fr_4fr] gap-20">
<div>

* Взаимодействие цветовых каналов
  * Размер области сильно влияет на воспринимаемую насыщенность
      * Маленькие области требуют высокой насыщенности
      * Большие области нуждаются в низкой насыщенности

</div>
<div>
<br>
<figure>
  <img src="/HSL.svg" style="width: 480px !important;">
</figure>
</div>
</div>

* Насыщенность и освещенность:
  * неразделимы
  * также не отделимы от прозрачности
  * маленькие разделенные области: рекомендуется использовать 2 бина (либо насыщенность, либо освещенность, но не вместе), в крайнем случае < 3-4 бинов
  * смежные области: много бинов (используйте только один из этих каналов)

---

# Как мы визуализируем?
<br>

<figure>
  <img src="/textbook/fig_3.7.svg" style="width: 900px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -10px; left: 500px;">Источник данных: <a href="https://www.cs.ubc.ca/~tmm/vadbook/">Рис. 3.7. T. Munzner. Visualization Analysis and Design</a>
  </figcaption>
</figure>

---

# Различение визуальной информации
<br>
<br>
<br>

<figure>
  <img src="/textbook/fig_3.7_2.svg" style="width: 900px !important;">
</figure>

---

# Сопоставление однородных данных

<br>

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div>
<figure>
  <img src="/meteoblue_2.png" style="width: 480px !important;">
</figure>
</div>
<div>
<figure>
  <img src="/meteoblue_3.png" style="width: 480px !important;">
</figure>
</div>
</div>

<br>

<figure>
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;">Источник данных: <a href="https://www.meteoblue.com/ru/%D0%BF%D0%BE%D0%B3%D0%BE%D0%B4%D0%B0/historyclimate/">meteoblue</a>
  </figcaption>
</figure>

---

# Сопоставление разнородных данных

<br>

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div>
<figure>
  <img src="/meteoblue_2.png" style="width: 480px !important;">
</figure>
</div>
<div>
<figure>
  <img src="/meteoblue_4.png" style="width: 480px !important;">
</figure>
</div>
</div>

<br>

<figure>
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;">Источник данных: <a href="https://www.meteoblue.com/ru/%D0%BF%D0%BE%D0%B3%D0%BE%D0%B4%D0%B0/historyclimate/">meteoblue</a>
  </figcaption>
</figure>

---

# Пример сопоставления: связанное выделение

<br>

<div class="grid grid-cols-[6fr_5fr_5fr] gap-5">
<div>

* Позволяет видеть,<br> как объекты и области,<br> смежные в одном представлении,<br> распределены в другом
  * Эффективная и широко распространенная<br> *идиома взаимодействия*
</div>
<div>
<figure>
  <img src="/EDV_1.png" style="width: 256px !important;">
</figure>
</div>
<div>
<figure>
  <img src="/EDV_2.png" style="width: 260px !important;">
</figure>
</div>
</div>

<br>

<figure>
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;">Источник изображений:
Visual Exploration of Large Structured Datasets.Wills. Proc. New Techniques
and Trends in Statistics (NTTS), pp. 237–246. IOS Press, 1995
</figcaption>
</figure>

---

# Пример сопоставления: связанное выделение

<figure>
  <img src="/improvise.png" style="width: 670px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;">Источник изображения: <a href="https://www.cs.ou.edu/~weaver/improvise/examples/census/index.html">https://www.cs.ou.edu/~weaver/improvise/examples/census/index.html</a>
</figcaption>
</figure>

---

# Пример множественного сопоставления

<figure>
  <img src="/scatterplot_D3.png" style="width: 400px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 500px;">Источник изображения: <a href="https://observablehq.com/@d3/splom">https://observablehq.com/@d3/splom</a>
  </figcaption>
</figure>

---

# Пример множественного сопоставления

<figure>
  <img src="/NN_1.png" style="width: 600px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -30px; left: 700px;">Источник изображения: А.Б.
  </figcaption>
</figure>

---

# Мини-диаграммы

#### Известны как [small multiple](https://en.wikipedia.org/wiki/Small_multiple)

<br>

<figure>
  <img src="/The_Horse_in_Motion.jpg" style="width: 620px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -50px; left: 650px;">Источник изображения:<br> <a href="http://loc.gov/pictures/resource/cph.3a45870/">Eadweard Muybridge, Horse In Motion (1878)</a>
  </figcaption>
</figure>

---

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div>
<figure>
  <img src="/Persons_With_Gainful_Occupations_and_Attending_School_in_1870.jpg" style="width: 350px !important;">
    <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 15px; left: 0px;">Источник изображений: <a href="https://www.loc.gov/maps/?fa=segmentof%3Ag3701gm.gct00297%2F%7Ccontributor%3Awalker%2C+francis+amasa&sb=shelf-id&st=gallery&sb=shelf-id&c=160">US Ninth Census 1870. Francis A. Walker</a>
  </figcaption>
</figure>
</div>
<div>
<figure>
  <img src="/iiif-service_gmd_gmd370m_g3701m_g3701gm_gct00297_ca000093-full-pct_12.5-0-default.jpg" style="width: 350px !important;">
</figure>
</div>
</div>

---

# Выбор визуального решения для сопоставления
<br>
<br>

<figure>
  <img src="/textbook/fig_12.6.svg" style="width: 600px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 90px; left: 500px;">Источник данных: <a href="https://www.cs.ubc.ca/~tmm/vadbook/">Рис. 12.6. T. Munzner. Visualization Analysis and Design</a>
  </figcaption>
</figure>

---

# Сопоставление

* Использование поля зрения вместо памяти
  * Меньшая когнитивная нагрузка при перемещении глаз между несколькими визуализациями, чем при запоминании предыдущих визуализаций

* Можно сопоставлять **однородную** и **разнородную** информацию
  * Для разнородной информации нужна общая шкала по одной из осей<br> или связанное выделение

* Можно сопоставлять множество визуализаций сразу
  * Насколько много? Это открытый вопрос для исследований

* Недостатки
  * Ограниченная доступная площадь экрана
  * Ограниченная точность сопоставления

---

# Различение визуальной информации
<br>
<br>

<figure>
  <img src="/textbook/fig_3.7_3.svg" style="width: 900px !important;">
</figure>
<br>

* Вид
  * Относительно большая область, в которой данные отображаются на дисплее
* [Глиф](https://en.wikipedia.org/wiki/Glyph_(data_visualization))
  * Небольшой объект с внутренней структурой

---
zoom: 0.84
--- 

# Разделение в визуализации

<div class="grid grid-cols-[5fr_5fr] gap-6">
<div>

#### Единая гистограмма со сгруппированными столбцами
* Разделение областей по штатам
* Внутри каждой области расположен сложный *глиф*, показывающий возраст
* Сравнение: легко между штатами, сложно по возрастам
<figure>
  <img src="/partitioning_1.svg" style="width: 320px !important;">
</figure>
</div>
<div>

<br>

#### Гистограммы с небольшим количеством элементов
* Разделение видов по возрасту
* Одна диаграмма на область
* Сравнение: легко в пределах возраста, сложнее по штатам
<figure>
  <img src="/partitioning_2.svg" style="width: 320px !important;">
</figure>
</div>
</div>

<figure>
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 20px; left: 0px;">Источник изображений: <a href="https://gist.github.com/mbostock/3887051">https://gist.github.com/mbostock/3887051</a>
</figcaption>
</figure>

---

# О глифах

<div class="grid grid-cols-[3fr_5fr] gap-15">
<div>

#### Не только маркеры
<br>
<figure>
  <img src="/matplotlib_marker_examples.png" style="width: 350px !important;">
</figure>
<br>
<v-click at="2">
<figure>
  <img src="/meteoblue_glyphs_1.png" style="width: 400px !important;">
</figure>
</v-click>
</div>
<div>
<v-click at="3">
<figure>
  <img src="/meteoblue_glyphs_2.png" style="width: 450px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 15px; left: 0px;">Источники изображений:<br>
  <a href="https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_star_poly.html">https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_star_poly.html</a> (слева вверху)<br>
  <a href="https://www.meteoblue.com/ru/%D0%BF%D0%BE%D0%B3%D0%BE%D0%B4%D0%B0/historyclimate/weatherarchive/%d0%91%d0%b0%d0%b7%d0%b5%d0%bb%d1%8c_%d0%a8%d0%b2%d0%b5%d0%b9%d1%86%d0%b0%d1%80%d0%b8%d1%8f_2661604?fcstlength=1y&year=2024&month=12">https://www.meteoblue.com/погода/historyclimate/weatherarchive/</a> (слева внизу)<br>
  <a href="https://www.meteoblue.com/ru/%D0%BF%D0%BE%D0%B3%D0%BE%D0%B4%D0%B0/%D0%BD%D0%B5%D0%B4%D0%B5%D0%BB%D1%8F/%d0%9c%d0%be%d1%81%d0%ba%d0%b2%d0%b0_%d0%a0%d0%be%d1%81%d1%81%d0%b8%d1%8f_524901">https://www.meteoblue.com/ru/погода/неделя/Москва_Россия_524901</a> (справа)
</figcaption>
</figure>
</v-click>
</div>
</div>

<v-click at="4">
<figure>
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 15px; left: 0px;">Источники изображений:<br>
  <a href="https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_star_poly.html">https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_star_poly.html</a> (слева)<br>
  <a href="https://stackoverflow.com/questions/29866592/draw-a-plot-of-glyphs-in-matplotlib">https://stackoverflow.com/questions/29866592/draw-a-plot-of-glyphs-in-matplotlib</a> (справа вверху)<br>
  <a href="https://www.meteoblue.com/ru/%D0%BF%D0%BE%D0%B3%D0%BE%D0%B4%D0%B0/historyclimate/weatherarchive/%d0%91%d0%b0%d0%b7%d0%b5%d0%bb%d1%8c_%d0%a8%d0%b2%d0%b5%d0%b9%d1%86%d0%b0%d1%80%d0%b8%d1%8f_2661604?fcstlength=1y&year=2024&month=12">https://www.meteoblue.com/погода/historyclimate/weatherarchive/</a> (справа)
</figcaption>
</figure>
</v-click>

---

# О глифах: тензорные глифы

<div class="grid grid-cols-[5fr_3fr] gap-2">
<div>
<figure>
  <img src="/glyphs_complicated.jpg" style="width: 600px !important;">
</figure>
<br>
<figure>
  <img src="/glyphs_ellipsoids.png" style="width: 320px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 30px; left: 0px;">Источник изображений:<br> <a href="https://people.cs.uchicago.edu/~glk/pubs/pdf/Kindlmann-Superquad1-VisSym-2004.pdf">Gordon Kindlmann. Superquadric tensor glyphs (2004)
</a>
  </figcaption>
</figure>
</div>
<div>
<figure>
  <img src="/glyphs_superquadrics.png" style="width: 264px !important;">
</figure>
</div>
</div>

---

# Различение визуальной информации
<br>
<br>
<br>

<figure>
  <img src="/textbook/fig_3.7_4.svg" style="width: 900px !important;">
</figure>

---

# Наложение слоев

* Cлой - набор объектов, распределенных по видимой области
  * Каждый набор представляет собой визуально различимую группу
  * Масштаб: целиком

* Выбор средств визуализации
  * Сколько слоев, как их различать?
    * Следует кодировать при помощью различимых каналов

---

# Наложение слоев

<br>

<div class="grid grid-cols-[5fr_5fr_5fr] gap-5">
<div>
<figure>
  <img src="/map_layer_1c.jpg" style="width: 300px !important;">
</figure>
</div>
<div>
<figure>
  <img src="/map_layer_2c.jpg" style="width: 300px !important;">
</figure>
</div>
<div>
<figure>
  <img src="/map_layer_3c.jpg" style="width: 300px !important;">
</figure>
</div>
</div>

<br>

<figure>
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 0px; left: 0px;">Источник изображений: <a href="https://yandex.ru/maps/2/saint-petersburg/?ll=30.356718%2C59.942538&z=14">Яндекс.Карты</a>
</figcaption>
</figure>

---

# Совмещение визуальной информации

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div>

* Ограничения:
  * 2-3 слоя
  * < 30 линий
    * Различных по цвету и начертанию

* Сопоставление и совмещение:
  * Сравнение нескольких мини-диаграмм и одной совмещенной диаграммы
  * Мини-диаграммы лучше подходят для выявление общего различия
  * Совмещенная диаграмма для поиска различий в деталях

</div>
<div>
<figure>
  <img src="/meteoblue_6.png" style="width: 500px !important;">
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 20px; left: 0px;">Источник данных: <a href="https://www.meteoblue.com/ru/погода/прогноз/multimodel/Гибралтар_Гибралтар_2411585">meteoblue</a>
</figcaption>
</figure>
</div>
</div>

---
zoom: 0.97
--- 

# Совмещение или сопоставление?

<figure>
  <img src="/pc_games_lines.png" style="width: 600px !important;">
  <figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: -40px; left: 700px;">Источник примера: <a href="https://github.com/eamonnmag/Visualization-Course">Eamonn Maguire</a>
</figcaption>
</figure>

<v-clicks depth="2">

* Такую визуализацию очень трудно воспринять
  1. Слишком много цветов (не все различимы)
  2. Слишком много пересекающихся линий (трудно увидеть непрерывность)
  3. Сложно сопоставить линии с легендой
</v-clicks>

---

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div>
<figure>
  <img src="/pc_games_small_multiples.png" style="width: 390px !important;">
</figure>


</div>
<div>
<v-clicks depth="2">

* Намного лучше

* Разделение подобных данных на мини-диаграммы, как правило, является удачной практикой, если у вас много данных

* Но видите ли вы здесь проблемы?
  * Масштабы осей различные от графика к графику
  * Цвет не несет информации
</v-clicks>
<figure>
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 140px; left: 0px;">Источник примера: <a href="https://github.com/eamonnmag/Visualization-Course">Eamonn Maguire</a>
</figcaption>
</figure>
</div>
</div>

---

<div class="grid grid-cols-[5fr_5fr] gap-10">
<div>
<figure>
  <img src="/pc_games_small_multiples_2.png" style="width: 390px !important;">
</figure>


</div>
<div>
<v-clicks depth="2">

* Теперь данные легче сравнить

* Но нельзя ли сделать ещё более эффективное сравнение?
</v-clicks>
<figure>
<figcaption style="color:#b3b3b3ff; font-size: 11px; position: relative; top: 140px; left: 0px;">Источник примера: <a href="https://github.com/eamonnmag/Visualization-Course">Eamonn Maguire</a>
</figcaption>
</figure>
</div>
</div>