📦 credenciales-app/
├── input/
│   ├── fotos/                    # Fotos originales del personal
│   └── firmas/                   # Firmas originales en JPEG
├── output/
│   ├── fotos/                    # Fotos recortadas y procesadas
│   └── firmas/                   # Firmas optimizadas y redimensionadas
├── core/
│   ├── face_processor.py         # Lógica de procesamiento facial (vacío por ahora)
│   └── signature_processor.py    # Lógica de procesamiento de firmas
├── utils/
│   ├── file_utils.py             # Funciones auxiliares para manejo de archivos
│   └── image_utils.py            # Utilidades de imagen (saturación, resize, etc.)
├── ui/
│   └── main_window.py            # Interfaz gráfica (futura implementación)
├── config.py                     # Configuración global del proyecto
├── main.py                       # Punto de entrada principal
└── requirements.txt              # Dependencias del proyecto

🧠 Objetivo general:
Automatizar el proceso de generación de credenciales para el personal,
procesando automáticamente más de 1000 fotos y firmas por tanda.

📌 Etapa 1: Firmas
- Aumentar saturación y contraste para que se vean bien.
- Opcional: limpiar fondo blanco.
- Redimensionar a tamaño estándar.
- Guardar con el mismo nombre en carpeta /output.

📌 Etapa 2: Fotos
- Detectar rostro.
- Recortar imagen incluyendo pecho, cara y un pequeño margen por encima de la cabeza.
- Redimensionar a tamaño estándar.
- Guardar en carpeta /output.

✨ Próximas funcionalidades:
- Vista previa en interfaz gráfica.
- Parámetros ajustables desde la GUI.
- Logs y control de errores.
- Exportación en PDF (futuro opcional).

🚀 Estado actual:
Estructura creada y lista para implementar el procesamiento de firmas.
