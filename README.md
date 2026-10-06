# Laravel Admin Panel (SB Admin 2)

Este proyecto consiste en la integración y despliegue de la plantilla **SB Admin 2** en un proyecto de **Laravel**.

## Descripción de la Tarea

La tarea principal de este repositorio ha sido tomar una plantilla HTML estática (SB Admin 2) y desplegarla correctamente dentro de la estructura de un proyecto Laravel. Esto incluye:

- Ubicación correcta de los recursos públicos (`css`, `js`, `img`, `vendor`) en la carpeta `public/`.
- Uso del helper `asset()` en las vistas de Blade para cargar los estilos y scripts adecuadamente.
- Creación de rutas (`routes/web.php`) y controladores (`TemplateController`) para servir la vista de la plantilla.
- Integración de la vista principal en `resources/views/template/template.blade.php`.

## Requisitos

- PHP >= 8.1
- Composer
- Servidor web (Apache, Nginx, o el servidor integrado de PHP)

## Instalación y Configuración

Sigue estos pasos para levantar el entorno de desarrollo:

1. **Instalar dependencias de Composer:**
   ```bash
   composer install
   ```

2. **Configurar el entorno:**
   Copia el archivo de ejemplo para crear tu `.env`:
   ```bash
   cp .env.example .env
   ```

3. **Generar la clave de la aplicación:**
   ```bash
   php artisan key:generate
   ```

4. **Levantar el servidor local:**
   ```bash
   php artisan serve
   ```
   *El proyecto estará disponible en `http://localhost:8000`.*

## Estructura de Archivos Relevantes

- **Vista Principal:** `resources/views/template/template.blade.php`
- **Controlador:** `app/Http/Controllers/TemplateController.php`
- **Ruta:** La ruta principal `/` está configurada en `routes/web.php` para apuntar a la plantilla.
- **Assets:** Se encuentran en la carpeta `public/` organizados por carpetas (`css`, `img`, `js`, `scss`, `vendor`).
