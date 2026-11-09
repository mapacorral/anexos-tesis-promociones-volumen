# Anexos del trabajo de grado: promociones por volumen e inventarios con demanda estocástica

Este repositorio tiene los anexos del trabajo de grado **«Análisis de las promociones por volumen sobre los costos en sistemas de inventario con demanda estocástica»**. Lo presentó María Paula Corral Ramírez para optar por el título de Ingeniera Industrial en la Universidad de los Andes (Facultad de Ingeniería, Departamento de Ingeniería Industrial, Bogotá, 2026).

- **Asesor:** Ciro Alberto Amaya Guio
- **Co-asesor:** Luis Enrique Tarazona Torres

El trabajo aplica tres modelos de inventario al caso de Buden.co: la cantidad económica de pedido (EOQ), la revisión continua (Q,R) y la revisión periódica (S,T). Cada modelo se resuelve sin descuentos y con descuentos por cantidad en todas las unidades. Después, un diseño factorial 2^10 mide qué factores cambian el ahorro que dan los descuentos.

## Contenido

| Anexo | Contenido | Carpeta |
|---|---|---|
| B | Formato de información en Excel con los datos del caso | [`anexo-B-datos`](anexo-B-datos) |
| C | Código del modelo de inventarios (`modelos_inventario.ipynb`) y su guía (`Guia_del_codigo.pdf`) | [`anexos-C-D-codigo`](anexos-C-D-codigo) |
| D | Código del análisis de sensibilidad (`analisis_sensibilidad.ipynb`) | [`anexos-C-D-codigo`](anexos-C-D-codigo) |

## Cómo correr el código

1. Instale Python 3 (el trabajo usó Python 3.13 con Anaconda) y las librerías:

   ```
   pip install -r requirements.txt
   ```

2. Abra `anexos-C-D-codigo/modelos_inventario.ipynb` y corra todas las celdas. El notebook resuelve las seis políticas del caso y genera las gráficas del Capítulo 3 en la carpeta `graficas/`.
3. Abra `anexos-C-D-codigo/analisis_sensibilidad.ipynb` y corra todas las celdas. Este notebook ejecuta primero `modelos_inventario.ipynb` con `%run` (tarda cerca de un minuto) para usar sus funciones y los datos del caso. Por eso los dos archivos deben estar en la misma carpeta.

## Datos

Buden.co (Eventos y Catering de Colombia SAS) suministró los datos para uso académico. En el Excel se omite el nombre del proveedor.
