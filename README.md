# mi-api-fastapi-python

API REST minimalista construida con Python, FastAPI y Uvicorn.

## Autor
**Juan Esteban Diaz Galindo**  
Semillero de Investigación de Teleinformática CEET

## Tecnologías utilizadas
- Python 3
- FastAPI
- Uvicorn

## Estructura del proyecto
```
mi-api-fastapi-python/
├── main.py
├── requirements.txt
└── README.md
```

## Instalación y ejecución

### 1. Clonar el repositorio
```cmd
git clone <URL-del-repositorio>
cd mi-api-fastapi-python
```

### 2. Crear y activar el entorno virtual
```cmd
python -m venv venv
venv\Scripts\activate.bat
```

### 3. Instalar dependencias
```cmd
pip install -r requirements.txt
```

### 4. Ejecutar el servidor
```cmd
uvicorn main:app --reload
```

## Endpoints disponibles

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| GET | `/` | Retorna `{"Hello": "World"}` |
| GET | `/items/{item_id}` | Retorna el item por ID con parámetro opcional `q` |

## Documentación automática

Con el servidor en ejecución, accede a:

- **Swagger UI:** http://127.0.0.1:8000/docs
- **ReDoc:** http://127.0.0.1:8000/redoc