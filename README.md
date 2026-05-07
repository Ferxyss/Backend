# Innovatech Frontend

Frontend del sistema Innovatech desarrollado para la Evaluación Parcial N°2 de la asignatura Introducción a Herramientas DevOps.

---

## Tecnologías Utilizadas

- Vue / Vite
- Docker
- Docker Hub
- GitHub Actions
- AWS EC2
- Nginx
- Linux

---

## Características Implementadas

- Contenedorización mediante Docker.
- Dockerfile multi-stage.
- Usuario no root.
- Pipeline CI/CD automatizado.
- Publicación automática en Docker Hub.
- Deploy automático en AWS EC2.
- Integración con backend privado.
- Uso de Security Groups para segmentación.

---

## Arquitectura

La solución implementa:

- EC2 pública para Frontend.
- EC2 privada para Backend.
- Comunicación interna mediante IP privada.
- Automatización de despliegue con GitHub Actions.

---

## CI/CD

El pipeline realiza automáticamente:

1. Build de imagen Docker.
2. Push a Docker Hub.
3. Deploy automático en EC2 Frontend vía SSH.

---

## Docker Hub

Imagen utilizada:

```bash
ferxyss/innovatech-frontend:latest
```

---

## Ejecución Local

```bash
docker build -t innovatech-frontend .
docker run -d -p 80:80 innovatech-frontend
```

---

## Seguridad Implementada

- Usuario no root.
- Backend privado.
- Security Groups.
- Secrets en GitHub Actions.
- SSH mediante llave PEM.

---

## Integrante

- Fernanda Paredes

---

## Asignatura

**ISY1101 - Introducción a Herramientas DevOps**
