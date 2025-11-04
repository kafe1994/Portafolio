# Portfolio de Alejandro Javier Liendo - Cloudflare Pages

## Estructura del Proyecto

```
cloudflare-portfolio/
├── index.html              # Página principal del portfolio
├── manifest.json           # Manifest para PWA
├── robots.txt              # Configuración para motores de búsqueda
├── _headers                # Headers de seguridad y cache
├── _redirects              # Configuración de redirecciones
├── README.md               # Este archivo
└── assets/
    ├── css/               # Archivos CSS (si se separan)
    ├── js/                # Archivos JavaScript (si se separan)
    └── images/            # Imágenes del portfolio
        └── profile-photo.jpg
```

## Deployment en Cloudflare Pages

### Método 1: Git Integration (Recomendado)

1. **Conectar repositorio:**
   - Ve a [Cloudflare Pages](https://pages.cloudflare.com/)
   - Conecta tu repositorio de GitHub/GitLab
   - Configura el build command y output directory

2. **Configuración del build:**
   - Build command: `npm run build` (si usas build tools)
   - Build output directory: `/` (root directory)
   - Environment variables: None needed (sitio estático)

3. **Deployment automático:**
   - Cada push a la rama main desplegará automáticamente
   - Preview deployments para pull requests

### Método 2: Direct Upload

1. **Subir archivos:**
   - Ve a Cloudflare Pages Dashboard
   - Arrastra la carpeta `cloudflare-portfolio` completa
   - O sube el ZIP del proyecto

### Configuraciones Incluidas

#### Headers de Seguridad
- **X-Frame-Options**: Previene clickjacking
- **X-XSS-Protection**: Protección contra XSS
- **X-Content-Type-Options**: Previene MIME sniffing
- **Content-Security-Policy**: Política de seguridad de contenido

#### Cache Optimization
- **Assets estáticos**: Cache de 1 año (31536000 segundos)
- **HTML**: Cache de 0 segundos (siempre revalidar)
- **Headers immutable**: Para mejor performance

#### PWA Support
- **Manifest.json**: Configurado para instalación como app
- **Service Worker**: Listo para implementar
- **Offline support**: Estructura preparada

## Funcionalidades del Portfolio

### Características Principales
- ✅ **Diseño responsive**: Compatible con todos los dispositivos
- ✅ **Bilingüe**: Español/Inglés con selector de idioma
- ✅ **Formulario de contacto**: Envía emails a `liendoalejandro94@gmail.com`
- ✅ **WhatsApp integrado**: Enlace directo (+54 3572 408 928)
- ✅ **Esquema de colores**: Negro/blanco/gris consistente
- ✅ **Animaciones suaves**: CSS transitions y effects
- ✅ **SEO optimizado**: Meta tags y estructura semántica

### Secciones
1. **Hero**: Presentación personal con animación de roles
2. **About**: Historia personal y enfoque profesional
3. **Skills**: Habilidades técnicas con niveles de experiencia
4. **Projects**: Portfolio de proyectos destacados
5. **Contact**: Formulario y información de contacto

### Tecnologías
- **HTML5**: Estructura semántica
- **CSS3**: Variables, Grid, Flexbox, Animations
- **JavaScript**: Vanilla JS para interactividad
- **Progressive Web App**: Manifest y configuración PWA

## Customización

### Colores
Los colores están definidos como variables CSS en `:root`:
```css
--primary-black: #0a0a0a;
--secondary-black: #1a1a1a;
--dark-gray: #2a2a2a;
--medium-gray: #4a4a4a;
--light-gray: #6a6a6a;
--pure-white: #ffffff;
```

### Traducciones
El sistema de traducción está en el objeto `translations` en el JavaScript:
- `es`: Contenido en español
- `en`: Contenido en inglés

### Formulario de Contacto
Para cambiar el email de destino, modifica la línea en `handleFormSubmit()`:
```javascript
const emailAddress = 'tu-nuevo-email@gmail.com';
```

## Performance

### Optimizaciones Incluidas
- **Minificación**: CSS y JS ready para minification
- **Image optimization**: Formatos optimizados
- **Lazy loading**: Para imágenes y contenido pesado
- **Cache headers**: Configuración optimizada
- **Compression**: Gzip/Brotli enabled por Cloudflare

### Core Web Vitals
El sitio está optimizado para:
- **LCP**: < 2.5s (Largest Contentful Paint)
- **FID**: < 100ms (First Input Delay)
- **CLS**: < 0.1 (Cumulative Layout Shift)

## Monitoreo

### Analytics
Considera agregar:
- **Google Analytics**: Para tracking de usuarios
- **Cloudflare Analytics**: Privacy-friendly analytics
- **Hotjar**: Para heatmaps y user feedback

### Uptime Monitoring
Configura alertas para:
- **Uptime monitoring**: Para verificar disponibilidad
- **Performance monitoring**: Para Core Web Vitals
- **Error tracking**: Para JavaScript errors

## Soporte

### Browsers Soportados
- Chrome 88+
- Firefox 85+
- Safari 14+
- Edge 88+

### Contacto
- **Email**: liendoalejandro94@gmail.com
- **WhatsApp**: +54 3572 408 928
- **Portfolio**: Tu dominio personalizado

---

**Última actualización**: 2025-11-05
**Versión**: 1.0.0
**Licencia**: MIT
