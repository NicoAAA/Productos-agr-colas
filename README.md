Tienda Campesina Agro SENA

Este proyecto es una página web responsive construida con Bootstrap 5 y Sass, diseñada para promocionar y vender productos agrícolas de la iniciativa rural del SENA. El objetivo es ofrecer una experiencia visual atractiva, organizada y coherente con la paleta de colores y el estilo del campo.

📁 Estructura del proyecto

/mi-proyecto
│
├── index.html             # Página principal con la estructura HTML
├── package.json           # Configuración de NPM y scripts
├── node_modules/          # Dependencias instaladas (Bootstrap, Sass)
├── scss/
│   └── style.scss         # Hoja de estilos principal en SCSS
└── css/
    └── style.css          # CSS compilado (Bootstrap + overrides)
assets/
├── img/                   # Imágenes de productos y fondo (ej. campo.jpg, verduras.
|   └── logo.svg               # Logo ficticio de Agro SENA
├── fonts/                 # Tipografía personalizada (Feather Bold.ttf)


⚙️ Tecnologías y dependencias

Bootstrap 5 (SCSS) para layout, components y grid system.

Sass (Dart Sass) para preprocesar SCSS y personalizar la paleta de colores.

NPM para gestionar dependencias y scripts de compilación.

Dependencias principales en package.json:

{
  "dependencies": {
    "bootstrap": "^5.3.2"
  },
  "devDependencies": {
    "sass": "^1.x.x"
  }
}

🚀 Instalación y desarrollo

Clona o descarga el repositorio.

Abre terminal en la carpeta raíz del proyecto.

Instala las dependencias:

npm install

Enciende el compilador Sass en modo watch:

npm run sass:dev

Esto observará cambios en scss/style.scss y generará automáticamente css/style.css.

Abre index.html en tu navegador (o usa un servidor local como Live Server) para ver los cambios en tiempo real.

🖋️ Edición de estilos (SCSS)

Variables de paleta: en la parte superior de scss/style.scss se definen:

$primary:   #2a6f2b;  // Verde campo
$secondary: #f0c987;  // Amarillo trigo
$success:   #4a9d4a;  
$info:      #8ecae6;  
$body-color:#333;     // Texto principal

Import de Bootstrap:

@import "../node_modules/bootstrap/scss/bootstrap";

Overrides y personalizaciones:

Tipografía personalizada con @font-face.

Estilos para navbar, hero, cards, accordion, carousel, formulario y footer.

Componentes de Bootstrap (modal, carousel, accordion) integrados y estilizados.

🧩 Componentes destacados

Navbar responsive con logo e íconos de colapso.

Sección Hero con fondo de campo y botón que abre modal de video.

Grid de Productos con cards que muestran imágenes, títulos y botones.

Accordion de Servicios para describir asesoría, logística y talleres.

Carousel de Testimonios estilizado: citas en cursiva y autor resaltado.

Formulario de Contacto con campos básicos y botón personalizado.

Footer con datos legales y enlaces a redes sociales.

📌 Uso en producción

Genera CSS minificado:

npm run sass:build

Sube sólo index.html, la carpeta css/ (con style.css), assets/ y el archivo JS de Bootstrap.

Asegúrate de enlazar correctamente css/style.css y js/bootstrap.bundle.min.js.

🎨 Personalización

Cambia la paleta de colores modificando las variables SCSS.

Agrega o quita secciones duplicando los patrones de Bootstrap.

Sustituye imágenes en assets/img/ con contenido real o ficticio.

Actualiza íconos usando Bootstrap Icons o tu propia librería.

