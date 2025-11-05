# 🛡️ Análisis de Seguridad Móvil con MobSF

## 📚 Proyecto de Sistemas Distribuidos
Este proyecto implementa un sistema para el análisis de seguridad en aplicaciones móviles utilizando **Mobile Security Framework (MobSF)** dentro de contenedores **Docker**, facilitando una instalación y ejecución rápidas.

---

### 🚀 Instalación Rápida

Sigue estos sencillos pasos para poner en marcha el sistema:

1.  **Clonar proyecto:**
    ```bash
    git clone [https://github.com/Sterwinc/Mobile-Security.git](https://github.com/Sterwinc/Mobile-Security.git)
    ```

2.  **Ejecutar:**
    ```bash
    cd Mobile-Security
    docker-compose up -d
    ```

3.  **Acceder a MobSF:** Abre tu navegador y navega a la siguiente dirección:
    * **URL:** `http://localhost:8000`
4.  **Credenciales de Acceso:**
    * **Usuario:** `mobsf`
    * **Contraseña:** `mobsf`

---

## 🛠️ Características Principales

* Análisis automático de archivos **APK** (Android).
* Detección de **vulnerabilidades de seguridad** comunes.
* Generación de **reportes detallados** y exportables.
* Arquitectura robusta con **contenedores Docker** para aislamiento y portabilidad.
* Configuración simplificada mediante `docker-compose`.
* Interfaz web intuitiva para la gestión y visualización.
* Análisis estático de código descompilado.
* Detección de **permisos peligrosos** y uso inseguro de APIs.
* Scan de componentes de Android (Activities, Services, Providers).
* **API REST** para integraciones automatizadas (CI/CD).

---

## 📋 Requisitos del Sistema

Para ejecutar este proyecto de forma óptima, necesitas:

* **Docker** instalado y configurado.
* **Docker Compose** (generalmente incluido en las instalaciones modernas de Docker).
* Mínimo de **2 GB de RAM** libres.
* **1 GB de espacio libre** en disco.
* Conexión a internet (para la descarga inicial de imágenes Docker).

---

## 🎯 Cómo Usar el Proyecto

| Paso | Acción | Descripción |
| :--- | :--- | :--- |
| **1. Instalación** | `docker-compose up -d` | Inicia el contenedor MobSF en segundo plano. |
| **2. Acceso** | Abrir `http://localhost:8000` | Accede a la interfaz web de MobSF. |
| **3. Login** | Usar `mobsf`/`mobsf` | Iniciar sesión con las credenciales predeterminadas. |
| **4. Análisis** | Subir archivo APK | Arrastra o sube el archivo APK que deseas auditar. |
| **5. Resultados** | Revisar el reporte | Analiza la puntuación de seguridad y los detalles de las vulnerabilidades encontradas. |

---

## 🏗️ Arquitectura del Sistema

El flujo de trabajo se basa en contenedores Docker para garantizar un entorno de análisis limpio y reproducible:

```text
Cliente Web (Navegador) 
    → Contenedor MobSF (Docker)
        → Módulo de Análisis de Seguridad
            → Análisis Estático (Código Fuente)
            → Detección de Vulnerabilidades
                → Generación de Reportes (PDF/HTML)
```
🔧 Comandos Útiles para GestiónUtiliza estos comandos de docker-compose para administrar tu entorno MobSF:ComandoDescripcióndocker-compose up -dIniciar la aplicación y ejecutar los contenedores en segundo plano.docker-compose downDetener y eliminar los contenedores y redes creados por Compose.docker-compose logs -fVer los logs de los servicios en tiempo real.docker-compose psVer el estado actual de los contenedores.docker-compose restartReiniciar el servicio MobSF.docker statsVer el uso de recursos (CPU, RAM) de los contenedores activos.
