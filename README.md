## LM-CSS
![Logo de java](https://s0.smartresize.com/wallpaper/157/626/HD-wallpaper-java-glitter-logo-programming-language-grid-metal-background-java-creative-programming-language-signs-java-logo-thumbnail.jpg](https://1000logos.net/wp-content/uploads/2020/09/CSS-Logo-2011.png)
# Descripción
Este es mi examen de CSS y consiste en una paguina web hecha en CSS sobre recetas de cocina como unas lentejas.
---
## Esta formado por:
### ejercicio_b.html
```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <title>Recetas de la abuela</title>
  <link href="./css/ejercicio_b.css" rel="stylesheet" type="text/css">
</head>
<body>
  <header>
    <h1>Recetas de la abuela</h1>
  </header>

  <nav>
    <ul>
      <li><a href="#">Inicio</a></li>
      <li><a href="#">Recetas fáciles</a></li>
      <li><a href="#">Postres</a></li>
      <li><a href="#">Platos de fiesta</a></li>
      <li><a href="#">Consejos</a></li>
    </ul>
  </nav>

  <main>
    <article class="receta-destacada">
      <h2>Receta destacada: Lentejas estofadas</h2>
      <img src="img/tazon-de-lentejas-con-verduras.jpg" alt="Lentejas estofadas">
      <p class="introduccion">Un plato de cuchara tradicional, perfecto para los días fríos. Sencillo, nutritivo y lleno de sabor.</p>
    </article>

    <section class="categorias-recetas">
      <img src="img/recipes.png" alt="Categorías de recetas">
      <h2>Explora nuestras categorías</h2>
      <table class="tabla-categorias">
        <thead>
          <tr>
            <th>Categoría</th>
            <th>Descripción</th>
            <th>Enlace</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Sopas y cremas</td>
            <td>Calienta el cuerpo y el alma con nuestras reconfortantes recetas.</td>
            <td><a href="#" class="boton-categoria-tabla">Ver más</a></td>
          </tr>
          <tr>
            <td>Carnes y asados</td>
            <td>Desde guisos clásicos hasta asados para sorprender, ¡para los amantes de la carne!</td>
            <td><a href="#" class="boton-categoria-tabla">Ver más</a></td>
          </tr>
          <tr>
            <td>Postres caseros</td>
            <td>El final perfecto para cualquier comida, ¡dulces tentaciones que te encantarán!</td>
            <td><a href="#" class="boton-categoria-tabla">Ver más</a></td>
          </tr>
        </tbody>
      </table>
    </section>
  </main>

  <aside>
    <section class="formulario-busqueda">
      <h3>Buscar receta</h3>
      <form action="#" method="get">
        <label for="busqueda">Introduce ingredientes o nombre:</label>
        <input type="text" id="busqueda" name="busqueda" placeholder="Ej: pollo, postre, fácil">
        <input type="submit" value="Buscar" id="buscar">
      </form>
    </section>

    <h3>Recetas populares</h3>
    <ul>
      <li><a href="#">Tortilla de patatas</a></li>
      <li><a href="#">Paella valenciana</a></li>
      <li><a href="#">Tarta de manzana</a></li>
      <li><a href="#">Gazpacho andaluz</a></li>
    </ul>
    <h3>Síguenos en Redes</h3>
    <div class="redes-sociales">
      <a href="#"><img src="img/icono_facebook.png" alt="Facebook"></a>
      <a href="#"><img src="img/icono_instagram.png" alt="Instagram"></a>
      <a href="#"><img src="img/icono_twitter.png" alt="Twitter"></a>
    </div>
  </aside>

  <footer>
    <p>&copy;2025 Recetas de la abuela - Todos los derechos reservados</p>
  </footer>
</body>
</html>
```
---
### ejercicio_b.css
```css
body{
	 background: linear-gradient( to right , lightyellow, #f4e7d5);
	 font-family: georgian;
 }
header{
	 background-color: #a38260;
	 text-align: center;
	 color: white;
	 text-shadow: 0 3px 3px lightyellow;
	 padding: 10px;
 }
 
 nav ul{
	 list-style: none;
	 text-align: center;
	 background-color: #b38260;
	 padding: 15px;
 }
 
 nav ul li{
	 display: inline-block;
	 margin:  0 15px;
 }
 
 nav ul li a{
	 background-color: #8c6a4a;
	 border-radius: 5px;
	 padding: 10px;
	 color: rgb(255,255,255);
	 text-decoration: none;
 }
 
 nav ul li a:hover{
	 background-color: #6b4827;
	 text-decoration: underline;
 }
 
 nav ul li a:focus{
	 background-color: #6b4827;
	 text-decoration: underline;
 }
 
.receta-destacada{
	background-color: white;
	border-radius: 10px;
	box-shadow: 0px 4px 4px #888888;
	text-align: center;
	margin: 20px auto;
	width: 50%;
	padding: 10px;
 }
 
.receta-destacada h2:first-letter{
	 color: white;
	 background-color: #c05e39;
 }
 
 .receta-destacada h2:first-line{
	 color: #c05e39;
 }
 
 .receta-destacada img{
	 border-radius: 10px;
	 width: 50%;
 }
 
 .introduccion{
	 font-style: italic;
	 color: #555;
 }
 
 .categorias-recetas h2{
	 text-align: center;
 }
 .categorias-recetas h2:first-letter{
	 color: white;
	 background-color: #c05e39
 }
 
 .categorias-recetas h2:first-line{
	 color: #c05e39;
 }
 
 .categorias-recetas img{
	 float: left;
	 width:100px;
 }
 
 .tabla-categorias{
	 border-radius: 0px 0px 10px 10px;
	background-color:white;
	border-collapse: collapse;
	margin: 40px auto;
	width: 60%;
	box-shadow: 0px 4px 4px #888888;
 }
 
 .tabla-categorias td{
	 border-top: 1px solid #d0b49f;
 }
 
 .tabla-categorias th{
	 color: white;
	 background-color: #c05e39;
 }
 
 .boton-categoria-tabla{
	 background-color: #c05e39;
	 text-decoration: none;
	 color: white;
	 border-radius: 5px;
	 padding: 2px;
	 text-align: center;
 }
 main{
	 float: left;
	 width: 85%;
 }
 
 footer{
	 background-color: #a38260;
	 text-align: center;
	 color: white;
	 padding: 10px;
	 font-weight: bold;
 }
 
 footer{
	 clear: both;
 }
 
 aside{
	 float: right;
	 width: 12%;
	 background-color: #f4e7d5;
	 border-left: 1px solid #d0b49;
	 padding-right: 30px;
	 
 }
 
 .formulario-busqueda{
	 background-color: white;
	 box-shadow: 0px 4px 4px #888888;
	 border-radius: 10px;
	 padding: 5px;
 }
 
 .formulario-busqueda h3{
	color: #7a5230; 
	text-align: center;
 }
 
 .formulario-busqueda label{
	color: #7a5230;
 }
 
 #busqueda{
	box-shadow: 0px 4px 4px #888888;
	border-radius: 5px;
	width: 85%;
	padding: 9px;
	margin-bottom: 10px;
 }
 
 #buscar{
	 background-color: #8c6a4a;
	 border-radius: 5px;
	 width: 95%;
	 padding: 9px;
 }
 
 aside h3{
	color: #7a5230; 
 }
 
 aside ul li{
	 list-style-image: url(img/estrella.png);
 }
 
 aside ul li a{
	 text-decoration: none;
	 color: #7a5230; 
 }
 
 aside ul li a:hover{
	 text-decoration: underline; 
 }
 
 
