# BLUprint Lite — Registro de cambios

Resumen de cambios visibles para los usuarios.

El formato sigue [Keep a Changelog](https://keepachangelog.com/) y el
proyecto usa [Versionado Semántico](https://semver.org/lang/es/).

## 0.1.2 — 2026-05-02

- Primera prueba del sistema de actualización automática.

## 0.1.1 — 2026-05-01

- **Actualizaciones automáticas con un solo clic.** Cuando publicamos una
  versión nueva, la app muestra un banner arriba. Pulsa **Actualizar
  ahora** y la app hace `git pull`, instala dependencias si hace falta,
  y recarga sola. Tus proyectos (`bluprint.db`) y medios
  (`bluprint-media/`) no se tocan.
- **Ocultar el @handle del autor** — toggle global desde el inspector
  que esconde la marca del autor en todas las diapositivas del
  proyecto. Útil cuando importas un hilo pero no quieres mostrar el
  handle en el resultado final.
- **Instalación con `git clone`** — la guía pasó de descargar el ZIP a
  clonar el repo. Es lo que habilita el botón de actualizar en un solo
  clic (el endpoint hace `git pull` por ti).

## 0.1.0 — 2026-04-30

Lanzamiento inicial.
