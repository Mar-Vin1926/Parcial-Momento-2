"# Parcial-Momento-2" 
# Aplicación de Análisis Básico de Ventas con Streamlit y Pandas

Esta es una aplicación web interactiva desarrollada con Streamlit y Pandas para analizar datos de ventas desde un archivo CSV. Permite cargar un conjunto de datos, aplicar filtros por categoría de producto y rango de precios, y muestra estadísticas clave como el total de ventas y el precio promedio de los productos filtrados.

## Funcionalidades Principales

* **Carga de Datos:** Permite cargar un archivo `sales_data.csv` para el análisis.
* **Visualización Completa:** Muestra el conjunto de datos cargado en una tabla interactiva.
* **Filtrado por Categoría:** Ofrece un menú desplegable en la barra lateral para filtrar los datos por una categoría de producto específica (Electronics o Accessories).
* **Filtrado por Rango de Precios:** Permite seleccionar un rango de precios mínimo y máximo mediante un control deslizante en la barra lateral.
* **Visualización de Datos Filtrados:** Muestra una tabla con los datos que cumplen con los criterios de filtrado seleccionados, indicando el número de registros resultantes.
* **Estadísticas Clave:** Calcula y muestra el total de ventas y el precio promedio de los productos dentro de los datos filtrados, utilizando métricas destacadas.

## Cómo Ejecutar la Aplicación

Sigue estos pasos para ejecutar la aplicación en tu entorno local:

1.  **Clonar el Repositorio (Opcional):** Si tienes este proyecto en un repositorio Git, clónalo a tu máquina local.

    ```bash
    git clone https://github.com/Mar-Vin1926/Parcial-Momento-2.git
    ```

2.  **Crear y Activar el Entorno Virtual:** Asegúrate de tener Python instalado en tu sistema. Navega al directorio del proyecto y crea un entorno virtual para aislar las dependencias:

    * **Para `venv` (módulo integrado de Python):**

        ```bash
        python -m venv venv
        # Activar el entorno virtual (dependiendo de tu sistema operativo)
        # En Windows:
        venv\Scripts\activate
        # En macOS y Linux:
        source venv/bin/activate
        ```

    * **Para `conda` (si estás usando Anaconda):**

        ```bash
        conda create --name mi_entorno python=[tu versión de Python preferida]
        conda activate mi_entorno
        ```

3.  **Instalar las Dependencias:** Utiliza el archivo `requirements.txt` para instalar las librerías necesarias:

    ```bash
    pip install -r requirements.txt
    ```

4.  **Ejecutar la Aplicación Streamlit:** Navega al directorio del proyecto (donde se encuentra `sales_app.py`) y ejecuta el siguiente comando:

    ```bash
    streamlit run sales_app.py
    ```

    Esto abrirá automáticamente la aplicación en tu navegador web. Si no se abre automáticamente, busca la URL en la terminal (generalmente comienza con `http://localhost:8501`).

## Estructura del Proyecto

EXAMEN/
├── static/
│   └── sales_data.csv      # Archivo de datos de ventas
├── sales_app.py            # Código de la aplicación Streamlit
├── requirements.txt        # Lista de dependencias
└── README.md               # Este archivo
└── generate_data.py

## Notas Adicionales

* Asegúrate de que el archivo `sales_data.csv` esté ubicado dentro de la carpeta `static` para que la aplicación pueda cargarlo correctamente.
* Puedes modificar el archivo `sales_data.csv` con tus propios datos de ventas, siempre y cuando mantenga las columnas necesarias (`Date`, `Product`, `Category`, `Price`, `Quantity`, `Total_Sales`).

¡Disfruta explorando tus datos de ventas con esta aplicación!