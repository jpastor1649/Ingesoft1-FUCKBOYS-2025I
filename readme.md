# Examen Práctico – Computación Visual  
**Periodo:** I-2025  
**Fecha límite de entrega:** Sábado 19 de julio, 1:00 p.m.  

---

## Instrucciones Generales

- Suba su examen a su **repositorio individual** en GitHub o GitLab con el siguiente nombre:

```

examen-computacion-visual-\[nombre-apellido]

```

- El repositorio debe ser **público** o estar **compartido con el docente**.
- Envíe el enlace del repositorio a través del siguiente formulario antes de la hora límite:  
[Formulario de Entrega](https://docs.google.com/forms/d/e/1FAIpQLSc-7w_ukei6X-waIamKt8pfdqsEsbaP08_UZN_VgskwL52sMg/viewform?usp=header)
- Todos los ejercicios deben estar correctamente documentados con `README.md`.

---

## Ejercicio 1: Procesamiento de Imagen y Detección con YOLO

**Descripción:**  
A partir de una imagen proporcionada por el docente (enlace: [Imagenes del examen](https://drive.google.com/drive/folders/133X_0FgdeDC6N-xe6CZWC1i8pLhPRxv5)), realice el procesamiento de imagen y la detección de objetos.

**Actividades:**

1. Cargar la imagen en Python con OpenCV.
2. Aplicar un filtro de suavizado (Gaussiano o Mediana).
3. Aplicar un filtro de detección de bordes (Sobel o Canny).
4. Visualizar las tres etapas:  
 - Imagen original  
 - Imagen suavizada  
 - Bordes detectados
5. Detectar objetos con YOLOv5 o YOLOv8 (modelo preentrenado).
6. Mostrar imagen con bounding boxes y etiquetas.

**Estructura esperada:**

```

ejercicio\_1\_procesamiento/
├── procesamiento.py
├── resultados/
│   ├── suavizado.png
│   ├── bordes.png
│   ├── deteccion\_yolo.png
└── README.md

```

---

## Ejercicio 2: Pirámide Escalonada 3D con React Three Fiber

**Descripción:**  
Crear una escena 3D en React con React Three Fiber, que contenga una pirámide hecha de cajas con materiales PBR.

**Template base en CodeSandbox:**  
[https://codesandbox.io/p/sandbox/threejs-basic-example-uvcc6](https://codesandbox.io/p/sandbox/threejs-basic-example-uvcc6)

**Sitios recomendados para texturas PBR:**
- https://ambientcg.com  
- https://polyhaven.com/textures

**Actividades:**

1. Hacer fork del template y nombrarlo como:  
   `piramide-[nombre-apellido]`
2. Construir la pirámide con múltiples `Box`.
3. Aplicar materiales PBR (diffuse, normal, roughness, etc.).
4. Agregar iluminación adecuada.
5. Incluir controles de cámara (`OrbitControls`).

**Estructura esperada:**

```

ejercicio\_2\_piramide\_3d/
├── README.md         # Incluir enlace al sandbox y descripción
├── captura.png       # Captura de la escena
└── texturas/         # Si usó texturas locales

```

---

## Ejercicio 3: Convolución Unidimensional en Python

**Descripción:**  
Implementar desde cero una función en Python que realice una convolución 1D entre una señal y un kernel.

**Actividades:**

1. Definir una señal de entrada de 10 a 20 valores.
2. Definir un kernel de tamaño 3 (ej. `[1, 0, -1]` o `[1/3, 1/3, 1/3]`).
3. Implementar la función de convolución **sin usar `numpy.convolve`**.
4. Graficar la señal, el kernel y el resultado con `matplotlib`.

**Estructura esperada:**

```

ejercicio\_3\_convolucion\_1d/
├── convolucion.py
├── graficos/
│   ├── señal\_original.png
│   ├── kernel.png
│   └── resultado.png
└── README.md

```

---

## Estructura Final del Repositorio

```

examen-computacion-visual-\[nombre-apellido]/
│
├── ejercicio\_1\_procesamiento/
│   ├── procesamiento.py
│   ├── resultados/
│   └── README.md
│
├── ejercicio\_2\_piramide\_3d/
│   ├── README.md
│   ├── captura.png
│   └── texturas/
│
├── ejercicio\_3\_convolucion\_1d/
│   ├── convolucion.py
│   ├── graficos/
│   └── README.md

```