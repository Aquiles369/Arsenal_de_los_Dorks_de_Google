# Changelog

Todos los cambios notables en este proyecto se documentarán en este archivo.

Formato basado en "Keep a Changelog".  
SemVer usado: MAJOR.MINOR.PATCH

## [Unreleased]
- Planeado: integración con export presets (httpx, burp) y selector de sensibilidad por dork.
- Planeado: añadir modos de sandbox para pruebas locales.

## [1.0.0] - 2025-10-03
### Added
- Publicación inicial del dataset: **12,000 dorks** organizados en ~47+ categorías.
- Interfaz web local (HTML/JS) con búsqueda en vivo, filtros por categoría/etiqueta/texto.
- Selector de objetivo (Target) para convertir dork → `site:{TARGET} {DORK}`.
- Batch control: seleccionar y ejecutar/abrir 20 / 50 / N dorks con control de intervalo (ms).
- Import/Export JSON con estructura completa `{ categories:[], dorks:[], notes:[], meta:{timestamp, version} }`.
- Edición masiva: pegar 1 dork por línea o subir cientos a la vez.
- Gestión completa: crear, editar y eliminar dorks y categorías; acciones en masa (abrir, exportar, borrar).
- Notas por dork y categoría con indicador visual y preview on-hover.
- Guardado automático en localStorage + Snapshot manual (Ctrl+S).
- Panel de actividad que registra últimas acciones (import, export, edición).
- Opción para copiar todos los dorks de una categoría.
- Funcionalidad para resetear al estado por defecto.

### Security
- Advertencia y recomendación de uso responsable: la herramienta **no** debe usarse para escaneo no autorizado.
- La app **no** automatiza explotación ni crawling avanzado; solo genera URLs de consulta.

### Notes
- Recomendado usar proxy (Burp, httpx) para ejecutar consultas y controlar tráfico.
- Versionar exports antes de operaciones masivas.

