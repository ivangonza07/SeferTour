# SeferTour

## 📖 Descripción

Aplicación web de gestión de tours/viajes desarrollada con el framework **Laravel 8**. El proyecto proporciona una plataforma para la reserva y gestión de paquetes turísticos.

## 🚀 Características

- **Framework Laravel 8** - Arquitectura MVC robusta
- **Sistema de autenticación** - Registro e inicio de sesión de usuarios
- **Panel de administración** - Gestión de tours y reservas
- **Base de datos MySQL** - Almacenamiento de datos persistente
- **Diseño responsive** - Interfaz adaptable a diferentes dispositivos

## 📋 Requisitos

- **PHP** 7.3 o superior
- **Composer** - Gestor de dependencias PHP
- **MySQL** 5.7+ o **MariaDB**
- **Node.js** y **npm** - Para compilación de assets

## 🛠️ Tecnologías

| Tecnología | Versión | Descripción |
|------------|---------|-------------|
| Laravel | 8.x | Framework PHP |
| PHP | 7.3+ | Lenguaje del servidor |
| MySQL | 5.7+ | Base de datos |
| Blade | - | Motor de plantillas |
| Bootstrap | 4.x | Framework CSS |
| jQuery | 3.x | Librería JavaScript |

## 📁 Estructura del Proyecto

```
SeferTour/
├── app/                    # Código de la aplicación
│   ├── Http/               # Controladores y middleware
│   ├── Models/             # Modelos Eloquent
│   └── Providers/          # Proveedores de servicios
├── bootstrap/              # Archivos de arranque
├── config/                 # Configuración de la aplicación
├── database/               # Migraciones y seeders
│   ├── migrations/
│   └── seeders/
├── public/                 # Archivos públicos (index.php, assets)
├── resources/              # Vistas y assets
│   ├── views/              # Plantillas Blade
│   ├── css/
│   └── js/
├── routes/                 # Definición de rutas
│   └── web.php
├── storage/                # Logs, cache, sesiones
├── tests/                  # Pruebas unitarias
├── composer.json           # Dependencias PHP
├── package.json            # Dependencias Node.js
├── webpack.mix.js          # Configuración de Webpack
└── docker-compose.yml      # Configuración Docker
```

## 🔧 Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/ivangonza07/SeferTour.git
cd SeferTour
```

### 2. Instalar dependencias PHP

```bash
composer install
```

### 3. Configurar entorno

```bash
cp .env.example .env
```

Edita el archivo `.env` con tus credenciales de base de datos:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=sefertour
DB_USERNAME=root
DB_PASSWORD=
```

### 4. Generar clave de aplicación

```bash
php artisan key:generate
```

### 5. Ejecutar migraciones

```bash
php artisan migrate
```

### 6. Instalar dependencias Node.js (opcional)

```bash
npm install
npm run dev
```

### 7. Iniciar servidor

```bash
php artisan serve
```

La aplicación estará disponible en `http://localhost:8000`

## 🐳 Docker (Alternativa)

El proyecto incluye configuración Docker:

```bash
docker-compose up -d
```

## 📖 Uso

1. **Registro**: Crea una cuenta en `/register`
2. **Inicio de sesión**: Accede en `/login`
3. **Explorar tours**: Navega por el catálogo disponible
4. **Reservar**: Selecciona y reserva tu tour

## 👤 Autor

**Ivan Gonzalez**
- 🐙 GitHub: [@ivangonza07](https://github.com/ivangonza07)

## 📄 Licencia

Este proyecto está licenciado bajo la [MIT License](https://opensource.org/licenses/MIT).
