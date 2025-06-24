# Clase de Javascript

## ¿Qué es Javascript?
Consulta en: [https://www.w3schools.com/js/default.asp](https://www.w3schools.com/js/default.asp)

## ¿Qué es el DOM?
Consulta en: [https://www.w3schools.com/js/js_htmldom.asp](https://www.w3schools.com/js/js_htmldom.asp)

---

## 📄 Recursos de la clase

- 👉 [Ejercicios en consola](docs/ejercicios_en_consola.pdf)

[![Estructura de directorio](docs/estructura_directorio.JPG)](docs/estructura_directorio.JPG)

- 👉 [Practica Javascript condiciones y ciclos](docs/guia_practica_cond_ciclos_DOM.pdf)

---

## 📚 Librería de Javascript para sliders
1 Sitio de librería de javascript para sliders
```
https://splidejs.com/
```
2 En el html dentro de head
```
<link href="https://cdn.jsdelivr.net/npm/@splidejs/splide@4.1.4/dist/css/splide-core.min.css" rel="stylesheet"> <link href="https://cdn.jsdelivr.net/npm/@splidejs/splide@4.1.4/dist/css/themes/splide-sea-green.min.css" rel="stylesheet">
```
3 En el html antes de cerrar el body, se pega arriba del script slider.js
```
<script src="https://cdn.jsdelivr.net/npm/@splidejs/splide@4.1.4/dist/js/splide.min.js"></script>
```
4 En el html dentro del body, se le coloca un id para identificar al section
```
<section id="galeria" class="splide" aria-label="Splide Basic HTML Example"> <div class="splide__track"> <ul class="splide__list"> <li class="splide__slide">Slide 01</li> <li class="splide__slide">Slide 02</li> <li class="splide__slide">Slide 03</li> </ul> </div> </section>
```

5 Dentro del archivo slider.js
```
new Splide('#galeria', {
perPage: 3,
perMove: 1
}).mount();
```
6 Dentro del archivo de slider.css
```
.card {
background-color: #ffffff;
border-radius: 10px;
height: 600px;
padding: 40px;
box-shadow: 0 0 15px rgba(0,0,0,0.8);
border: 1px solid #111111;
margin: 5px;
}
```

7 En el html, código ya utilizando imágenes
```
<li class="splide__slide card"><img src="images/aquaman.png" alt=""></li> <li class="splide__slide card"><img src="images/batman.png" alt=""></li> <li class="splide__slide card"><img src="images/hulk.png" alt=""></li> <li class="splide__slide card"><img src="images/wolverine.png" alt=""></li> <li class="splide__slide card"><img src="images/linterna-verde.png" alt=""></li> <li class="splide__slide card"><img src="images/daredevil.png" alt=""></li>
```

8 Dentro del archivo de slider.css — animación en imágenes
```
img {
transition: transform 500ms ease-in-out;
width: 100%;
}

img:hover {
transform: scale(1.2);
}
```



