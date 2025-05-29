# ESCOTEL - Sitio Web

## Tecnologías Utilizadas

### Frontend
- **HTML5** - Estructura del sitio
- **CSS3** - Estilos avanzados con efectos
- **JavaScript (Vanilla)** - Funcionalidades sin frameworks

### Librerías y Recursos Externos
- **Google Fonts (Inter)** - Tipografía
- **Font Awesome** - Iconografía
- **Google Maps** - Integración de mapas

## Estructura del Sitio

### Secciones Principales

1. **Header Navigation**

2. **Hero Section**

3. **Soluciones**

4. **Servicios**

5. **Footer**


## Funciones JavaScript

### 1. Smooth Scrolling
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

### 2. Navbar Scroll Effect
```javascript
// Efecto de transparencia en navbar al hacer scroll
window.addEventListener('scroll', function() {
    if (window.scrollY > 50) {
        navbar.style.background = 'rgba(255, 255, 255, 0.95)';
        navbar.style.backdropFilter = 'blur(10px)';
    }
});
```

### 3. Click Outside Handler
```javascript
// Cierra el menú mobile al hacer click fuera
document.addEventListener('click', function(e) {
    if (!mobileMenuBtn.contains(e.target) && !navLinks.contains(e.target)) {
        navLinks.classList.remove('active');
    }
});
```

### Google Maps
- Iframe con ubicación

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
