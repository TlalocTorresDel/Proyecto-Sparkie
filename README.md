# Sistema de Recomendación de Libros - Proyecto Gutenberg

Sistema de recomendación basado en similitud de contenido usando PySpark y NLTK.

## Equipo
- Lopez Alvarez Maria De Los Angeles
- Torres Del Agua Tlaloc Enrique

## Instalación:
# Clonar repositorio
git clone https://github.com/tlaloctorresdel/proyecto-sparkie.git
cd proyecto-sparkie

# Crear entorno virtual
python3 -m venv venv
source venv/bin/activate

# Instalar dependencias
pip install -r requirements.txt

# Descargar recursos NLTK
python3 -c "import nltk; nltk.download('stopwords'); nltk.download('punkt')"
```

## Estructura del Proyecto
```
proyecto-sparkie/
├── data/
│   ├── raw/              # 100 libros del Proyecto Gutenberg (.txt)
│   └── processed/        # Datos procesados (vocabulario, matrices)
├── notebooks/            # Jupyter notebooks
│   └── ejemplos_profesor/  # Notebooks del profesor
├── src/                  # Código fuente Python
│   ├── procesamiento.py  # Procesamiento de texto y vocabulario
│   ├── similitud.py      # Matriz de similitudes con PySpark
│   └── recomendacion.py  # Sistema de recomendación
├── requirements.txt      # Dependencias del proyecto
├── DescargarPySpark.txt  # Lista original de paquetes
└── README.md
```

## Uso

### Activar entorno virtual
```bash
source venv/bin/activate
```

### Ejecutar Jupyter Lab
```bash
jupyter lab
```

### Ejecutar scripts
```bash
python src/procesamiento.py
```

## Tareas del Proyecto

- [x] Paso 1: Descargar 100 libros del Proyecto Gutenberg
- [x] Paso 2: Eliminar comentarios de inicio y fin
- [ ] Paso 3: Crear vocabulario (mayúsculas, limpieza, tokens, stopwords)
- [ ] Paso 4: Crear matriz de similitudes en PySpark
- [ ] Paso 5: Función de recomendación (N libros similares)
- [ ] Paso 6: Función de palabras descriptivas (M palabras por documento)

## Flujo de Trabajo Git
```bash
# Antes de trabajar
git pull origin main

# Después de trabajar
git add .
git commit -m "Descripción de cambios"
git push origin main
