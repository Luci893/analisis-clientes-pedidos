# Desafío técnico: Análisis de clientes y pedidos

## Descripción

Proyecto de procesamiento y análisis de datos desarrollado en Python para explorar información de clientes y pedidos de un negocio.

El trabajo utiliza dos archivos CSV relacionados mediante el identificador de cliente (`CustomerID`). El objetivo es examinar la calidad de los datos, procesar la información y obtener resultados útiles para comprender la información de clientes y las operaciones de venta.

## Objetivos

- Leer y procesar archivos CSV con Python.
- Explorar la estructura y el contenido de los datos.
- Identificar y gestionar inconsistencias en los registros.
- Analizar la información de los clientes, incluyendo sus identificadores, nombres y ubicaciones.
- Procesar pedidos, productos, fechas y valores monetarios.
- Relacionar los pedidos con los clientes mediante `CustomerID`.
- Obtener estadísticas y resultados que permitan interpretar los datos desde una perspectiva de negocio.

## Dataset

El proyecto utiliza dos archivos:

### 1. Clientes (`customers.csv`)

Contiene información de los clientes.

| Columna | Descripción |
|---|---|
| `CustomerID` | Identificador del cliente. |
| `FirstName` | Nombre. |
| `LastName` | Apellido. |
| `City` | Ciudad. |
| `State` | Estado o región. |

### 2. Pedidos (`orders.csv`)

Contiene información de los pedidos y sus productos.

| Columna | Descripción |
|---|---|
| `CustomerID` | Identificador del cliente asociado al pedido. |
| `OrderID` | Identificador del pedido. |
| `Date` | Fecha y hora del registro. |
| `OrderTotal` | Importe total asociado al pedido. |
| `ProductName` | Nombre o código del producto. |
| `Price` | Precio registrado para el producto. |

Los archivos originales se descargan desde el repositorio público de [ITU](https://github.com/fpellerano/itu). También se encuentran disponible en la carpeta data de este repositorio.

## Tecnologías utilizadas

- **Python:** procesamiento de datos y lógica de análisis.
- **CSV:** formato de almacenamiento de los datos.
- **Google Colab:** entorno de desarrollo y ejecución del notebook.

## Metodología

1. Descarga y carga de los archivos CSV.
2. Inspección inicial de los datos.
3. Procesamiento de los registros de clientes.
4. Procesamiento de los registros de pedidos.
5. Revisión de posibles duplicados e inconsistencias.
6. Análisis de los resultados obtenidos en ambos conjuntos de datos.

## Resultados del análisis

### Clientes

| Indicador | Resultado |
|---|---|
| Cantidad de clientes | 602 |
| Estados diferentes | 14 |
| El estado con más clientes | CA |
| Los estados con menos clientes | WA, NH, ID, OR, MA, IN |
| Apellido más común | SMITH con 8 repeticiones |

### Pedidos

| Indicador | Resultado |
|---|---|
| Cantidad de pedidos únicos | 16672 |
| Promedio de artículos por pedido | 1.76 |
| Pedido con más artículos | pedido 5802666 |
| Mayor cantidad de artículos de un pedido | 35 |
| Cantidad de pedidos realizados en octubre 2021 | 267 |
| Cliente que gasto más en 2021 | cliente 5464 |
| Mayor gasto registrado en 2021 | 56170.0 |
| Mejor mes para las ventas | Enero |
| Cantidad de ventas del mejor mes | 858727.0 |

## Cómo ejecutar el proyecto

1. Abrir el notebook en Google Colab.
2. Ejecutar las celdas en orden.
3. Verificar que los archivos CSV se descarguen correctamente.
4. Consultar las tablas, estadísticas y resultados generados.

El notebook descarga los archivos desde su fuente pública y los guarda en la carpeta `sample_data` de la sesión de Colab.

## Estado del proyecto

Proyecto práctico de procesamiento de datos orientado a la exploración, limpieza y análisis de información de clientes y pedidos.
