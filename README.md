# unir_pdfs

Este script de Python combina todos los archivos PDF que se encuentran dentro de una carpeta específica en un solo archivo PDF.
Bastante útil cuando la teoría de un mismo tema está dividida por subtemas en diferentes PDFs.

---

## Cómo funciona

- El script toma la ruta de una carpeta donde se encuentran varios archivos PDF.
- Une todos los PDFs en un único archivo con el nombre de la carpeta.
  * Los archivos se unen en orden alfabético, por lo que conviene enumerarlos para definir el orden.
- Guarda el archivo combinado en la misma carpeta.

---

## Requisitos

- Python 3.6+
- Librería `PyPDF2`

Puedes instalar la librería necesaria con:

```bash
pip install PyPDF2
