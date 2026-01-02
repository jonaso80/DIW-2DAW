# Explicación proyecto

**Asignatura:** Diseño de Interfaces Web (DIW)    
**Curso:** 2º Desarrollo de Aplicaciones Web (DAW)  
**Autor:** Jonás Pérez Cuenca

---

## 1. Concepto y Diseño
La web ha sido diseñada como una *landing page* de producto premium para la raqueta **Babolat Pure Aero Rafa Origin**. El objetivo visual es transmitir la energía de Rafael Nadal mediante el uso de su paleta de colores oficial: **Amarillo neón, Rosa intenso y Azul**. 

He optado por un estilo **"Dark Mode"** para resaltar los componentes neón y las imágenes.

---

## 2. Uso del Grid System y Bootstrap
* **Contenedores:** Se utiliza `.container` para centrar el contenido y mantener márgenes en todas las pantallas.
* **Estructura de Columnas:**
    * `col-sm-6`: En tablets (dispositivos medianos) se muestran 2 tarjetas por fila.
    * `col-md-4`: En escritorio se muestran las 3 en una sola fila.
    * `col-12`: En móvil se apilan verticalmente para facilitar la lectura.
* **Utilidades de Flexbox:** Se han usado clases como `d-flex`, `align-items-center` y `gap-3` para los espaciados y alineación vertical de textos e imágenes.



---

## 3. Componentes y Personalización
1.  **Animaciones CSS:** Se ha creado un *keyframe* personalizado (`float`) para dotar a la raqueta de un movimiento de levitación orgánico.

---

## 4. Tema Personalizado y Variables
En lugar de depender de los colores estándar de Bootstrap, se ha creado un tema propio utilizando **Variables CSS (`:root`)**:

* **Variables principales:** `--rafa-yellow`, `--rafa-pink` y `--rafa-blue`.
* **Botones Custom:** La clase `.btn-action` sustituye a los botones nativos, incorporando degradados lineales y efectos de sombra (`box-shadow`) que reaccionan al *hover*.

---

## 5. Responsividad y Mobile First
* **Hero Section:** En dispositivos móviles, se ajusta el `height` a `75vh` y se desactiva el `clip-path` para evitar cortes en el texto.
* **Tipografía Adaptativa:** Uso de la función `clamp()` en los títulos (`main-title`), permitiendo que el tamaño de la fuente se ajuste entre un mínimo y un máximo según el ancho de la ventana (`vw`).
* **Imágenes Fluidas:** La imagen de la raqueta utiliza `max-width: 100%` para escalar correctamente en pantallas pequeñas.

---

## 6. Accesibilidad - Nivel AA
* **Contraste:** El color `--text-muted` (#b0b0b0) ha sido seleccionado para cumplir con los ratios de contraste WCAG sobre fondos negros.
* **Atributos ARIA:** Se ha añadido `aria-hidden="true"` a elementos decorativos (como el cursor luminoso) para no confundir a los lectores de pantalla.
* **Semántica HTML5:** Uso de etiquetas estructurales como `<header>`, `<main>`, `<section>` y `<footer>`.
* **Skip Links:** Se ha incluido un enlace de "Saltar al contenido" para navegación por teclado.

---

* **Repositorio:** https://github.com/jonaso80/DIW-2DAW.git
