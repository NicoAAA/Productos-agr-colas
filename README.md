# Tienda Campesina Agro SENA

Este proyecto es una página web responsive construida con **Bootstrap 5** y **Sass**, diseñada para promocionar y vender productos agrícolas de la iniciativa rural del SENA. El objetivo es ofrecer una experiencia visual atractiva, organizada y coherente con la paleta de colores y el estilo del campo.

---

## 📁 Estructura del proyecto

```
/Productos-agr-colas
│
├── index.html             # Página principal con la estructura HTML
├── package.json           # Configuración de NPM y scripts
├── node_modules/          # Dependencias instaladas (Bootstrap, Sass)
├── scss/
│   └── style.scss         # Hoja de estilos principal en SCSS
└── css/
    └── style.css          # CSS compilado (Bootstrap + overrides)
assets/
├── img/                   # Imágenes de productos y fondo (ej. campo.jpg, verduras.jpg)
|   |
|   └── logosena.svg           # Logo ficticio de Agro SENA
|   └── cards/             # Carpeta con las imagenes de las cards
|   └── hero/              # Carpeta con las imagenes del hero
|
└── fonts/                 # Tipografía personalizada (Feather Bold.ttf)

```

---

## ⚙️ Tecnologías y dependencias

* **Bootstrap 5** (SCSS) para layout, components y grid system.
* **Sass (Dart Sass)** para preprocesar SCSS y personalizar la paleta de colores.
* **NPM** para gestionar dependencias y scripts de compilación.

Dependencias principales en `package.json`:

```json
{
  "dependencies": {
    "bootstrap": "^5.3.2"
  },
  "devDependencies": {
    "sass": "^1.x.x"
  }
}
```

---

## 🚀 Instalación y desarrollo

1. Clona o descarga el repositorio.
2. Abre terminal en la carpeta raíz del proyecto.
3. Instala las dependencias:

   ```bash
   npm install
   ```
4. Enciende el compilador Sass en modo `watch`:

   ```bash
   npm run sass:dev
   ```

   Esto observará cambios en `scss/style.scss` y generará automáticamente `css/style.css`.
5. Abre `index.html` en tu navegador (o usa un servidor local como Live Server) para ver los cambios en tiempo real.

---

## 🖋️ Edición de estilos (SCSS)

* **Variables de paleta**: en la parte superior de `scss/style.scss` se definen:

  ```scss
  $primary:   #2a6f2b;  // Verde campo
  $secondary: #f0c987;  // Amarillo trigo
  $success:   #4a9d4a;  
  $info:      #8ecae6;  
  $body-color:#333;     // Texto principal
  ```
* **Import de Bootstrap**:

  ```scss
  @import "../node_modules/bootstrap/scss/bootstrap";
  ```
* **Overrides y personalizaciones**:

  * Tipografía personalizada con `@font-face`.
  * Estilos para navbar, hero, cards, accordion, carousel, formulario y footer.
  * Componentes de Bootstrap (modal, carousel, accordion) integrados y estilizados.

---

## 🧩 Componentes destacados

1. **Navbar** responsive con logo e íconos de colapso.
2. **Sección Hero** con fondo de campo y botón que abre modal de video.
3. **Grid de Productos** con cards que muestran imágenes, títulos y botones.
4. **Accordion de Servicios** para describir asesoría, logística y talleres.
5. **Carousel de Testimonios** estilizado: citas en cursiva y autor resaltado.
6. **Formulario de Contacto** con campos básicos y botón personalizado.
7. **Footer** con datos legales y enlaces a redes sociales.

---

## 📌 Uso en producción

1. Genera CSS minificado:

   ```bash
   npm run sass:build
   ```
2. Sube sólo `index.html`, la carpeta `css/` (con `style.css`), `assets/` y el archivo JS de Bootstrap.
3. Asegúrate de enlazar correctamente `css/style.css` y `js/bootstrap.bundle.min.js`.

---

## 🎨 Personalización

* Cambia la paleta de colores modificando las variables SCSS.
* Agrega o quita secciones duplicando los patrones de Bootstrap.
* Sustituye imágenes en `assets/img/` con contenido real o ficticio.
* Actualiza íconos usando [Bootstrap Icons](https://icons.getbootstrap.com/) o tu propia librería.

---

**¡Listo!** Con esta guía podrás entender y extender la Tienda Campesina Agro SENA. Cualquier duda, revisa el código o abre un issue.
