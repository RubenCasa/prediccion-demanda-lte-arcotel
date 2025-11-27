#  Predicción de Demanda de Líneas LTE en Ecuador

Este proyecto aplica técnicas de **Analítica Predictiva** para estimar el comportamiento futuro de las líneas activas de tecnología LTE en Ecuador. Utilizamos datos oficiales de la ARCOTEL y modelos de regresión lineal con ingeniería de características (lags) para anticipar la demanda.

<img width="1548" height="933" alt="image" src="https://github.com/user-attachments/assets/97880acc-c464-40bc-88b9-a2227ff2a726" />

https://datosabiertos.gob.ec/dataset/lineas-activas-tecnologia/resource/64386886-e048-4d23-b305-266aa670fe46 

## Descripción del Proyecto

El objetivo principal fue construir un modelo capaz de predecir la cantidad de líneas LTE para el mes siguiente con un margen de error bajo (MAPE < 8%). Esto permite a las operadoras de telecomunicaciones tomar decisiones basadas en datos sobre infraestructura y retención de clientes.

**Metodología utilizada (SEMMA):**
1.  **Sample & Explore:** Carga de datos históricos y visualización de tendencias por operadora.
2.  **Modify:** Creación de variables de rezago (*lag*) para usar el comportamiento del mes anterior como predictor.
3.  **Model:** Entrenamiento de un modelo de Regresión Lineal.
4.  **Assess:** Evaluación de precisión usando el Error Porcentual Absoluto Medio (MAPE).

##  Resultados Clave

* **Precisión del Modelo:** Se logró un **MAPE del 5.95%**, superando la meta inicial del 8%.
* **Desempeño:** El modelo captura exitosamente la tendencia de crecimiento y detecta caídas abruptas en la demanda, lo cual es crítico para la reacción temprana del negocio.

##  Fuente de Datos

Los datos fueron obtenidos del portal de datos abiertos de la **Agencia de Regulación y Control de las Telecomunicaciones (ARCOTEL)**.

* **Dataset:** 1.1.3 - Líneas activas por tecnología.
* **Fecha de corte:** Diciembre 2021.
* **Licencia:** Creative Commons Non-Commercial.
* **Fuente:** ARCOTEL.

##  Aplicación e Impacto (Business Value)

Basado en los resultados, este modelo ofrece valor directo para operadoras como CNT, Claro y Movistar:

1.  **Planificación de Infraestructura:** Permite prever picos de demanda para invertir en ancho de banda y antenas antes de que la red se sature.
2.  **Estrategia de Retención:** Al predecir caídas en las líneas activas (Churn), el equipo de marketing puede activar campañas preventivas para retener usuarios.
3.  **Respaldo Regulatorio:** Al usar datos oficiales, las proyecciones sirven para justificar planes de inversión ante el regulador.

## Tecnologías

* Python 3.12.7
* Pandas (Manipulación de datos)
* Matplotlib (Visualización)
* Scikit-Learn (Modelado y métricas)
---
*Este proyecto fue desarrollado como parte de la asignatura de Analítica de Datos.*
