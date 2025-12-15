# 📚 Biblioteca de Cómics y Mangas - Versión Estática

Una aplicación web completa y autocontenida para gestionar y visualizar colecciones de cómics y mangas. 100% estática, sin necesidad de servidor.

![Preview](https://i.imgur.com/uR1l3gL.jpg)

## ✨ Características Principales

- 📚 **Gestión de Series**: Crear, editar y eliminar series de manga
- 📖 **Visualizador de Capítulos**: Lectura fluida con auto-scroll ajustable
- ⚙️ **Panel de Administración**: Interfaz completa para gestionar contenido
- 🔄 **Navegación Inteligente**: Botones anterior/siguiente automáticos entre capítulos
- ⚡ **Auto-Scroll Control**: Velocidad ajustable (1-10 niveles)
- ⌨️ **Atajos de Teclado**: Navegación rápida con flechas y espacio
- 📱 **Diseño Responsivo**: Funciona perfectamente en móviles y desktop
- 💾 **Almacenamiento Local**: Datos guardados automáticamente en el navegador
- 🌙 **Modo Oscuro**: Interfaz elegante para lectura prolongada
- 🎨 **Animaciones Suaves**: Transiciones fluidas y experiencia moderna

## 🚀 Demostración

Puedes ver una demostración en vivo aquí:
- **Aplicación Principal**: [Ver Demo](https://tu-sitio-demo.com)
- **Panel de Administración**: [Admin Demo](https://tu-sitio-demo.com)

## 📁 Estructura del Proyecto

```
manga-library-static/
├── index.html              # Aplicación completa (32KB)
├── README.md               # Documentación en inglés
├── README-ES.md           # Documentación en español
└── assets/                # Imágenes y recursos (opcional)
```

## 🎯 Cómo Usar

### Método 1: Descarga Directa
1. Descarga el archivo `index.html`
2. Ábrelo en tu navegador web
3. ¡Listo! La aplicación está funcionando

### Método 2: GitHub Pages (Recomendado)
1. Haz **Fork** de este repositorio
2. Ve a **Settings → Pages**
3. Activa **GitHub Pages** con la rama `main`
4. Tu sitio estará disponible en: `https://tu-usuario.github.io/manga-library-static`

### Método 3: Otros Hosting
- **Netlify**: Arrastra y suelta el archivo `index.html`
- **Vercel**: Importa este repositorio
- **Firebase Hosting**: Sube el archivo a Firebase Hosting

## 🎮 Uso de la Aplicación

### Para Usuarios Finales
1. **Explorar Series**: Navega por las diferentes series disponibles
2. **Leer Capítulos**: Haz clic en cualquier capítulo para comenzar a leer
3. **Auto-Scroll**: Usa el botón ▶️ para activar el scroll automático
4. **Control de Velocidad**: Ajusta la velocidad de lectura con el control deslizante
5. **Navegación**: Usa los botones ⬅️ Siguiente ➡️ para moverte entre capítulos

### Para Administradores
1. **Acceder al Panel**: Haz clic en "⚙️ Panel de Administración"
2. **Crear Series**: Usa el formulario para agregar nuevas series
3. **Gestionar Contenido**: Edita o elimina series existentes
4. **Los datos se guardan automáticamente** en el navegador

## ⌨️ Atajos de Teclado

| Tecla | Función |
|-------|----------|
| ← | Capítulo anterior |
| → | Capítulo siguiente |
| Espacio | Iniciar/Detener auto-scroll |
| Escape | Volver al inicio |

## 🎨 Personalización

### Cambiar Imágenes
Edita la sección `initializeApp()` en el archivo `index.html`:

```javascript
images: [
    "https://i.imgur.com/tu-imagen-1.jpg",  // Reemplaza con tus imágenes
    "https://i.imgur.com/tu-imagen-2.jpg",
    // ... más imágenes
]
```

### Modificar Colores
Edita las variables CSS al inicio del archivo:

```css
:root {
    --primary-color: #4CAF50;      /* Color primario */
    --secondary-color: #2196F3;    /* Color secundario */
    --background-color: #212121;    /* Color de fondo */
    --text-color: #EAEAEA;         /* Color del texto */
}
```

### Agregar Nuevas Series
Puedes agregar nuevas series directamente en el código o usar el panel de administración:

```javascript
{
    id: Date.now(),
    title: "Tu Nueva Serie",
    description: "Descripción de tu serie",
    slug: "tu-nueva-serie",
    chapters: [
        {
            id: Date.now(),
            title: "Capítulo 1",
            slug: "capitulo-1",
            chapterNumber: 1,
            images: ["url-imagen-1.jpg", "url-imagen-2.jpg"],
            isPublished: true,
            createdAt: new Date().toISOString()
        }
    ]
}
```

## 🌐 Hosting Recomendado

### Gratuitos (Recomendado para empezar)
- **GitHub Pages**: Integración perfecta con Git
- **Netlify**: Despliegue automático y fácil
- **Vercel**: Excelente rendimiento global
- **Firebase Hosting**: Integración con Google Cloud

### De Pago (Para proyectos serios)
- **DigitalOcean**: Droplets económicos y confiables
- **AWS S3 + CloudFront**: Escalabilidad infinita
- **Cloudflare Pages**: CDN global y rápido

## 🔒 Seguridad y Privacidad

✅ **100% Privado**: Todos los datos se guardan localmente en tu navegador  
✅ **Sin Servidores**: No hay servidores externos que puedan ser hackeados  
✅ **Sin Recolección de Datos**: No se recopila información personal  
✅ **Offline**: Los datos cargados se pueden ver sin conexión a internet  
✅ **Open Source**: Puedes revisar y modificar el código  

## 🚀 Limitaciones

- **Almacenamiento**: Limitado al espacio del navegador (5-10MB típicamente)
- **Imágenes**: Deben estar hosteadas externamente (Imgur, GitHub, etc.)
- **Concurrencia**: Solo un usuario por navegador
- **Backup**: Debes hacer backup manual de los datos

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica y moderna
- **CSS3**: Flexbox, Grid, animaciones y variables
- **Vanilla JavaScript**: Sin dependencias externas
- **LocalStorage**: API de almacenamiento del navegador
- **Responsive Design**: Mobile-first approach

## 📞 Soporte

- **Issues**: Reporta problemas en [GitHub Issues](https://github.com/tu-usuario/manga-library-static/issues)
- **Discusiones**: Participa en [GitHub Discussions](https://github.com/tu-usuario/manga-library-static/discussions)
- **Wiki**: Documentación adicional en [GitHub Wiki](https://github.com/tu-usuario/manga-library-static/wiki)

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! 

1. **Fork** este repositorio
2. **Crea** una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. **Commit** tus cambios (`git commit -am 'Añadir nueva funcionalidad'`)
4. **Push** a la rama (`git push origin feature/nueva-funcionalidad`)
5. **Abre** un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para detalles.

## 🙏 Agradecimientos

- **Iconos**: [Lucide Icons](https://lucide.dev/)
- **Fuentes**: System fonts para máxima compatibilidad
- **Inspiración**: Comunidades de manga y anime worldwide

## 📈 Roadmap

- [ ] Subida directa de imágenes
- [ ] Sistema de descargas (ZIP/PDF)
- [ ] Modo multiusuario
- [ ] Sincronización en la nube
- [ ] App móvil (PWA)
- [ ] Sistema de calificación
- [ ] Modo lectura nocturno mejorado
- [ ] Marcadores y favoritos
- [ ] Sistema de comentarios

---

**⭐ Si te gusta este proyecto, no olvides darle una estrella en GitHub!**

**🎉 ¡Tu biblioteca de mangas está lista para usar en cualquier lugar!**