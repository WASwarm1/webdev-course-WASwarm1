# 🎨 Guía Rápida de CSS

## ¿Cómo agregar CSS?

### 1. CSS Interno (en el mismo archivo HTML)
```html
<head>
    <style>
        h1 {
            color: blue;
        }
    </style>
</head>
```

### 2. CSS Externo (archivo separado)
```html
<head>
    <link rel="stylesheet" href="estilos.css">
</head>
```

### 3. CSS en Línea (directamente en el elemento)
```html
<h1 style="color: blue;">Título</h1>
```

---

## Selectores Básicos

```css
/* Selector de elemento */
p {
    color: blue;
}

/* Selector de clase */
.mi-clase {
    color: red;
}

/* Selector de ID */
#mi-id {
    color: green;
}

/* Selector universal (todos los elementos) */
* {
    margin: 0;
}
```

**Uso en HTML:**
```html
<p>Párrafo azul</p>
<p class="mi-clase">Párrafo rojo</p>
<p id="mi-id">Párrafo verde</p>
```

---

## Colores

```css
/* Nombres de colores */
color: red;
color: blue;
color: green;

/* Códigos hexadecimales */
color: #FF0000; /* rojo */
color: #00FF00; /* verde */
color: #0000FF; /* azul */

/* RGB */
color: rgb(255, 0, 0); /* rojo */

/* RGBA (con transparencia) */
color: rgba(255, 0, 0, 0.5); /* rojo semi-transparente */
```

---

## Propiedades de Texto

```css
/* Color del texto */
color: blue;

/* Tamaño de fuente */
font-size: 16px;
font-size: 2em;

/* Familia de fuente */
font-family: Arial, sans-serif;

/* Peso de fuente (grosor) */
font-weight: bold;
font-weight: normal;

/* Estilo de fuente */
font-style: italic;
font-style: normal;

/* Alineación del texto */
text-align: left;
text-align: center;
text-align: right;

/* Decoración del texto */
text-decoration: underline;
text-decoration: none;

/* Altura de línea */
line-height: 1.5;
```

---

## Colores de Fondo

```css
/* Color de fondo sólido */
background-color: yellow;
background-color: #FFD700;

/* Imagen de fondo */
background-image: url('imagen.jpg');

/* Gradiente */
background: linear-gradient(to right, blue, purple);
```

---

## Modelo de Caja (Box Model)

```css
/* Ancho y alto */
width: 300px;
height: 200px;

/* Padding (espacio interior) */
padding: 20px; /* todos los lados */
padding-top: 10px;
padding-right: 15px;
padding-bottom: 10px;
padding-left: 15px;

/* Margin (espacio exterior) */
margin: 20px; /* todos los lados */
margin-top: 10px;
margin-right: 15px;
margin-bottom: 10px;
margin-left: 15px;

/* Centrar elemento */
margin: 0 auto;

/* Border (borde) */
border: 2px solid black;
border-width: 2px;
border-style: solid;
border-color: black;
border-radius: 10px; /* bordes redondeados */
```

---

## Visualización del Modelo de Caja

```
┌─────────────────────────────────────┐
│          MARGIN (exterior)          │
│  ┌───────────────────────────────┐  │
│  │     BORDER (borde)            │  │
│  │  ┌─────────────────────────┐  │  │
│  │  │  PADDING (interior)     │  │  │
│  │  │  ┌───────────────────┐  │  │  │
│  │  │  │    CONTENT        │  │  │  │
│  │  │  │   (contenido)     │  │  │  │
│  │  │  └───────────────────┘  │  │  │
│  │  └─────────────────────────┘  │  │
│  └───────────────────────────────┘  │
└─────────────────────────────────────┘
```

---

## Propiedades de Display

```css
/* Tipos de display */
display: block;    /* elemento en bloque (nueva línea) */
display: inline;   /* elemento en línea */
display: none;     /* ocultar elemento */
```

---

## Ejemplo Completo: Tarjeta de Perfil

```css
/* Estilo del body */
body {
    background-color: #f0f0f0;
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 20px;
}

/* Contenedor principal */
.tarjeta {
    background-color: white;
    width: 400px;
    margin: 0 auto;
    padding: 30px;
    border: 2px solid #ddd;
    border-radius: 15px;
}

/* Título */
h1 {
    color: #2C3E50;
    font-size: 32px;
    margin-bottom: 10px;
}

/* Imagen */
.foto {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    border: 4px solid #3498DB;
}

/* Párrafos */
p {
    color: #555;
    font-size: 16px;
    line-height: 1.6;
}

/* Enlaces */
a {
    color: #3498DB;
    text-decoration: none;
    font-weight: bold;
}

a:hover {
    text-decoration: underline;
}
```

---

## Colores Populares

```css
/* Azules */
#3498DB  /* Azul claro */
#2C3E50  /* Azul oscuro */
#5DADE2  /* Azul cielo */

/* Verdes */
#2ECC71  /* Verde esmeralda */
#27AE60  /* Verde oscuro */

/* Rojos */
#E74C3C  /* Rojo */
#C0392B  /* Rojo oscuro */

/* Amarillos */
#F39C12  /* Naranja */
#FFD700  /* Dorado */

/* Púrpuras */
#9B59B6  /* Púrpura */
#8E44AD  /* Púrpura oscuro */

/* Grises */
#ECF0F1  /* Gris claro */
#95A5A6  /* Gris medio */
#7F8C8D  /* Gris oscuro */
```

---

## Trucos Útiles

### Centrar un elemento
```css
.elemento {
    width: 500px;
    margin: 0 auto;
}
```

### Sombra de caja
```css
box-shadow: 0 2px 5px rgba(0,0,0,0.2);
```

### Transiciones suaves
```css
transition: all 0.3s ease;
```

### Efecto hover (al pasar el mouse)
```css
.boton:hover {
    background-color: blue;
    transform: scale(1.1);
}
```

---

## Errores Comunes

❌ **Olvidar el punto y coma**
```css
/* Incorrecto */
color: blue
font-size: 16px

/* Correcto */
color: blue;
font-size: 16px;
```

❌ **Olvidar las llaves**
```css
/* Incorrecto */
p
    color: blue;

/* Correcto */
p {
    color: blue;
}
```

❌ **Espacios en nombres de clases**
```css
/* Incorrecto */
.mi clase {
    color: blue;
}

/* Correcto */
.mi-clase {
    color: blue;
}
```

---

## Consejos

✅ **Usa nombres descriptivos** para tus clases: `.boton-principal` en vez de `.btn1`  
✅ **Organiza tu CSS** agrupando estilos relacionados  
✅ **Comenta tu código** para recordar qué hace cada sección  
✅ **Prueba diferentes valores** para ver qué funciona mejor  
✅ **Usa herramientas online** como [ColorPicker](https://www.google.com/search?q=color+picker) para elegir colores

---

## Recursos Adicionales

📚 **MDN Web Docs**: https://developer.mozilla.org/es/docs/Web/CSS  
📚 **W3Schools**: https://www.w3schools.com/css/  
🎨 **Paletas de colores**: https://coolors.co/

---

**¡Practica y experimenta con diferentes estilos!** 🎨✨