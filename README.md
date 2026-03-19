# 🏥 Clínica App - Orquestador y Entorno de Desarrollo

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)

Este repositorio actúa como el **orquestador principal** para el ecosistema de Clínica App. Utiliza **Git Submodules** para integrar de forma limpia el backend y el frontend, y **Docker Compose** para levantar todo el entorno de desarrollo con un solo comando.

## 🚀 Demostración del Sistema

> **Nota:** El sistema está diseñado para uso interno y no se encuentra desplegado de forma pública por motivos de privacidad de datos, pero puedes ver el flujo principal a continuación.

![Demo del Sistema]([ENLACE_A_TU_GIF_AQUI_O_ARRASTRA_LA_IMAGEN_DIRECTO_A_GITHUB])

## 🏗️ Arquitectura del Proyecto

El sistema está dividido en microservicios gestionados a través de submódulos para separar responsabilidades y facilitar la escalabilidad:

* **[clinica-api]([https://github.com/Charlyqv/clinica-api]):** Backend desarrollado en **PHP 8 / Laravel**. Expone una API RESTful segura y gestiona la lógica de negocio.
* **[clinica-belleza-app]([https://github.com/Charlyqv/clinica-belleza-app]):** Frontend desarrollado como una Single Page Application (SPA) utilizando **React y Vite**.
* **Base de Datos:** Contenedor aislado de **MySQL 8.0**.

## ⚙️ Instalación y Configuración Rápida

Para replicar este entorno en cualquier equipo, asegúrate de tener instalado [Docker](https://www.docker.com/) y [Git](https://git-scm.com/).

**1. Clonar el repositorio con sus submódulos:**
Es crucial utilizar el flag `--recurse-submodules` para descargar el código del API y del Frontend simultáneamente.

```bash
git clone --recurse-submodules [https://github.com/Charlyqv/clinica-app.git](https://github.com/Charlyqv/clinica-app.git)
cd clinica-app