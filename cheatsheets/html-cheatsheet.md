# 📄 Guía Rápida de HTML

## Estructura Básica

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Título de la Página</title>
</head>
<body>
    <!-- Tu contenido aquí -->
</body>
</html>
```

---

## Etiquetas de Texto

### Títulos
```html
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
<h3>Título de Nivel 3</h3>
<h4>Título de Nivel 4</h4>
<h5>Título de Nivel 5</h5>
<h6>Título de Nivel 6</h6>
```

### Párrafos y Texto
```html
<p>Este es un párrafo de texto.</p>
<strong>Texto en negrita</strong>
<em>Texto en cursiva</em>
<br> <!-- Salto de línea -->
```

---

## Listas

### Lista sin orden (viñetas)
```html
<ul>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
    <li>Elemento 3</li>
</ul>
```

### Lista numerada
```html
<ol>
    <li>Primer elemento</li>
    <li>Segundo elemento</li>
    <li>Tercer elemento</li>
</ol>
```

---

## Imágenes

```html
<img src="ruta/imagen.jpg" alt="Descripción de la imagen">
```

**Atributos importantes:**
- `src`: Ruta de la imagen
- `alt`: Texto alternativo (descripción)
- `width`: Ancho en píxeles
- `height`: Alto en píxeles

**Ejemplo completo:**
```html
<img src="https://ejemplo.com/foto.jpg" alt="Mi foto" width="300">
```

---

## Enlaces

```html
<a href="https://www.ejemplo.com">Texto del enlace</a>
```

**Tipos de enlaces:**
```html
<!-- Enlace a otra página web -->
<a href="https://www.google.com">Ir a Google</a>

<!-- Enlace a otra página del mismo sitio -->
<a href="contacto.html">Contáctanos</a>

<!-- Enlace que abre en nueva pestaña -->
<a href="https://www.ejemplo.com" target="_blank">Abrir en nueva pestaña</a>

<!-- Enlace de correo electrónico -->
<a href="mailto:correo@ejemplo.com">Enviar email</a>
```

---

## Contenedores

### Div (división)
```html
<div>
    <h2>Título de la sección</h2>
    <p>Contenido de la sección.</p>
</div>
```

### Span (texto en línea)
```html
<p>Este es un <span>texto especial</span> dentro del párrafo.</p>
```

---

## Comentarios

```html
<!-- Este es un comentario y no se mostrará en la página -->
```

---

## Etiquetas Semánticas Útiles

```html
<header>Encabezado de la página</header>
<nav>Menú de navegación</nav>
<main>Contenido principal</main>
<section>Sección de contenido</section>
<article>Artículo independiente</article>
<aside>Contenido relacionado (barra lateral)</aside>
<footer>Pie de página</footer>
```

---

## Ejemplos Prácticos

### Página Simple
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Mi Primera Página</title>
</head>
<body>
    <h1>Bienvenido a mi página</h1>
    <p>Esta es mi primera página web.</p>
    
    <h2>Mis intereses</h2>
    <ul>
        <li>Programación</li>
        <li>Diseño</li>
        <li>Música</li>
    </ul>
    
    <img src="foto.jpg" alt="Mi foto">
    
    <a href="contacto.html">Contáctame</a>
</body>
</html>
```

---

## Consejos Importantes

✅ **Siempre cierra las etiquetas**: `<p>texto</p>`  
✅ **Usa comillas en los atributos**: `<img src="foto.jpg">`  
✅ **Indenta tu código** para que sea más fácil de leer  
✅ **Usa nombres descriptivos** en tus archivos: `mi-pagina.html`  
✅ **Agrega texto alt a las imágenes** para accesibilidad

❌ **No olvides** cerrar las etiquetas  
❌ **No uses** espacios en nombres de archivos  
❌ **No mezcles** mayúsculas y minúsculas sin razón

---

## Recursos Adicionales

📚 **MDN Web Docs**: https://developer.mozilla.org/es/docs/Web/HTML  
📚 **W3Schools**: https://www.w3schools.com/html/

---

**¡Sigue practicando y experimentando con HTML!** 