# Proyecto TTS

Instructivo rápido para preparar el entorno, instalar dependencias.

## Requisitos
- Python 3.10.x instalado

## Pasos

1) Crear y activar un entorno virtual (recomendado `.venv`)

Windows (PowerShell):

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Si PowerShell bloquea la ejecución, ejecutar (si es necesario):

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

Windows (CMD):

```cmd
python -m venv .venv
.venv\Scripts\activate.bat
```

macOS / Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

2) Instalar dependencias

```bash
pip install --upgrade pip
pip install -r Requirements.txt
```

3) Ejecutar el código

Este repositorio incluye el notebook `TTS.ipynb`.

Abrir con Jupyter:

```bash
python -m notebook TTS.ipynb
# o
jupyter notebook TTS.ipynb
```

Si tu proyecto tiene un script de entrada (por ejemplo `main.py`), ejecuta:

```bash
python main.py
```

## Problemas comunes
- Si falta alguna librería, revisa el contenido de `Requirements.txt` y reinstala.
- Si hay errores de versión de Python, asegúrate de usar Python 3.10.x.
