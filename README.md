# 🎨 Generador de Fractales con Números Complejos

Este proyecto permite generar imágenes de fractales a partir de polinomios complejos definidos por el usuario. Utiliza operaciones matemáticas sobre números complejos y un sistema de convergencia de Newton para visualizar en el plano complejo.

---

## 📁 Archivos del Proyecto

- `Proyecto.py`: Implementa las clases para números complejos, polinomios, y el generador de fractales.
- `pruebas.py`: Contiene pruebas unitarias que verifican el correcto funcionamiento de las clases.
- `parametros.txt`: Archivo de configuración que define cómo se generará el fractal (tamaño, polinomio, colores, etc.).

---

## 📄 Formato del archivo `parametros.txt`

Este archivo contiene los parámetros que el programa lee para generar la imagen fractal:

```txt
min : -2-2i               # Esquina inferior izquierda del plano complejo
max : 2+2i                # Esquina superior derecha del plano complejo
width : 1024              # Ancho de la imagen en píxeles
height : 1024             # Alto de la imagen en píxeles
degree : 2                # Grado del polinomio
polynomial : (1+0i)z^2 + (-1+0i)   # Polinomio complejo en notación personalizada
iterations : 30           # Máximo de iteraciones para determinar convergencia
threshold : 3             # Distancia máxima para considerar convergencia a una raíz
color : (255,100,50)      # Color base del fractal (puede modificarse)
name : fractal3.png       # Nombre del archivo de salida
```

---

## 🖼️ Generación del fractal

1. Edita `parametros.txt` con tus valores deseados.
2. Ejecuta el archivo `Proyecto.py`:

```bash
python Proyecto.py
```

Esto generará una imagen PNG del fractal con las especificaciones dadas.

---

## 🧪 Pruebas unitarias

Para verificar la correcta implementación de las clases y métodos:

```bash
python pruebas.py
```

Las pruebas cubren:
- Suma, resta, multiplicación y potencia de números complejos
- Evaluación y derivación de polinomios
- Parsing de configuraciones y generación de fractales

---

## 🧠 Requisitos

- Python 3.7 o superior
- Librería **Pillow** para manipulación de imágenes:

```bash
pip install pillow
```

---

## 💡 Créditos

Este proyecto fue desarrollado como parte de una práctica de visualización de fractales y álgebra compleja.

---

## ✅ Ejemplo visual

(Si lo deseas, aquí puedes añadir una imagen generada como ejemplo)
