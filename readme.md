# ESCOTEL - Sitio Web Corporativo

## Tecnologías Utilizadas

### Frontend
- **HTML5** - Estructura del sitio
- **CSS3** - Estilos avanzados con efectos
- **JavaScript (Vanilla)** - Funcionalidades sin frameworks

### Librerías y Recursos Externos
- **Google Fonts (Inter)** - Tipografía moderna
- **Font Awesome** - Iconografía
- **Google Maps** - Integración de mapas

### Características Técnicas
- **Smooth Scrolling** - Navegación fluida entre secciones
- **Backdrop Filter** - Efectos de desenfoque glassmorphism

## Estructura del Sitio

### Secciones Principales

1. **Header Navigation**
   - Barra superior con información de contacto
   - Navbar con logo y menú principal
   - Menús desplegables organizados por categorías

2. **Hero Section**
   - Banner principal con imagen de fondo
   - Efecto glassmorphism overlay

3. **Soluciones** (`#soluciones`)
   - Conectividad empresarial
   - Seguridad de redes
   - Comunicación unificada

4. **Servicios** (`#servicios`)
   - Redes inalámbricas
   - Centros de datos
   - Soporte técnico 24/7
   - Mapa de ubicación

5. **Footer**
   - Información corporativa
   - Enlaces organizados por categorías
   - Datos de contacto completos

## Funciones JavaScript Importantes

### 1. Toggle Menú Mobile
```javascript
// Manejo del menú hamburguesa en dispositivos móviles
mobileMenuBtn.addEventListener('click', function() {
    navLinks.classList.toggle('active');
});
```

### 2. Smooth Scrolling
```javascript
// Navegación suave entre secciones ancla
links.forEach(link => {
    link.addEventListener('click', function(e) {
        targetElement.scrollIntoView({
            behavior: 'smooth',
            block: 'start'
        });
    });
});
```

### 3. Navbar Scroll Effect
```javascript
// Efecto de transparencia en navbar al hacer scroll
window.addEventListener('scroll', function() {
    if (window.scrollY > 50) {
        navbar.style.background = 'rgba(255, 255, 255, 0.95)';
        navbar.style.backdropFilter = 'blur(10px)';
    }
});
```

### 4. Click Outside Handler
```javascript
// Cierra el menú mobile al hacer click fuera
document.addEventListener('click', function(e) {
    if (!mobileMenuBtn.contains(e.target) && !navLinks.contains(e.target)) {
        navLinks.classList.remove('active');
    }
});
```

### Paleta de Colores
- **Principal**: #b30000 (Rojo corporativo)
- **Hover**: #e60000 / #cc0000
- **Texto**: #1a1a1a (Negro suave)
- **Fondo**: #f4f4f4 (Gris claro)

### Efectos Visuales
- **Glassmorphism**: Overlays con `backdrop-filter: blur()`

### Responsividad
- **Mobile Menu**: Menú de hamburguesa para navegación
- **Grid Layout**: Con `auto-fit` y `minmax()`

### Google Maps
- Iframe embebido con ubicación específica

### Redes Sociales
- Iconos de Font Awesome con efectos hover

### Archivos Principales
- `index.html`
- `styles.css`
- `script.js`

### Assets Externos
- Logo alojado en dominio de ESCOTEL
- Fonts de Google Fonts CDN
- Font Awesome CDN
- Imagen hero desde Storyblok