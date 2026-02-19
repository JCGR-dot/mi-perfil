# Taller Básico Laravel – Mi Perfil (UNAB)

## Descripción breve
Proyecto desarrollado para el **Taller Básico de Introducción a Laravel (UNAB)**.  
La aplicación muestra un perfil personal dividido en cuatro secciones (**Perfil**, **Intereses**, **Habilidades** y **Metas**) utilizando **rutas en `web.php`** y **vistas Blade**.  
El diseño se realiza con **CSS propio (sin Bootstrap)**, aplicando tipografía legible, paleta de colores, espaciados consistentes y ajustes responsive.

---

## Requisitos del sistema
- **PHP** (compatible con la versión de Laravel usada en el proyecto)
- **Composer**
- Terminal (PowerShell/CMD/Git Bash)
- Navegador web (Chrome/Edge/Firefox)
- Servidor local:
  - Recomendado: **servidor integrado de Laravel** con `php artisan serve`
  - Alternativa: **XAMPP/WAMP/MAMP** (apuntando a la carpeta `public/`)
- (Opcional) **Git** (si deseas clonar y manejar commits)


---

## Instrucciones de instalación

### Opción A — Instalación con Git (clonar repositorio)
1. Clona el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
2. Entra a la carpeta del proyecto:
   ```bash
   cd nombre-del-proyecto
3. Instala dependencias:
   ```bash
   composer install
4. Crea el archivo .env a partir del ejemplo:
   ```bash
   Linux/Mac/Git Bash
   
   cp .env.example .env
   
   Windows (PowerShell)
   
   Copy-Item .env.example .env
   
   Windows (CMD)
   
   copy .env.example .env
5. Genera la clave de la aplicación:
   ```bash
   php artisan key:generate
---

### Opción B — Instalación sin Git (descargar ZIP)
1. Descarga el proyecto como archivo ZIP.

2. Descomprime el ZIP en una carpeta local (ejemplo: Documentos/mi-perfil-laravel/).

3. Abre una terminal dentro de la carpeta del proyecto.

4. Instala dependencias:
   ```bash
   composer install
5. Crea el archivo .env:
     ```bash
     Windows (PowerShell)
   
     Copy-Item .env.example .env

     Windows (CMD)

     copy .env.example .env
     
     Linux/Mac/Git Bash

     cp .env.example .env
6. Genera la clave de la aplicación:
    ```bash
    php artisan key:generate
---

### Cómo ejecutar el proyecto
Opción recomendada — Servidor integrado de Laravel
1. Inicia el servidor:
   ```bash
   php artisan serve
2. Abre en el navegador:

- http://127.0.0.1:8000/perfil

- http://127.0.0.1:8000/perfil/intereses

- http://127.0.0.1:8000/perfil/habilidades

- http://127.0.0.1:8000/perfil/metas

> Para detener el servidor: CTRL + C en la terminal.

---
### Opción alternativa — XAMPP/Apache
Laravel funciona correctamente cuando el servidor web apunta a la carpeta public/.

1. Coloca el proyecto dentro de htdocs (si usas XAMPP).

2. Configura tu servidor para que apunte a:
    ```text
    nombre-del-proyecto/public
3. Accede en el navegador (ejemplo):
    ```bash
    http://localhost/nombre-del-proyecto/public/perfil
---
### Documentación del proyecto
Rutas disponibles
| Ruta                  | Vista                   | Descripción                               |
| --------------------- | ----------------------- | ----------------------------------------- |
| `/perfil`             | `perfil.blade.php`      | Muestra información general del perfil    |
| `/perfil/intereses`   | `intereses.blade.php`   | Muestra intereses y pasatiempos           |
| `/perfil/habilidades` | `habilidades.blade.php` | Muestra habilidades técnicas              |
| `/perfil/metas`       | `metas.blade.php`       | Muestra metas a corto/mediano/largo plazo |


Estructura de archivos relevante

- routes/web.php

  Contiene las rutas del taller.
- resources/views/

  Contiene las vistas Blade:

  - perfil.blade.php

  - intereses.blade.php

  - habilidades.blade.php

  - metas.blade.php

- public/css/estilos.css

Archivo de estilos CSS propio (sin Bootstrap).

Enlace del CSS en las vistas

Todas las vistas enlazan el CSS así:

<link rel="stylesheet" href="{{ asset('css/estilos.css') }}">

---

### Solución de problemas (rápida)
- Composer no se reconoce: reinstala Composer o revisa PATH y reinicia la terminal.

- PHP no se reconoce: revisa instalación de PHP/XAMPP y PATH (php -v).

- CSS no carga: confirma public/css/estilos.css y recarga con CTRL + F5.

- “View not found”: verifica que la vista exista en resources/views/ y el nombre coincida con la ruta.

---

### Autor y fecha
- Autor: Juan Camilo Gómez Roa

- Fecha: 2026-02-18