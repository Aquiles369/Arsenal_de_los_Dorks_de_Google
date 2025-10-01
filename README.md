<h1 align="center"><img height="40" src="https://github.com/Aquiles369/iconos/blob/main/img/lobo1.gif"><img height="40" src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExNWx4YTl1dW9scXlqZDk2cTdyY2VvcXQwMG40OGoxY25rZzV0MDZhcCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/peSyJWjNTRfzaWh49M/giphy.gif">"Google Dorks Arsenal"<img height="40" src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExNWx4YTl1dW9scXlqZDk2cTdyY2VvcXQwMG40OGoxY25rZzV0MDZhcCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/peSyJWjNTRfzaWh49M/giphy.gif"><img height="35" src="https://github.com/Aquiles369/iconos/blob/main/img/lobo1.gif"></h1>

<br>



<p align="center">
 <img  height="470rem" alt="GIF" src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExemV6OGJ2MmY0MWtjM2llcDdrbHlkbm9qZm5rZGhjaGhybWFicGQzcSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/XdLPY0v1jiPmsfp9ik/giphy.gif"/>
</p>

Tool_Google_dorks_12k

Repositorio con una colección extensa y categorizada de >12,000 Google Dorks pensada para investigación, análisis y pruebas en entornos controlados. Fácil de buscar, filtrar e integrar en tus pipelines y herramientas de reconocimiento.
Advertencia: uso responsable y legal únicamente — no escanees infraestructuras sin autorización. (Ver RESPONSIBLE_USE.md)


Resumen rápido

Colección: >12,000 dorks (formato web / dataset).

Categorías: incluye 14 categorías principales (≈7k dorks) + 4 categorías personalizadas extraidas de informes/medium/bug-bounty, y más de 30 subcategorías en total.

Formato: interfaz web local (HTML/JS) + export/import JSON. Toda la data se guarda en localStorage por defecto (offline, en tu máquina).

Licencias sugeridas: Código → MIT. Dataset (dorks) → CC0 (o la que elijas).

Características principales (presentación)

Interfaz intuitiva para buscar, filtrar y seleccionar dorks por categoría, subcategoría o texto.

Selector de objetivo (target) simple: ponés el dominio/host y elegís cuántos dorks lanzar y el intervalo entre requests (rate control).

Batch control: podés seleccionar abrir/executar 20 / 50 / N dorks a la vez, o deseleccionar individualmente.

Gestión completa: crear, editar o eliminar dorks individualmente; agregar categorías nuevas; borrar categorías completas.

Importación/Exportación: cargar/guardar todo en JSON (importá un JSON y la app recarga con tus dorks, notas y categorías).

Modo de edición masiva: pegar 1 dork por línea o cientos a la vez para añadir rápidamente.

Notas: podés añadir notas a cada categoría y a cada dork. Las notas se guardan con Ctrl+S (o botón guardar).

UI → cuando un dork/categoría tiene nota, se muestra un círculo rojo indicador; hover muestra contenido de la nota sin necesidad de abrir.

Buscador por categoría y por contenido (fulltext).

Reseteo rápido al estado por defecto si querés empezar de cero.

También tiene la opción para copiar todos los dorks de la categoría.

Export JSON con todas las notas y metadatos (listo para compartir o versionar).


Uso (modo web local)

Abrí index.html en tu navegador (o desplegalo en tu laboratorio local).

En Target, ingresá el dominio (ej.: example.com).

Seleccioná categoría(s) o buscá por palabra.

Elegí la cantidad de dorks a lanzar y el intervalo (ms) entre requests para controlar la velocidad.

Ejemplo: 50 dorks, intervalo 1500ms → evita bursts y reduce ruido.

Pulsá Start para abrir/ejecutar los dorks seleccionados.

Podés pausar / cancelar en cualquier momento.

Nota: la herramienta sólo genera las URLs de consulta (dork → site:TARGET + DORK) — no automatiza explotación ni crawling avanzado. Usá un proxy y/o tu tooling (Burp, httpx, etc.) si necesitás más control.

Gestión de dorks

Agregar: botón “Agregar Dorks” → pegar 1 por línea o subir JSON.

Editar: abrir dork → editar texto / nota / categoría.

Eliminar: por dork o por categoría completa.

Bulk: seleccionar múltiples dorks → acciones (abrir, exportar, borrar).

Etiquetas: asigná tags/flags para filtrar rápidamente (e.g., auth, sensitive, public-files).

Import / Export

Exportar: descarga JSON con estructura { categories:[], dorks:[], notes:[], meta:{timestamp, version} }.

Importar: subí JSON válido — la app reconstituye categorías, dorks y notas.

Recomendado: versioná tus exports (git / backups) antes de editar masivamente.

Notas y UI helpers

Guardado automático local (localStorage) + botón manual Ctrl+S para snapshot inmediato.

Indicador visual (círculo rojo) cuando una nota existe; hover muestra contenido completo (sin abrir).

Buscador avanzado por categoría, tag y texto de nota.

Panel de actividad: registro de las últimas acciones (última edición, import, export).
