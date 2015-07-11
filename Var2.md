# Pr2_Glazunova_lab2
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
 <title>Примеры. Добавление прямоугольника на карту.</title>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
 <!--
 Подключаем API карт 2.x
 Параметры:
 - load=package.full - полная сборка;
 - lang=ru-RU - язык русский.
 -->
 <script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU"
 type="text/javascript"></script>
 <script type="text/javascript">
 // Как только будет загружен API и готов DOM, выполняем инициализацию
 ymaps.ready(init);
 function init() {
 var myMap = new ymaps.Map('map', {
 center: [-25.29, -57.62],
 zoom: 10
 }),
 // Создаем шестигранник
 myPolygon = new ymaps.Polygon([[


 // Задаем координаты 
[-25.349931, -57.674851],
[-25.274409, -57.7291], 
[-25.209464, -57.659067], 
[-25.201960, -57.554692], 
[-25.271288, -57.501134],
[-25.348682, -57.555375],
]]);

 
myMap.geoObjects.add(myPolygon)
                 .add(myPolygon);
 }
 </script>
</head>
<body>
<h2>Добавление шестигранника на карту</h2>
<div id="map" style="width:600px;height:400px"></div>
</body>
</html>
