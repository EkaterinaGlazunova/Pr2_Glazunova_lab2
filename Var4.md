# Pr2_Glazunova_lab2
<html xmlns="http://www.w3.org/1999/xhtml">
 <head>    
 <title>Примеры. Добавление треугольника на карту.</title>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>  
 <!--         Подключаем API карт 2.x
  Параметры:
  - load=package.full - полная сборка;
  - lang=ru-RU - язык русский.     -->
<script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU"
type="text/javascript"></script>
<script type="text/javascript"> 
ymaps.ready(init);  
 function init() { 
 var myMap = new ymaps.Map('map', { 
 center: [65.5093, -151.3900], 
 zoom: 8         
 }),            
                 
 myPolygon = new ymaps.Polygon([[
// Координаты Треугольника.
[65.417113, -150.978996], 
[65.409101, -151.64092],
[65.657369, -151.300342],			
]]);

 myMap.geoObjects.add(myPolygon)
                 .add(myPolygon); 
 }    
 </script> 
</head>  
<body> 
<h2>Добавление треугольника на карту</h2>  
<div id="map" style="width:600px;height:400px"></div> </body>  
</html>  
 
