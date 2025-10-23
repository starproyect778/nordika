# 📚 GUÍA DE ESTUDIO - PROYECTO NORDIKA

## 🎯 Introducción

Este documento te ayudará a entender la estructura y funcionamiento del sitio web de Nordika, una agencia de viajes nórdicos ficticia creada con fines educativos.

---

## 📁 Estructura del Proyecto

```
a_Proyecto Nordika_a/
│
├── CSS/
│   └── estilo.css          # Hoja de estilos principal (BIEN ORGANIZADA)
│
├── HTML/
│   ├── nordika.html        # Página principal
│   ├── suecia.html         # Página de Suecia
│   ├── dinamarca.html      # Página de Dinamarca
│   ├── noruega.html        # Página de Noruega
│   ├── finlandia.html      # Página de Finlandia
│   ├── islandia.html       # Página de Islandia
│   ├── tour-escandinavia.html  # Tours combinados
│   │
│   ├── Suecia/             # Ciudades de Suecia
│   │   ├── estocolmo.html
│   │   ├── gotemburgo.html
│   │   ├── malmo.html
│   │   ├── kiruna.html
│   │   └── visby.html
│   │
│   ├── Dinamarca/          # Ciudades de Dinamarca
│   ├── Noruega/            # Ciudades de Noruega
│   ├── Finlandia/          # Ciudades de Finlandia
│   └── Islandia/           # Destinos de Islandia
│
└── Imágenes/               # Todas las imágenes del sitio
```

---

## 🎨 ARCHIVO CSS - ESTRUCTURA DETALLADA

El archivo `CSS/estilo.css` está organizado en **15 secciones** numeradas y comentadas:

### 1. **Variables CSS** (Líneas 1-45)
```css
:root {
    --color-primary: #2c5f8d;
    --spacing-lg: 32px;
    --radius-sm: 8px;
}
```
**Qué son:** Variables reutilizables en todo el CSS
**Para qué sirven:** Mantener consistencia de colores, espacios y estilos
**Ventaja:** Cambiar un valor aquí actualiza TODO el sitio

### 2. **Reset y Base** (Líneas 47-65)
```css
* { margin: 0; padding: 0; box-sizing: border-box; }
body { font-family: 'Segoe UI'; }
```
**Qué son:** Reseteo de estilos del navegador
**Para qué sirven:** Eliminar inconsistencias entre navegadores
**Importante:** `box-sizing: border-box` hace que padding/border se incluyan en el tamaño

### 3. **Tipografía** (Líneas 67-95)
```css
h1 { font-size: clamp(2rem, 5vw, 3.5rem); }
```
**Qué es `clamp()`:** Define tamaño mínimo, preferido y máximo
**Ventaja:** Tipografía totalmente responsive sin media queries

### 4. **Navegación** (Líneas 97-199)
```css
.navbar { position: sticky; top: 0; }
.navbar-toggle { display: none; }  /* Visible solo en móviles */
```
**Conceptos clave:**
- `position: sticky` → Navbar fijo al hacer scroll
- `z-index: 1000` → Siempre visible sobre todo
- Menú hamburguesa para móviles

### 5. **Hero Sections** (Líneas 201-429)
```css
.hero-section { min-height: 85vh; }
.hero-content { display: grid; grid-template-columns: 1fr 1fr; }
```
**Conceptos clave:**
- `vh` = viewport height (85vh = 85% de la altura de pantalla)
- Grid de 2 columnas (texto e imagen)
- Botones con hover effects

### 6-7. **Contenido Principal y Tarjetas** (Líneas 431-557)
```css
.contenido-principal {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
}
```
**Conceptos clave:**
- `auto-fit` → Ajusta columnas automáticamente
- `minmax()` → Mínimo 350px, máximo 1fr (fracción)
- Tarjetas con efectos hover (elevación, zoom)

### 8. **Reseñas** (Líneas 559-685)
**Elementos decorativos:**
- Comillas grandes con `::before` y `::after`
- Línea decorativa bajo títulos
- Efecto glassmorphism en tarjetas

### 9. **Footer** (Líneas 687-750)
**Elementos:**
- Redes sociales con iconos
- `backdrop-filter: blur()` para efecto vidrio

