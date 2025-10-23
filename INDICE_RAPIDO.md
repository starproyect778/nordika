# 🗺️ ÍNDICE RÁPIDO - NORDIKA CSS

## 📍 Búsqueda Rápida por Líneas

### 🎨 DISEÑO Y VARIABLES
```
Líneas    | Qué contiene
----------|----------------------------------
1-45      | Variables CSS (colores, espacios, sombras)
47-65     | Reset de navegador
67-95     | Tipografía base (h1-h6, p, a, img)
```

### 🧭 NAVEGACIÓN
```
Líneas    | Qué contiene
----------|----------------------------------
97-106    | Navbar sticky
108-117   | Contenedor del navbar
119-133   | Logo
135-141   | Menú de navegación
143-179   | Enlaces y botón de contacto
181-199   | Menú hamburguesa (móvil)
```

### 🎯 SECCIONES HERO
```
Líneas    | Qué contiene
----------|----------------------------------
201-211   | Hero principal (estructura)
213-223   | Hero content (grid 2 columnas)
225-247   | Texto del hero (h1, h2, p)
249-253   | Botones del hero
255-293   | Estilos de botones
295-318   | Imagen del hero
320-429   | Hero de destinos (similar)
```

### 🃏 TARJETAS Y CONTENIDO
```
Líneas    | Qué contiene
----------|----------------------------------
431-448   | Contenedor principal (grid)
451-557   | Tarjetas de viajes completas
459-495   | Estructura de tarjeta
497-516   | Imagen de tarjeta
518-557   | Info y precio
```

### ⭐ RESEÑAS
```
Líneas    | Qué contiene
----------|----------------------------------
559-576   | Sección de reseñas
578-600   | Título y decoración
602-685   | Grid y tarjetas de reseñas
625-675   | Comillas decorativas
677-685   | Autor de reseña
```

### 👣 FOOTER
```
Líneas    | Qué contiene
----------|----------------------------------
687-700   | Footer principal
702-750   | Redes sociales
```

### 🎫 RESERVAS
```
Líneas    | Qué contiene
----------|----------------------------------
752-850   | Sección completa de reservas
785-820   | Información del paquete
822-840   | Caja de precio
842-850   | Botón finalizar
```

### 📊 ESTADÍSTICAS
```
Líneas    | Qué contiene
----------|----------------------------------
852-885   | Sección de estadísticas
887-950   | Tarjetas de stats (glassmorphism)
```

### 🌟 INSPIRACIÓN
```
Líneas    | Qué contiene
----------|----------------------------------
952-1000  | Sección de inspiración final
1002-1018 | Contenido central
1020-1050 | Copos de nieve animados
```

### 🎬 ANIMACIONES
```
Líneas    | Qué contiene
----------|----------------------------------
1052-1075 | @keyframes fall (copos)
1077-1095 | @keyframes fadeInUp/Down
1097-1150 | Fade-in al scroll + delays
```

### 🔘 BOTONES Y UTILIDADES
```
Líneas    | Qué contiene
----------|----------------------------------
1152-1195 | Botón volver arriba
1197-1205 | Clases de alineación
1207-1225 | Clases de márgenes
1227-1232 | Contenedor genérico
```

### 📱 RESPONSIVE (MEDIA QUERIES)
```
Líneas    | Breakpoint        | Dispositivo
----------|-------------------|------------------
1240-1250 | 1400px+          | Desktop XL
1252-1260 | 1200px           | Laptop grande
1262-1280 | 1100px           | Tablets horizontal
1282-1320 | 1024px           | Tablets
1322-1480 | 768px            | Móviles/Tablet V
1482-1540 | 640px            | Móviles grandes
1542-1620 | 480px            | Móviles
1622-1640 | 360px            | Móviles pequeños
```

---

## 🔍 BUSCAR POR CONCEPTO

### Grid CSS
- Línea 440: Grid principal de destinos
- Línea 215: Grid del hero (2 columnas)
- Línea 602: Grid de reseñas
- Línea 889: Grid de estadísticas

