# Generador de Fractales con Números Complejos

Este proyecto permite generar imágenes de fractales a partir de polinomios complejos definidos por el usuario. Utiliza operaciones matemáticas sobre números complejos y un sistema de convergencia de Newton para visualizar en el plano complejo.

---

## Archivos del Proyecto

- `Proyecto.py`: Implementa las clases para números complejos, polinomios, y el generador de fractales.
- `pruebas.py`: Contiene pruebas unitarias que verifican el correcto funcionamiento de las clases.
- `parametros.txt`: Archivo de configuración que define cómo se generará el fractal (tamaño, polinomio, colores, etc.).

---

## Estructura del Código

### Clase `NumeroComplejo`

- `__init__`
- `_verificar_instancia`
- `__add__`, `__sub__`, `__mul__`, `__pow__`
- `modulo`
- `__repr__`
- `_copia`

### Clase `PolinomioComplejo`

- `__init__`
- `evaluar`

### Clase `ParsearPolinomios`

- `cadena_a_complejo`
- `parsear_complejo`
- `parsear_terminos`
- `construir_coeficientes`
- `parsear_polinomio`

### Clase `BuscarPatrones`

- `__init__`
- `_limpiar_expresion`
- `_extraer_complejo`
- `_extraer_exponente`
- `_recorrer_expresion`
- `encontrar_todo`

### Clase `LecturaValores`

- `__init__`
- `interpretar_valor`
- `leer_configuracion_fractal`

### Clase `GeneradorFractales`

- `__init__`
- `_mapear_pixel_a_complejo`
- `determinar_color_pixel`
- `_calcular_color`
- `generar`
- `guardar_imagen`

---

## Formato del archivo `parametros.txt`

Este archivo contiene los parámetros que el programa lee para generar la imagen fractal:

```txt
min : -2-2i
max : 2+2i
width : 1024
height : 1024
degree : 2
polynomial : (1+0i)z^2 + (-1+0i)
iterations : 30
threshold : 3
color : (255,100,50)
name : fractal3.png
```

---

## Generación del fractal

1. Edita `parametros.txt` con tus valores deseados.
2. Ejecuta el archivo `Proyecto.py`:

```bash
python Proyecto.py
```

Esto generará una imagen PNG del fractal con las especificaciones dadas.

---

## Pruebas unitarias

Para verificar la correcta implementación de las clases y métodos:

```bash
python pruebas.py
```

Las pruebas cubren:
- Suma, resta, multiplicación y potencia de números complejos
- Evaluación y derivación de polinomios
- Parsing de configuraciones y generación de fractales

---

## Requisitos

- Python 3.7 o superior
- Librería Pillow para manipulación de imágenes:

```bash
pip install pillow
```

---

## Créditos

Este proyecto fue desarrollado como parte de una práctica de visualización de fractales y álgebra compleja.
