# Sistema de control de accesos.

**Secuara** es una plataforma diseñada para gestionar, monitorear y controlar el ingreso y salida de personas, vehículos y proveedores en conjuntos residenciales, empresas, oficinas y otros espacios privados o semi-privados.

El sistema permite mejorar la seguridad, optimizar procesos administrativos y centralizar la información en tiempo real.

---

## 🎯 Objetivos del Proyecto

- Garantizar la seguridad de los residentes, empleados y visitantes.
- Automatizar el registro de accesos.
- Reducir errores humanos en el control manual.
- Facilitar la administración de permisos.
- Generar reportes y estadísticas.
- Integrar dispositivos físicos y software.

## 🏗️ Arquitectura del Sistema

El sistema está compuesto por tres capas principales:

### 1️⃣ Capa de Presentación

- Aplicación Web
- Aplicación Móvil
- Panel Administrativo

### 2️⃣ Capa de Lógica de Negocio

API REST
- Servicios de autenticación
- Gestión de permisos
- Procesamiento de accesos

### 3️⃣ Capa de Datos

- Base de datos relacional
- Almacenamiento de logs
- Backups automáticos

## 🧩 Módulos Principales

Para el desarrollo del MVP (Producto Mínimo Viable), el sistema se divide en módulos esenciales que permiten validar el producto en el mercado con el menor costo y tiempo posible.

### 👤 1. Módulo de Gestión de Usuarios

Permite administrar todas las personas que interactúan con el sistema.

Funciones principales:

- Registro de residentes, empleados y administradores.
- Asignación de roles (Administrador, Portero, Usuario).
- Gestión de credenciales de acceso.
- Activación y desactivación de cuentas.
- Recuperación y cambio de contraseña.

**Objetivo MVP: Garantizar control básico de usuarios y permisos.**

### 🚪 2. Módulo de Control de Accesos

Encargado de validar y registrar todos los ingresos y salidas.

Funciones principales:

- Registro manual y automático de accesos.
- Validación por QR, PIN o credencial.
- Control por horarios.
- Alertas por accesos no autorizados.
- Historial de movimientos.

Objetivo MVP: Registrar accesos de forma confiable y centralizada.

### 🏷️ 3. Módulo de Gestión de Visitantes

- Permite administrar las visitas temporales.
- Funciones principales:
- Pre-registro de visitantes.
- Generación de códigos QR.
- Autorización por parte del residente o administrador.
- Control de vigencia de invitaciones.
- Historial de visitas.

Objetivo MVP: Reducir tiempos de ingreso y mejorar trazabilidad.

### 🚗 4. Módulo de Control Vehicular

- Administra el acceso de vehículos.
- Funciones principales:
- Registro de placas.
- Asociación vehículo–usuario.
- Control de parqueaderos.
- Registro de entradas y salidas vehiculares.
- Reporte de ocupación.

Objetivo MVP: Gestionar parqueaderos sin sistemas complejos.

### 📊 5. Módulo de Reportes y Auditoría

Permite visualizar la información generada.

Funciones principales:

- Reportes diarios y mensuales.
- Búsqueda por usuario o fecha.
- Exportación básica (PDF/Excel).
- Registro de acciones del sistema.

Objetivo MVP: Brindar información clave para administración y control.

### ⚙️ 6. Módulo de Configuración del Sistema

- Centraliza los parámetros generales.
- Funciones principales:
- Definición de horarios.
- Reglas de acceso.
- Gestión de dispositivos.
- Parámetros de seguridad.
- Personalización básica.

Objetivo MVP: Permitir adaptación mínima a cada cliente.

### 📱 7. Módulo de Interfaz de Portería

Diseñado para el personal operativo.

Funciones principales:

- Registro rápido de visitas.
- Escaneo de QR.
- Visualización de autorizaciones.
- Alertas en tiempo real.
- Acceso simplificado.

Objetivo MVP: Optimizar el trabajo del personal de seguridad.

### 🌐 8. Módulo Web/App para Usuarios

Permite a residentes y empleados gestionar su acceso.

Funciones principales:

- Generar invitaciones.
- Consultar historial.
- Actualizar datos.
- Recibir notificaciones.

Objetivo MVP: Dar autonomía al usuario sin sobrecargar al administrador.

### 🔌 9. Módulo de Integración (Opcional MVP)

Permite conectar el sistema con hardware o terceros.

Funciones principales:

- Integración con lectores QR.
- Conexión con cámaras.
- API externa.

Exportación de datos.

Objetivo MVP: Preparar el sistema para escalamiento futuro.

### 🔐 Seguridad

El sistema implementa múltiples niveles de seguridad:

Autenticación con JWT/OAuth

- Cifrado de contraseñas
- Control de roles
- Registros de auditoría
- Protección contra ataques
- Respaldos periódicos

### 🛠️ Tecnologías Utilizadas

- API REST
- **Backend:** Python
- **Framework:** fastAPI
- **Frontend:** React
- **Base de Datos:** PostgreSQL

### Infraestructura

- Docker
- AWS
