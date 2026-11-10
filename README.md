# Trabajo Práctico Especial: Staged Kidney Disease (CKD-NHANES 2021-2023)

Fundamentos de la Ciencia de Datos, cursada 2026. Grupo 3.

Análisis exploratorio, limpieza y validación de hipótesis sobre el dataset CKD-NHANES 2021-2023 (enfermedad renal crónica).

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `CodeTPE.ipynb` | Notebook con todo el análisis, organizada en secciones |
| `CKD-NHANES/CKD_NHANES_2021_2023.csv` | Dataset utilizado |
| `CKD-NHANES/metadata.docx` | Descripción de las variables del dataset |
| `requirements.txt` | Librerías necesarias para ejecutar la notebook |

## Organización de la notebook

1. Carga de datos
2. Exploración inicial
3. Limpieza de datos
4. Análisis exploratorio de los datos
5. Hipótesis univariada: porcentaje de fumadores actuales frente a la referencia del CDC
6. Hipótesis bivariada: capacidad de filtrado (eGFR) en hombres y mujeres
7. Hipótesis multivariada: marcadores renales y BMI frente a la diabetes diagnosticada
8. Hipótesis 4a: etnia de los casos de CKF
9. Hipótesis 4b: presión arterial como factor de riesgo del CKF
10. Hipótesis 4c: factores asociados a la probabilidad de presentar CKD

## Requisitos

- Python 3.14 (probado con Python 3.14.8). Con versiones más viejas de Python, algunas de las versiones de `requirements.txt` pueden no instalarse.
- pip
- Git (opcional, solo para clonar el repositorio). Sin Git, se puede descargar el repositorio desde GitHub con *Code → Download ZIP* y descomprimirlo.

## Instrucciones de ejecución

1. Clonar el repositorio y entrar a la carpeta:

   ```bash
   git clone https://github.com/FranGonzalez354/TPE_fundamentos.git
   cd TPE_fundamentos
   ```

   Si se descargó el ZIP, entrar a la carpeta descomprimida (`TPE_fundamentos-main`).

2. Crear y activar un entorno virtual:

   En Linux o macOS:

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

   En Windows (PowerShell):

   ```powershell
   py -m venv .venv
   .venv\Scripts\Activate.ps1
   ```

   Si PowerShell no permite ejecutar el script de activación, correr antes `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass`. En Windows (cmd), activar con `.venv\Scripts\activate.bat`.

3. Instalar las dependencias:

   ```bash
   pip install -r requirements.txt
   ```

4. Abrir Jupyter Lab:

   ```bash
   jupyter lab
   ```

5. Abrir `CodeTPE.ipynb` y ejecutar todas las celdas en orden (menú *Run → Run All Cells*).

La notebook lee el dataset desde la ruta relativa `CKD-NHANES/CKD_NHANES_2021_2023.csv`, por lo que debe ejecutarse desde la carpeta raíz del repositorio.
