# 🌳 Arbolado Público en CABA

Este proyecto explora el **arbolado público de la Ciudad de Buenos Aires**, utilizando un dataset oficial de datos abiertos.  

Se construye un flujo completo:
1. Obtención y carga del CSV en un entorno reproducible (Google Colab).  
2. Almacenamiento en una base de datos **SQLite** (ligera y portable).  
3. Consultas SQL básicas.  
4. Visualizaciones interactivas con **Plotly**.  

---

## 📂 Estructura del proyecto

```bash
arboles-caba/
├── data/                 # CSV con datos originales
│   └── arbolado.csv
├── notebooks/            # Notebooks de análisis
│   └── exploracion.ipynb
├── sql/                  # (Opcional) scripts SQL adicionales
└── README.md             # Documentación


---

## 📊 Dataset
- **Fuente:** [Gobierno de la Ciudad de Buenos Aires – Arbolado Público](https://data.buenosaires.gob.ar/dataset/arbolado-publico)  
- **Descripción:** Contiene información de árboles en vía pública: ubicación, especie, diámetro, altura, estado sanitario, entre otros.

---

## ⚙️ Requisitos

- Python 3.x  
- Librerías:
  - `pandas`
  - `sqlite3` (incluido en la stdlib de Python)
  - `plotly`

En Google Colab ya vienen instalados por defecto.

---

## 🚀 Instrucciones de uso

1. **Clonar el repositorio**:
   ```bash
   git clone https://github.com/nramrezmoreale/arboles-caba.git
   cd arboles-caba

	2.	Abrir el notebook en Google Colab:
	•	Ir a Google Colab
	•	Subir o abrir notebooks/exploracion.ipynb
	3.	Subir el CSV (data/arbolado.csv) al entorno de Colab (usando files.upload() o montando Google Drive).
	4.	Ejecutar todas las celdas para:
	•	Cargar los datos.
	•	Crear la base SQLite.
	•	Realizar consultas SQL.
	•	Generar gráficos y un mapa interactivo.

⸻

📈 Visualizaciones incluidas
	•	Cantidad de árboles por comuna.
	•	Especies más comunes (Top 10).
	•	Altura promedio por comuna.
	•	Distribución de diámetros de tronco.
	•	Mapa interactivo de árboles (muestra de 2000).

⸻

📌 Notas
	•	El CSV supera los 50 MB, por lo que se gestiona con Git LFS.
	•	Para reproducir el entorno localmente, asegurarse de tener instalado Git LFS:
  brew install git-lfs
  git lfs install


✍️ Autores: Nicolás Paul  Ramírez Moreale y Camila Funes
👨‍🏫 Profesor: Juan Carlos Cifuentes Durán
📅 Proyecto académico – Programación Avanzada para Ciencia de Datos, Universidad de la Ciudad de Buenos Aires  (2025)
