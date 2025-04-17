# Administrador de Aplicaciones

Aplicación web para gestionar, catalogar y respaldar aplicaciones de diferentes tipos (web, móvil, escritorio, API, etc.).

## Características principales

- **Listado y búsqueda** de aplicaciones con filtros por nombre, tipo y descripción.
- **Importación** de datos desde texto o archivos en formato CSV/tabulado.
- **Exportación** a Excel (CSV) y vista de impresión.
- **Backup**: descarga de copia de seguridad en formato `.json`.
- **Restauración**: recuperación de datos desde un archivo `.json` de backup.
- **Edición, eliminación y renumeración** de registros.
- **Gestión de tipos** de aplicaciones personalizables.

## Uso rápido

1. **Descarga o clona este repositorio.**
2. Abre el archivo `Admin_AAA.html` en tu navegador.
3. Utiliza los botones de la parte superior para agregar, importar, exportar, hacer backup o restaurar tus aplicaciones.

## Formatos de importación soportados

- **Simple:**  
  ```
  Nombre: URL
  ```
  Ejemplo:
  ```
  Google: https://www.google.com
  Facebook: https://www.facebook.com
  ```

- **CSV/Tabulado:**  
  ```
  ID,Nombre,Tipo,URL,Descripción,Comentarios
  1,App1,web,https://app1.com,Descripción1,Comentario1
  2,App2,desktop,https://app2.com,Descripción2,Comentario2
  ```

## Backup y restauración

- **Backup:**  
  Haz clic en el botón `Backup` para descargar un archivo `.json` con todos tus datos actuales.
- **Restaurar:**  
  Haz clic en `Restaurar` y selecciona un archivo `.json` previamente guardado para recuperar tus datos.

## Requisitos

- Navegador web moderno (Chrome, Edge, Firefox, etc.).
- No requiere instalación ni servidor.

## Estructura del archivo de backup

El archivo de backup es un `.json` que contiene un arreglo de objetos con los siguientes campos:

```json
[
  {
    "id": 1,
    "name": "Nombre de la app",
    "type": "web",
    "url": "https://ejemplo.com",
    "description": "Descripción",
    "comments": "Comentarios"
  }
]
```

## Créditos

Elaborado por: Ing. Jesus Tordoya Cornejo  
Junio 2024

---

**Sugerencia:**  
Puedes modificar y personalizar este archivo `README.md` según evolucione tu aplicación.
