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
 center: [-22.91, -43.17],
 zoom: 8
 }),
 // Создаем круг
 myCircle = new ymaps.Circle([
 // Задаем координаты 
 [-22.91, -43.17],
13599]);
 
 myMap.geoObjects.add(myCircle);
 }
 </script>
</head>
<body>
<h2>Добавление круг на карту</h2>
<div id="map" style="width:600px;height:400px"></div>
</body>
</html>
