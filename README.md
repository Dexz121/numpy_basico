numpy-basico

Pequeña guía para correr y guardar el notebook del repositorio.

Requisitos

Python 3.10+

pip (y opcional: virtualenv o venv)

Ejecutar localmente (Jupyter)
# Clonar tu fork (recomendado forkar antes en GitHub)
git clone https://github.com/<TU-USUARIO>/numpy_basico.git
cd numpy_basico

# (opcional) entorno virtual
python3 -m venv venv && source venv/bin/activate

# Instalar dependencias mínimas
pip install -U pip
pip install jupyter numpy  # agrega otras si el notebook las pide

# Lanzar Jupyter
jupyter notebook


Abre el .ipynb, Run All, y guarda (Ctrl+S).

Para subir cambios:

git add *.ipynb
git commit -m "Run all cells and save outputs"
git push origin main

Ejecutar en Google Colab (rápido)

Fork del repo en GitHub.

En Colab: File → Open notebook → GitHub, pega la URL de tu fork.

Runtime → Run all.

File → Save a copy to GitHub (elige tu fork y mismo path).

Estructura típica
numpy_basico/
├─ <notebook>.ipynb
├─ README.md
└─ (otros archivos/datos si aplica)

Notas

Si una celda requiere paquetes extra, instálalos dentro del notebook:

!pip install paquete


Si el repo original actualiza, puedes sincronizar tu fork con upstream.
