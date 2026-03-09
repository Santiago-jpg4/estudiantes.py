# Estudiantes - Gestión de Información de Estudiantes

Este es un programa simple en Python que permite gestionar información de estudiantes mediante una clase llamada `Estudiante`.

## Descripción

La clase `Estudiante` proporciona funcionalidades básicas para:

- **Crear** un registro de estudiante con nombre, edad y calificación
- **Calcular** si el estudiante aprueba o reprueba según su calificación
- **Mostrar** la información completa del estudiante

## Estructura de la Clase

### Atributos

| Atributo | Descripción |
|----------|-------------|
| `nombre` | Nombre completo del estudiante |
| `edad` | Edad del estudiante |
| `calificación` | Calificación del estudiante (0-5) |

### Métodos

#### `__init__(self, nombre, edad, calificacion)`
Constructor que inicializa un nuevo estudiante con los parámetros proporcionados.

**Parámetros:**
- `nombre` (str): Nombre completo del estudiante
- `edad` (int): Edad del estudiante
- `calificacion` (float): Calificación del estudiante (escala 0-5)

#### `calcular_aprobacion(self)`
Calcula si el estudiante aprueba o reprueba según su calificación.

**Retorna:**
- `str`: "Aprobado" si la calificación es mayor o igual a 3, de lo contrario "Reprobado"

#### `mostrar_informacion(self)`
Muestra por consola la información completa del estudiante formateada en un recuadro, incluyendo:
- Nombre
- Edad
- Calificación
- Estado de aprobación

## Ejemplo de Uso

```python
if __name__ == "__main__":
    # Registro de estudiantes
    estudiante1 = Estudiante("Juan Pérez", 20, 2.5)
    estudiante2 = Estudiante("María López", 19, 4.5)
    estudiante3 = Estudiante("Alberto Perez", 29, 2.9)
    
    # Mostrar información de los estudiantes
    estudiante1.mostrar_informacion()
    estudiante2.mostrar_informacion()
    estudiante3.mostrar_informacion()
```

## Salida Esperada

```
==============================
INFORMACIÓN DEL ESTUDIANTE
==============================
Nombre: Juan Pérez
Edad: 20
Calificación: 2.5
Estado: Reprobado
==============================
==============================
INFORMACIÓN DEL ESTUDIANTE
==============================
Nombre: María López
Edad: 19
Calificación: 4.5
Estado: Aprobado
==============================
==============================
INFORMACIÓN DEL ESTUDIANTE
==============================
Nombre: Alberto Perez
Edad: 29
Calificación: 2.9
Estado: Reprobado
==============================
```

## Criterio de Aprobación

| Calificación | Estado |
|--------------|--------|
| >= 3.0 | Aprobado |
| < 3.0 | Reprobado |

## Requisitos

- Python 3.x

## Cómo Ejecutar

```bash
python Estudiantes.py
```

## Licencia

Este es un proyecto educativo de ejemplo.