### 10. **Reservas** (Líneas 752-850)
**Características:**
- Formulario centrado
- Lista de inclusiones
- Precio destacado

### 11. **Estadísticas** (Líneas 852-950)
```css
.stat-item {
    backdrop-filter: blur(10px);  /* Glassmorphism */
}
```
**Animación:** Contadores con JavaScript (ver HTML)

### 12. **Inspiración** (Líneas 952-1050)
```css
background-attachment: fixed;  /* Parallax */
```
**Elementos:**
- Copos de nieve animados
- Fondo parallax
- CTA (Call To Action) final

### 13. **Animaciones** (Líneas 1052-1150)
```css
@keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
}
```
**Tipos de animaciones:**
- Fade in/out
- Slide up/down
- Caída de copos de nieve
- Delays escalonados

### 14. **Botones y Utilidades** (Líneas 1152-1250)
**Clases de utilidad:**
```css
.text-center { text-align: center; }
.mt-3 { margin-top: 24px; }
```
**Botón flotante:** Volver arriba (aparece con scroll)

### 15. **Media Queries** (Líneas 1252-FIN)
**Breakpoints:**
- 1400px+ → Desktop grande
- 1200px → Laptop
- 1100px → Tablet horizontal
- 768px → Tablet vertical (menú hamburguesa)
- 640px → Móvil grande
- 480px → Móvil pequeño
- 360px → Móvil muy pequeño

---

## 🔑 CONCEPTOS CLAVE PARA ESTUDIAR

### 1. **CSS Grid**
```css
display: grid;
grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
gap: var(--spacing-xl);
```
**Aprende:** Cómo crear layouts responsivos con grid

### 2. **Flexbox**
```css
display: flex;
justify-content: space-between;
align-items: center;
gap: 24px;
```
**Aprende:** Alineación de elementos en fila/columna

### 3. **CSS Variables**
```css
:root { --color-primary: #2c5f8d; }
.elemento { background: var(--color-primary); }
```
**Aprende:** Reutilización de valores

### 4. **Pseudo-elementos**
```css
.elemento::before { content: ''; }
.elemento::after { content: '"'; }
```
**Aprende:** Agregar contenido decorativo sin HTML

### 5. **Transiciones y Transforms**
```css
transition: all 0.3s ease;
transform: translateY(-8px) scale(1.05);
```
**Aprende:** Animaciones suaves en hover

### 6. **Position**
```css
position: sticky;   /* Fijo al hacer scroll */
position: fixed;    /* Fijo en viewport */
position: absolute; /* Relativo al padre */
position: relative; /* Contexto para absolute */
```

### 7. **Z-Index**
```css
z-index: 1000;  /* Navbar (más alto) */
z-index: 2;     /* Contenido */
z-index: 1;     /* Fondo */
```
**Aprende:** Control de capas (quién está encima)

### 8. **Clamp para Responsive**
```css
font-size: clamp(1rem, 2vw, 1.5rem);
/* mínimo 1rem, preferido 2% del viewport, máximo 1.5rem */
```

### 9. **Media Queries**
```css
@media (max-width: 768px) {
    .elemento { /* estilos para tablet/móvil */ }
}
```
**Aprende:** Adaptar diseño a diferentes pantallas

### 10. **Animaciones con @keyframes**
```css
@keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
}
.elemento { animation: fadeInUp 1s ease-out; }
```

---

## 🎯 JAVASCRIPT - Funcionalidades Implementadas

### 1. **Menú Responsive**
```javascript
document.querySelector('.navbar-toggle').addEventListener('click', function() {
    document.querySelector('.navbar-menu').classList.toggle('active');
});
```
**Qué hace:** Abre/cierra el menú hamburguesa en móviles

### 2. **Animaciones al Scroll (Intersection Observer)**
```javascript
const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add('fade-in-visible');
        }
    });
});
```
**Qué hace:** Detecta cuando un elemento entra en pantalla y lo anima

