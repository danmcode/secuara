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
Funciones principales:
- Creacción de estructura, de Torres -> apartamentos, Lostes -> Casas, Bloques -> Oficinas etc.
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
- 
Objetivo MVP: Dar autonomía al usuario sin sobrecargar al administrador.

### 📝 9. Módulo de Minutas y Novedades

Permite al personal de portería o seguridad registrar eventos relevantes durante su turno.

Funciones principales:

- Registro de novedades diarias.
- Bitácora de turnos.
- Registro de incidentes, visitas especiales y situaciones anómalas.
- Adjuntar evidencias (fotos o documentos).
- Consulta histórica por fecha y responsable.

Objetivo MVP: Centralizar la información operativa y mejorar la trazabilidad de eventos.


### 🔌 10. Módulo de Integración (Opcional MVP)

Permite conectar el sistema con hardware o terceros.

Funciones principales:

- Integración con lectores QR.
- Conexión con cámaras.
- API externa.

Exportación de datos.

Objetivo MVP: Preparar el sistema para escalamiento futuro.

### 📦 11. Módulo de Correspondencia

Permite gestionar la recepción, entrega y control de paquetes, cartas y encomiendas.

Funciones principales:

- Registro de correspondencia entrante.
- Asociación con residente o empresa.
- Notificación automática al destinatario.
- Registro de entrega con firma o confirmación.
- Historial de correspondencia.

Objetivo MVP: Reducir pérdidas y mejorar el control de paquetes.

### ✅ 12. Módulo de Tareas y Supervisión

Permite al administrador asignar y supervisar actividades del personal de seguridad.

Funciones principales:

- Creación de tareas para guardas y ronderos.
- Asignación por turno o zona.
- Definición de horarios y prioridades.
- Confirmación de cumplimiento.
- Reporte de tareas realizadas.

Objetivo MVP: Mejorar la operación y supervisión del personal en campo.

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

## 🚀 Escalamiento y Expansión del Software

Esta sección reúne ideas estratégicas para convertir el sistema en una plataforma integral y transversal para empresas de administración, seguridad y organizaciones.

### 1. 📞 Citofonía Digital Integrada

- Integración con el sistema de control de accesos.
- Comunicación directa con residentes desde portería o app.
- Apertura remota de accesos.
- Registro automático de llamadas.

### 2. 👤 Conexión con Reconocimiento Facial

- Integración con cámaras inteligentes.
- Identificación automática de personas autorizadas.
- Alertas por rostros no registrados.
- Mejora de tiempos de ingreso.

### 3. 🚗 Reconocimiento de Placas Vehiculares

- Lectura automática de placas.
- Validación en tiempo real.
- Control de parqueaderos sin contacto.
- Integración con barreras vehiculares.

### 4. 🏢 Gestión Administrativa de Activos

Módulos para la administración transversal de recursos físicos y financieros.

- Gestión de activos (tanques, plantas, equipos, energía).
- Control de mantenimientos.
- Administración de proveedores.
- Gestión de contratos.
- Manejo de facturas y pagos.
- Reportes financieros.

Objetivo: Convertir el sistema en una plataforma integral para copropiedades, empresas y firmas de seguridad.

### 5. 🌐 Plataforma Multientidad

Administración centralizada de múltiples sedes.

- Panel para empresas administradoras.
- Gestión de varios clientes desde una sola cuenta.
- Roles empresariales avanzados.

### 6. 📊 Analítica Avanzada y BI

- Dashboards ejecutivos.
- Indicadores de desempeño.
- Predicción de riesgos.
- Optimización operativa.

### 7. 🤖 Automatización e Inteligencia Artificial

- Detección automática de anomalías.
- Sugerencias de seguridad.
- Análisis de patrones.

Optimización de recursos.

### 8. 🔗 Ecosistema de Integraciones

- Marketplace de integraciones.
- Conexión con ERPs.
- APIs para terceros.
- Integración con sistemas gubernamentales (según normativa).

### 9. 🛡️ Programación Inteligente de Guardas con IA

Módulo avanzado para la gestión dinámica del personal de seguridad mediante inteligencia artificial.

Funciones principales:

- Programación automática de turnos.
- Monitoreo de ausencias en tiempo real.
- Identificación del guarda disponible más cercano.
- Optimización de tiempos de respuesta.
- Reasignación automática de puestos.
- Consideración de descansos, horas extra y cargas laborales.

Objetivo: Garantizar continuidad del servicio y máxima cobertura de seguridad con mínima intervención humana.

**Por qué este módulo es clave para vender**

Con esto puedes decirle a una empresa de seguridad:

“Nuestro sistema reduce fallas por ausencias y optimiza automáticamente su operación”.

Eso significa:

✅ Menos supervisores
✅ Menos errores humanos
✅ Menos sanciones por incumplimiento
✅ Mejor servicio al cliente

= Más dinero para ellos → más fácil vender.

A futuro, este módulo puede evolucionar a:

🚀 Nivel avanzado:

- Predicción de ausencias
- Fatiga laboral
- Riesgo de fallas
- Recomendaciones de rotación
- Optimización por zonas críticas
Se vuelve casi un Waze de guardas

### 10. 🗺️ Mapa Inteligente de Riesgos y Zonas Críticas

Módulo colaborativo basado en inteligencia artificial para identificar y visualizar zonas con alta incidencia delictiva o riesgo operativo.

Funciones principales:

- Mapa georreferenciado de incidentes.
- Identificación de focos de riesgo.
- Análisis predictivo de zonas peligrosas.
- Integración con reportes de empresas afiliadas.
- Alertas preventivas para rondas y patrullajes.
- Historial por zona y periodo.

Objetivo: Mejorar la prevención del delito y optimizar la planeación de recorridos mediante información compartida e inteligente.

------

## 💼 Modelo de Negocio (SaaS)

Secuara opera bajo un modelo **Software como Servicio (SaaS)**, enfocado
en el mercado Latinoamericano, iniciando en Colombia.

### Esquema de Cobro

El costo del servicio se define según el número de **usuarios activos**
registrados en la plataforma:

Incluye: - Residentes - Empleados - Guardas - Administrativos -
Colaboradores

### Planes Referenciales LATAM

  Plan|Usuarios|Precio USD/Mes
  -|-|-
  Básico        |Hasta 100   |30 -- 50
  Profesional   |Hasta 500   |80 -- 120
  Empresarial   |Ilimitado   |200+

### Add-ons

-   Inteligencia Artificial
-   Mapas de Riesgo
-   Reconocimiento Facial
-   Integraciones Avanzadas

### Ventajas

-   Escalable
-   Predecible
-   Transparente
-   Adaptado a LATAM

------------------------------------------------------------------------

© 2026 Secuara - Plataforma de Seguridad Inteligente
