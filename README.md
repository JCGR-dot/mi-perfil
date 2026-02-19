# Mi Perfil - Proyecto Laravel

Este proyecto es una aplicación web desarrollada en Laravel que muestra información personal en diferentes secciones: Perfil, Intereses, Habilidades y Metas.

## 📋 Requisitos Previos

Antes de comenzar, asegúrate de tener instalado lo siguiente:

- **PHP** >= 8.1
- **Composer** (gestor de dependencias de PHP)
- **Node.js** y **NPM** (opcional, para assets)
- **Git** (opcional, para clonar el repositorio)
- **XAMPP/WAMP/Laragon** (si trabajas en Windows) o **LAMP** (si trabajas en Linux)

## 🚀 Instalación Paso a Paso

### 1. Instalar PHP y Composer

#### En Windows:
1. Descarga PHP desde [windows.php.net/download](https://windows.php.net/download)
2. Descarga Composer desde [getcomposer.org](https://getcomposer.org/Composer-Setup.exe)
3. Ejecuta el instalador de Composer y sigue las instrucciones

#### En Linux (Ubuntu/Debian):
```bash
# Instalar PHP y extensiones necesarias
sudo apt update
sudo apt install php php-cli php-mbstring php-xml php-bcmath php-curl php-mysql php-zip unzip curl

# Instalar Composer
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
sudo chmod +x /usr/local/bin/composer