### 3. **Contador Animado**
```javascript
const startCounting = () => {
    counters.forEach(counter => {
        const target = parseInt(counter.getAttribute('data-target'));
        // Anima de 0 hasta el número objetivo
    });
};
```
**Qué hace:** Números que cuentan de 0 a su valor final

### 4. **Botón Volver Arriba**
```javascript
if (window.pageYOffset > 300) {
    scrollToTopBtn.classList.add('visible');
}
```
**Qué hace:** Muestra botón después de hacer scroll

---

## 📋 CHECKLIST DE ESTUDIO

### Nivel Básico ✅
- [ ] Entiendo qué son las variables CSS
- [ ] Sé usar Flexbox básico
- [ ] Entiendo las unidades (px, rem, %, vh, vw)
- [ ] Puedo crear botones con hover
- [ ] Entiendo margin y padding

### Nivel Intermedio ✅
- [ ] Domino CSS Grid
- [ ] Sé usar pseudo-elementos (::before, ::after)
- [ ] Entiendo position (static, relative, absolute, fixed, sticky)
- [ ] Puedo hacer diseños responsive con media queries
- [ ] Entiendo z-index y contextos de apilamiento

### Nivel Avanzado ✅
- [ ] Domino animaciones con @keyframes
- [ ] Sé usar Intersection Observer API
- [ ] Entiendo requestAnimationFrame
- [ ] Puedo optimizar performance con will-change
- [ ] Domino efectos avanzados (backdrop-filter, glassmorphism)

---

## 🔍 DONDE BUSCAR CADA COSA

| Necesito... | Buscar en línea(s) |
|-------------|-------------------|
| Variables de colores | 1-13 |
| Espaciados del sitio | 26-31 |
| Estilos del navbar | 97-199 |
| Hero section | 201-311 |
| Tarjetas de viajes | 451-557 |
| Reseñas de clientes | 559-685 |
| Footer | 687-750 |
| Estadísticas | 852-950 |
| Animaciones | 1052-1150 |
| Responsive móvil | 1400+ |

---

## 💡 TIPS PARA ESTUDIAR

1. **Empieza por las variables** (sección 1)
   - Entiende la paleta de colores
   - Nota el sistema de espaciado de 8px

2. **Estudia el Hero Section** (sección 5)
   - Es un buen ejemplo de Grid + Flexbox
   - Aprende los efectos hover de botones

3. **Analiza las tarjetas** (sección 7)
   - Efecto de elevación al hover
   - Transiciones suaves

4. **Revisa las animaciones** (sección 13)
   - Cómo funcionan @keyframes
   - Delays escalonados

5. **Estudia el responsive** (sección 15)
   - Cómo se adapta a móviles
   - Menú hamburguesa

---

## 🚀 EJERCICIOS PROPUESTOS

1. **Cambiar colores:** Modifica las variables CSS y observa los cambios
2. **Agregar una tarjeta:** Crea un nuevo destino copiando el HTML
3. **Modificar animaciones:** Cambia la velocidad de los copos de nieve
4. **Crear nueva sección:** Agrega una sección "Ofertas Especiales"
5. **Mejorar responsive:** Ajusta el diseño para tablets específicamente

---

## 📚 RECURSOS PARA APRENDER MÁS

- **CSS Grid:** css-tricks.com/snippets/css/complete-guide-grid/
- **Flexbox:** css-tricks.com/snippets/css/a-guide-to-flexbox/
- **Variables CSS:** developer.mozilla.org/es/docs/Web/CSS/Using_CSS_custom_properties
- **Animaciones:** developer.mozilla.org/es/docs/Web/CSS/CSS_Animations
- **Intersection Observer:** developer.mozilla.org/es/docs/Web/API/Intersection_Observer_API

---

## ✅ CÓDIGO COMPLETAMENTE REVISADO

El archivo CSS ha sido:
- ✅ **Organizado** en 15 secciones claramente delimitadas
- ✅ **Comentado** cada concepto y propiedad importante
- ✅ **Optimizado** sin código duplicado
- ✅ **Sin errores** de sintaxis
- ✅ **Responsive** para todos los dispositivos
- ✅ **Profesional** con mejores prácticas actuales

---

**¡Ahora el código es perfecto para estudiar! 🎉**

