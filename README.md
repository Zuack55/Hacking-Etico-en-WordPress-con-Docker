# Hacking Ético en WordPress con Docker

![Banner](./imgwp.png)

## Descripción
Laboratorio práctico y sencillo que muestra cómo levantar una instancia vulnerable de **WordPress** con **Docker** y realizar un ejercicio básico de reconocimiento y explotación —todo en un entorno controlado.  
El objetivo es aprender los pasos típicos de una auditoría: levantar el target, enumerar, identificar usuarios, probar contraseñas y, finalmente, ver el impacto al tener acceso al panel de administración.

> ⚠️ **Solo para fines educativos.** Ejecuta estas pruebas únicamente en entornos controlados y con permiso explícito. No ataques sistemas ajenos ni entornos de producción.

## Qué contiene este repositorio
- Configuración para levantar un WordPress vulnerable con **Docker Compose** (basado en `dvwp`).
- Instrucciones paso a paso para:
  - Levantar el entorno con Docker.
  - Enumerar directorios y recursos.
  - Escanear con `wpscan`.
  - Enumerar usuarios y probar fuerza bruta con `rockyou.txt`.
  - Acceder al panel y hacer una modificación simple en el tema (ejemplo de post-explotación).
- `banner.png` — imagen de cabecera (colócala en la raíz del repo).

## Requisitos
- Sistema Linux (recomendado: Ubuntu 20.04)  
- Docker y Docker Compose  
- Máquina de pruebas (p. ej. Kali) con herramientas: `wpscan`, `dirb`, wordlists como `rockyou.txt`
