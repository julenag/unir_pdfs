import os
from PyPDF2 import PdfMerger

# Ruta de la carpeta donde están los PDFs
carpeta = r"RUTA/A/LA/CARPETA"  # <-- Cambia esto por la ruta real

# Obtener el nombre de la carpeta (para usarlo como nombre de archivo)
nombre_carpeta = os.path.basename(os.path.normpath(carpeta))

# Crear objeto para combinar PDFs
merger = PdfMerger()

# Obtener todos los archivos PDF de la carpeta
pdfs = [f for f in os.listdir(carpeta) if f.lower().endswith('.pdf')]
pdfs.sort()  # Opcional: para unirlos en orden alfabético

# Añadir cada PDF al archivo combinado
for pdf in pdfs:
    ruta_pdf = os.path.join(carpeta, pdf)
    merger.append(ruta_pdf)

# Guardar el resultado
salida = os.path.join(carpeta, f"{nombre_carpeta}.pdf")
merger.write(salida)
merger.close()

print(f"PDFs combinados correctamente en: {salida}")