### Flexbox
- Línea 112: Navbar container
- Línea 136: Menú de navegación
- Línea 250: Botones del hero
- Línea 703: Redes sociales

### Animaciones
- Línea 1052: @keyframes fall
- Línea 1077: @keyframes fadeInUp
- Línea 1097: Fade-in al scroll
- Línea 1118: Delays escalonados

### Efectos Hover
- Línea 131: Logo hover
- Línea 158: Link hover
- Línea 277: Botón primario hover
- Línea 486: Tarjeta hover
- Línea 623: Reseña hover

### Position
- Línea 98: sticky (navbar)
- Línea 1154: fixed (botón scroll)
- Línea 220: relative (hero content)
- Línea 314: absolute (overlay)

### Pseudo-elementos
- Línea 474: ::before (línea decorativa tarjeta)
- Línea 591: ::after (línea bajo título)
- Línea 635: ::before (comilla izquierda)
- Línea 644: ::after (comilla derecha)

### Variables CSS
- Línea 4: Colores
- Línea 15: Gradientes
- Línea 20: Sombras
- Línea 26: Espaciado
- Línea 34: Bordes
- Línea 41: Transiciones

### Responsive
- Línea 1262: Tablet H ajustes
- Línea 1322: Menú hamburguesa
- Línea 1542: Móviles (botones full-width)

---

## 🎨 PALETA DE COLORES

```css
Principal:    #2c5f8d  ████ Azul océano
Secundario:   #1a4d75  ████ Azul oscuro
Acento:       #ffc107  ████ Dorado
Oscuro:       #1a3a52  ████ Azul muy oscuro
Claro:        #f8f9fa  ████ Gris claro
Blanco:       #ffffff  ████ Blanco
Texto:        #333333  ████ Gris oscuro
Texto claro:  #666666  ████ Gris medio
```

---

## 📏 SISTEMA DE ESPACIADO

```css
--spacing-xs:   8px   ▯
--spacing-sm:   16px  ▯▯
--spacing-md:   24px  ▯▯▯
--spacing-lg:   32px  ▯▯▯▯
--spacing-xl:   48px  ▯▯▯▯▯▯
--spacing-xxl:  64px  ▯▯▯▯▯▯▯▯
```

---

## 🎯 BREAKPOINTS

```
360px  |─────| Móvil muy pequeño
480px  |──────────| Móvil pequeño
640px  |────────────────| Móvil grande
768px  |──────────────────────| Tablet vertical
1024px |───────────────────────────────| Tablet horizontal
1100px |────────────────────────────────────| Laptop
1200px |──────────────────────────────────────────| Laptop grande
1400px |────────────────────────────────────────────────| Desktop XL
```

---

## 🚀 COMANDOS DE BÚSQUEDA (Ctrl+F)

### Buscar por componente:
```
.navbar
.hero-section
.contenido-principal
.viaje-item
.reseña-card
.footer
.stats-section
```

### Buscar por efecto:
```
hover
transition
transform
animation
@keyframes
```

### Buscar por responsive:
```
@media
max-width
min-width
```

---

## ✅ CHECKLIST DE REVISIÓN

- [x] Todas las secciones comentadas
- [x] Código sin duplicados
- [x] Variables CSS utilizadas correctamente
- [x] Sin errores de sintaxis
- [x] Responsive para todos los dispositivos
- [x] Animaciones optimizadas
- [x] Comentarios explicativos
- [x] Estructura lógica y ordenada

---

## 📝 NOTAS IMPORTANTES

1. **Variables primero:** Siempre revisar las variables antes de cambiar estilos
2. **Mobile first:** Los media queries van de menor a mayor
3. **Comentarios:** Cada sección tiene título y explicación
4. **Performance:** Se usa `will-change` en animaciones
5. **Accesibilidad:** Todos los botones tienen cursor: pointer

---

**Última actualización:** Octubre 2025
**Versión:** 2.0 - Reorganizada y documentada

