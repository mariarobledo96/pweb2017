% Diseño adaptable (_responsive_)

>The **control** which designers know in the print medium, and often desire in the web medium, is simply a function of the **limitation of the printed page**. We should embrace the fact that the web doesn’t have the same constraints, and **design for this flexibility**. But first, we must 'accept the ebb and flow of things.'

&mdash; John Allsopp, “A Dao of Web Design”

## Paso 0

Punto de partida:

[Rejillas rígidas](https://codepen.io/justincavery/full/rzfbg)


## Paso 1

[Rejillas flexibles](https://alistapart.com/d/responsive-web-design/ex/ex-site-flexible.html)

---

- con imágenes flexibles
- se adapta a visores con formatos horizontales o verticales

---

Problemas:

- en visores pequeños, los elementos se empiezan a _pisar_ unos a otros
- en visores muy grandes, las imágenes adoptan tamaños descomunales

---

Conclusión:

El diseño flexible funciona bien en contextos de escritorio para los que fue diseñado, pero no está optimizado para extenderse mucho más allá.

## Siguiente paso: convertirse en adaptable

En lugar de hacer diseños desconectados "a medida" para un número siempre creciente de dispositivos muy diversos, deberían tratarse como **facetas de la misma experiencia**. 

¿Cómo? Mediante el diseño web adaptable (_responsive web design_) 

---

CSS3 permite recopilar información no solamente sobre el tipo de medio (pantalla, impresión...), sino sobre características concretas del medio (como su tamaño o resolución, por ejemplo) a través de los `media queries`.

---

Convertir el diseño en una única columna:

```
@media screen and (max-width: 600px) {
  .mast,
  .intro,
  .main,
  .footer {
    float: none;
    width: auto;
  }
}
```

[Ejemplo mejorado](https://alistapart.com/d/responsive-web-design/ex/ex-site-linearize.html)

---

El uso de los `media queries` permite cambios más allá de la simple ubicación de las imágenes: es posible introducir _layouts_ alternativos adaptados realmente a las necesidades de cada rango de resoluciones.

[Ejemplo final](https://alistapart.com/d/responsive-web-design/ex/ex-site-FINAL.html)

---

El diseño adaptable tampoco se limita a las modificaciones de disposición. Permite resaltar los elementos más importantes para visores pequeños; mostrar u ocultar elementos selectivamete para mejorar la navegación; o adaptar los tamaños de letra de titulares y demás textos para optimizar la lectura.

---

## Resumen

El diseño adaptable (_responsive web design_) se compone de tres ingredientes técnicos:

1. Rejillas fluidas
2. Imágenes flexibles
3. `Media queries`

---

En lugar de destinar nuestro contenido a compartimentos estancos sobre-adaptados a dispositivos con fecha de caducidad, podemos plantear diseños que muestren lo más destacable de la experiencia en cada contexto.