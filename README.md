# Reconocimiento de Mariposas con MATLAB :butterfly:

## By: TatoNaranjo | Santiago Naranjo Herrera

![MATLAB](https://img.shields.io/badge/MATLAB-%230076A8.svg?&style=for-the-badge&logo=matlab&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![App Designer](https://img.shields.io/badge/MATLAB%20App%20Designer-0076A8?style=for-the-badge&logo=matlab&logoColor=white)

## Tabla de Contenidos :page_with_curl:
- [Descripción del Proyecto](#descripción-del-proyecto)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Características Principales](#características-principales)
- [Dependencias](#dependencias)
- [Pasos de Instalación y Uso](#pasos-de-instalación-y-uso)
- [Dataset y Archivos](#dataset-y-archivos)
- [Licencia](#licencia)
- [Contacto](#contacto)

## Descripción del Proyecto :computer:
Este proyecto es un sistema para el **reconocimiento y clasificación de especies de mariposas** (como Monarca e Isabella) utilizando técnicas de **procesamiento de imágenes y machine learning** en MATLAB.

El sistema completo está construido usando **MATLAB App Designer**, proporcionando una interfaz gráfica de usuario (GUI) intuitiva para que los usuarios puedan:
1.  Aplicar diferentes filtros y kernels a las imágenes.
2.  Entrenar un modelo de red neuronal (Backpropagation).
3.  Clasificar nuevas imágenes de mariposas para identificar su especie.

## Tecnologías Utilizadas :black_nib:
![MATLAB](https://img.shields.io/badge/MATLAB-%230076A8.svg?&style=for-the-badge&logo=matlab&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)

## Características Principales :star:
El proyecto se divide en varios componentes modulares (aplicaciones `.mlapp`):

* **Procesamiento de Imágenes (`ProcesamientoKernels.mlapp`):** Una GUI para cargar imágenes, aplicar diversos kernels (definidos en `kernel.json`) como Sobel, Gaussiano, etc., y visualizar los resultados.
* **Entrenamiento del Modelo (`EntrenamientoU.mlapp`):** Interfaz dedicada a cargar los datasets (`X.txt`, `Y.txt`) y entrenar la red neuronal de Backpropagation.
* **Clasificación (`AplicacionBP.mlapp`):** La aplicación principal que utiliza el modelo ya entrenado para predecir la especie de una nueva imagen de mariposa cargada por el usuario.

## Dependencias :warning:
Para ejecutar este proyecto, necesitarás:

* **MATLAB** (Recomendado R2021a o superior).
* **Toolboxes de MATLAB:**
    * `Image Processing Toolbox`
    * `Deep Learning Toolbox` (o `Neural Network Toolbox`)

## Pasos de Instalación y Uso :checkered_flag:

1.  **Clona el repositorio**
    * Abre una terminal en tu computadora.
    * Ejecuta el siguiente comando para clonar el repositorio:
    ```bash
    git clone [https://github.com/TatoNaranjo/BPMariposas](https://github.com/TatoNaranjo/BPMariposas)
    ```

2.  **Abre el proyecto en MATLAB**
    * Inicia MATLAB.
    * Navega hasta la carpeta donde clonaste el repositorio.

3.  **Ejecuta las aplicaciones**
    * Puedes ejecutar cualquiera de las aplicaciones `.mlapp` escribiendo su nombre en la Command Window de MATLAB o haciendo doble clic sobre ellas.
    * **Para entrenar:** Ejecuta `EntrenamientoU.mlapp`.
    * **Para clasificar:** Ejecuta `AplicacionBP.mlapp`.
    * **Para probar filtros:** Ejecuta `ProcesamientoKernels.mlapp`.

## Dataset y Archivos :file_folder:
El proyecto incluye los siguientes archivos de datos clave:

* `X.txt` / `Y.txt`: Matriz de características (X) y etiquetas (Y) para el entrenamiento general.
* `X_Isabella.txt` / `X_Monarca.txt`: Archivos de características extraídas, específicas para las especies Isabella y Monarca.
* `kernel.json`: Un archivo de configuración JSON que define las matrices de los diferentes kernels de procesamiento de imágenes (Sobel, Gaussian Blur, etc.) utilizados en la app `ProcesamientoKernels.mlapp`.

## Licencia :door:
Este proyecto está licenciado bajo la [Licencia MIT](https://opensource.org/licenses/MIT).

## Contacto :computer:
Para preguntas o comentarios, puedes contactarme a través de mi [correo electrónico](mailto:naranjosa2004@gmail.com).
