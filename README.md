# Sistema de Gestión de Citas Médicas 🏥

Una aplicación web completa y moderna para la programación y gestión de citas médicas, diseñada para optimizar la organización de consultorios o clínicas.

## 🚀 Tecnologías Utilizadas

Este proyecto utiliza una arquitectura monolítica moderna (SPA) impulsada por el ecosistema de Laravel y herramientas frontend de vanguardia:

- **Backend:** Laravel (PHP)
- **Frontend:** Vue.js 3
- **Conector:** Inertia.js (El puente perfecto entre Laravel y Vue sin necesidad de crear una API REST)
- **Estilos:** Tailwind CSS 
- **Gráficos:** Chart.js y vue-chartjs para el panel de administración
- **Base de Datos:** MySQL
- **Notificaciones:** Sistema de correos (Mailable de Laravel)

## ✨ Características Principales

*   **Autenticación y Roles:** Acceso seguro diferenciado para Pacientes y Administradores.
*   **Gestión de Horarios (Schedules):** Los administradores pueden definir horas de disponibilidad para recibir citas.
*   **Reserva de Citas:** Los pacientes pueden agendar consultas médicas de manera intuitiva y rápida.
*   **Dashboard Administrativo:** Panel de control con gráficos y estadísticas en tiempo real usando Chart.js para medir la actividad del consultorio.
*   **Notificaciones por Correo Electrónico:** 
    *   Correos automáticos de confirmación al agendar una cita.
    *   Correos de recordatorio de citas próximas (con opción de envío manual desde el panel).

## 🛠️ Instalación Local

Si deseas correr este proyecto localmente, sigue estos pasos:

1.  **Clonar el repositorio:**
    ```bash
    git clone https://github.com/santiagoxx93/citas-medicasproyecto.git
    cd citas-medicasproyecto
    ```

2.  **Instalar dependencias de PHP y Node:**
    ```bash
    composer install
    npm install
    ```

3.  **Configurar variables de entorno:**
    Copia el archivo `.env.example` y renómbralo a `.env`.
    ```bash
    cp .env.example .env
    ```
    Configura tus credenciales de base de datos y de servidor de correos (ej. Mailtrap para pruebas) en el archivo `.env`.

4.  **Generar la key de la aplicación:**
    ```bash
    php artisan key:generate
    ```

5.  **Correr migraciones (y seeders si existen):**
    ```bash
    php artisan migrate
    ```

6.  **Compilar los assets de frontend y levantar el servidor:**
    Abre dos pestañas de tu terminal:
    ```bash
    # Pestaña 1
    npm run dev
    
    # Pestaña 2
    php artisan serve
    ```

7.  Visita `http://localhost:8000` en tu navegador.

## 📄 Manual de Usuario
El repositorio incluye un archivo llamado `Manual de Usuario Citas-Medicas.pdf` con la explicación detallada visual y operativa del sistema.

---
*Desarrollado para demostrar habilidades construyendo SPAs modernas con el stack VILT (Vue, Inertia, Laravel, Tailwind).*
