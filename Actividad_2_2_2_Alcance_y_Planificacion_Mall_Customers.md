# Actividad 2.2.2 — Definición de Alcance y Planificación de un Proyecto de Ciencia de Datos

**Asignatura:** SCY1102 — Gestión de Proyectos de Datos  
**Proyecto:** Mall Customer Segmentation  
**Caso:** Retail — Segmentación de Clientes en un Centro Comercial  

**Integrantes:**  
Cristian Romero · Javier Sagredo · Nicolas Osses · Rolando Paredes

---

## Descripción del proyecto

Un centro comercial busca comprender mejor el comportamiento de sus clientes para identificar distintos patrones de consumo.

Para ello, se utilizará el dataset **Mall Customers**, que contiene información relacionada con características de los clientes, como edad, género, ingreso anual y nivel de gasto.

El proyecto propone utilizar el algoritmo de clustering **K-Means**, principalmente sobre las variables **Annual Income** y **Spending Score**, con el objetivo de descubrir agrupaciones naturales de clientes.

Los segmentos obtenidos podrán ser utilizados como apoyo para que el área de Marketing comprenda mejor los distintos perfiles de clientes y pueda diseñar estrategias comerciales más específicas.

---

# Parte 1 — Definición del alcance

## Objetivo del proyecto

Desarrollar un modelo de segmentación de clientes mediante **K-Means**, utilizando principalmente el ingreso anual y el Spending Score, con el fin de identificar grupos de clientes con comportamientos similares y generar información útil para la toma de decisiones del área de Marketing.

---

## Entregables

### 1. Dataset preparado y documentado

Se entregará una versión del dataset revisada y preparada para el análisis.

Las principales actividades serán:

- Revisión de la estructura del dataset.
- Identificación de valores faltantes o inconsistentes.
- Análisis de calidad de los datos.
- Selección de las variables relevantes.
- Preparación de las variables para el algoritmo K-Means.
- Documentación de las transformaciones realizadas.

---

### 2. Modelo de segmentación validado

Se desarrollará un modelo de clustering utilizando el algoritmo **K-Means**.

El modelo deberá incluir:

- Selección de las variables de entrada.
- Prueba de distintos valores de `K`.
- Aplicación del método del codo.
- Evaluación mediante **Silhouette Score**.
- Selección del número de clústeres más adecuado.
- Asignación de cada cliente a un segmento.

El resultado esperado es obtener aproximadamente **cinco segmentos de clientes**, siempre que las métricas de evaluación respalden esta cantidad.

---

### 3. Informe o dashboard de segmentos

Se elaborará una visualización de los segmentos obtenidos que permita comprender las principales características de cada grupo.

El informe incluirá:

- Cantidad de clientes por segmento.
- Ingreso anual promedio.
- Spending Score promedio.
- Representación gráfica de los clústeres.
- Descripción general de cada segmento.
- Interpretación de los resultados desde una perspectiva de negocio.

---

## Elementos fuera de alcance

Para mantener el proyecto dentro de un alcance realista, se establecen los siguientes elementos como fuera de alcance:

### 1. Implementación productiva en tiempo real

El modelo no será desplegado como un sistema que clasifique automáticamente clientes en tiempo real.

El proyecto se limitará al análisis de datos, desarrollo del modelo y presentación de resultados.

### 2. Integración automática con sistemas externos

No se realizará una integración directa con sistemas como:

- CRM.
- Sistemas de ventas.
- Sistemas de fidelización.
- Plataformas publicitarias.

La integración con estos sistemas podría desarrollarse posteriormente en una etapa productiva.

### 3. Automatización completa de campañas

El proyecto no enviará campañas automáticamente según el segmento asignado a cada cliente.

Los resultados serán utilizados únicamente como apoyo para la toma de decisiones del equipo de Marketing.

### 4. Soporte y mantenimiento posterior

El proyecto no contempla mantenimiento permanente, actualización continua del modelo ni soporte técnico después de la entrega académica.

---

## Supuestos

### Supuesto 1 — Disponibilidad de los datos

Se asume que el dataset estará disponible durante todo el proyecto y contendrá información suficiente para realizar el análisis y la segmentación.

### Supuesto 2 — Participación de stakeholders

Se asume que los stakeholders relevantes, especialmente el área de Marketing, estarán disponibles para validar la utilidad e interpretación de los segmentos obtenidos.

### Supuesto 3 — Representatividad del Spending Score

Se considera que el **Spending Score** disponible en el dataset representa de manera razonable el comportamiento de compra de cada cliente.

Esta variable será utilizada como uno de los principales indicadores para construir los segmentos.

---

## Restricciones

### Restricción 1 — Tiempo

El proyecto deberá completarse dentro del plazo académico definido para la asignatura.

Esto limita la posibilidad de implementar funcionalidades productivas o integraciones adicionales.

### Restricción 2 — Datos disponibles

El análisis estará limitado a las variables disponibles en el dataset.

No se incorporarán nuevas fuentes de información externas durante esta etapa del proyecto.

### Restricción 3 — Privacidad de los datos

Los datos utilizados deberán mantenerse anonimizados y utilizarse únicamente para los objetivos definidos en el proyecto.

Además, se evitará utilizar características sensibles como criterio directo para generar decisiones automáticas sobre los clientes.

### Restricción 4 — Recursos tecnológicos

El proyecto será desarrollado utilizando herramientas disponibles para el equipo, principalmente:

- Python.
- Jupyter Notebook o Google Colab.
- Pandas.
- Scikit-learn.
- Matplotlib.
- Jira o Trello para planificación.
- Canva o Miro para documentación visual.

---

# Parte 2 — Planificación del proyecto

Para organizar el desarrollo del proyecto se utilizará el marco de trabajo **CRISP-DM**.

CRISP-DM divide un proyecto de ciencia de datos en seis fases:

1. Comprensión del negocio.
2. Comprensión de los datos.
3. Preparación de los datos.
4. Modelado.
5. Evaluación.
6. Despliegue.

El proceso es iterativo, por lo que es posible regresar a fases anteriores cuando los resultados obtenidos indiquen que se requieren ajustes.

---

## 1. Comprensión del negocio

### Objetivo

Comprender el problema que desea resolver el centro comercial y establecer los objetivos del proyecto.

### Tareas

- Analizar el problema planteado por el cliente.
- Identificar los stakeholders.
- Revisar los requerimientos funcionales y no funcionales.
- Establecer los objetivos de la segmentación.
- Definir el alcance del proyecto.
- Identificar supuestos y restricciones.
- Definir qué resultados deberían generar valor para Marketing.

### Responsable principal

**Cristian**

### Tiempo estimado

**3 horas**

---

## 2. Comprensión de los datos

### Objetivo

Analizar las características del dataset antes de comenzar el modelado.

### Tareas

- Cargar el dataset.
- Revisar cantidad de registros y columnas.
- Analizar los tipos de datos.
- Generar estadísticas descriptivas.
- Identificar valores faltantes.
- Detectar posibles valores atípicos.
- Analizar las distribuciones de las variables.
- Estudiar las relaciones entre ingreso anual y Spending Score.

### Responsable principal

**Javier**

### Tiempo estimado

**4 horas**

---

## 3. Preparación de los datos

### Objetivo

Preparar los datos para que puedan ser utilizados correctamente por el algoritmo K-Means.

### Tareas

- Tratar valores faltantes si existen.
- Revisar registros duplicados.
- Seleccionar las variables relevantes.
- Preparar `Annual Income`.
- Preparar `Spending Score`.
- Evaluar la necesidad de escalamiento.
- Construir el dataset final de modelado.
- Documentar las transformaciones realizadas.

Las variables como género u otras características demográficas podrán analizarse posteriormente para comprender los segmentos, pero no serán utilizadas directamente como variables de entrada principales del modelo.

### Responsable principal

**Nicolas**

### Tiempo estimado

**4 horas**

---

## 4. Modelado

### Objetivo

Construir el modelo de clustering utilizando K-Means.

### Tareas

- Ejecutar K-Means con distintos valores de `K`.
- Calcular la inercia de cada modelo.
- Aplicar el método del codo.
- Calcular el Silhouette Score.
- Comparar diferentes configuraciones.
- Seleccionar la cantidad adecuada de clústeres.
- Entrenar el modelo final.
- Asignar cada cliente a un segmento.
- Generar una representación gráfica de los clústeres.

### Responsable principal

**Rolando**

### Tiempo estimado

**5 horas**

---

## 5. Evaluación

### Objetivo

Determinar si los segmentos obtenidos son técnicamente adecuados y útiles desde una perspectiva de negocio.

### Tareas

- Revisar el método del codo.
- Analizar el Silhouette Score.
- Comparar la separación entre los clústeres.
- Analizar el tamaño de cada segmento.
- Calcular ingreso promedio por segmento.
- Calcular Spending Score promedio por segmento.
- Interpretar las características de cada grupo.
- Validar si los segmentos pueden ser comprendidos por Marketing.
- Revisar posibles concentraciones demográficas que puedan generar sesgos.

Si los resultados no son satisfactorios, se podrá regresar a las etapas de preparación de datos o modelado.

### Responsables principales

**Cristian y Javier**

### Tiempo estimado

**4 horas**

---

## 6. Despliegue

### Objetivo

Preparar los resultados del proyecto para que puedan ser comprendidos y utilizados por los stakeholders.

En este proyecto, despliegue no significa implementar el modelo en un sistema productivo, sino preparar y comunicar los resultados obtenidos.

### Tareas

- Crear gráficos de los segmentos.
- Preparar las métricas principales.
- Describir cada segmento.
- Generar el informe final.
- Documentar el modelo.
- Registrar conclusiones y recomendaciones.
- Preparar los resultados para ser entregados al cliente.

### Responsables

**Todo el equipo**

### Tiempo estimado

**4 horas**

---

## Resumen de planificación

| Fase CRISP-DM | Responsable principal | Tiempo estimado |
|---|---|---:|
| Comprensión del negocio | Cristian | 3 h |
| Comprensión de los datos | Javier | 4 h |
| Preparación de los datos | Nicolas | 4 h |
| Modelado | Rolando | 5 h |
| Evaluación | Cristian y Javier | 4 h |
| Despliegue | Todo el equipo | 4 h |
| **Total** | **Equipo** | **24 h** |

---

# Reflexión grupal

Una definición clara del alcance permite establecer desde el comienzo qué entregará el proyecto y qué elementos quedarán fuera. Esto evita generar expectativas poco realistas y reduce la posibilidad de realizar trabajo que no contribuya directamente al objetivo definido.

Además, definir el alcance permite identificar anticipadamente los supuestos y restricciones que podrían afectar la viabilidad del proyecto. En nuestro caso, factores como el tiempo disponible, las variables presentes en el dataset, la calidad de los datos y los recursos tecnológicos determinan qué tan lejos puede llegar la solución dentro del contexto académico.

La planificación mediante **CRISP-DM** permite organizar el proyecto de ciencia de datos en fases claramente definidas y mantener una conexión constante entre las necesidades del negocio y las actividades técnicas.

Su estructura también permite controlar mejor los riesgos, ya que el proceso es iterativo. Por ejemplo, si durante la evaluación se descubre que los clústeres obtenidos no tienen una separación adecuada o no generan información útil para Marketing, es posible regresar a la preparación de los datos o al modelado y realizar ajustes.

En nuestro proyecto, esta planificación evita que el trabajo se limite simplemente a ejecutar un algoritmo K-Means. El objetivo real es obtener segmentos que puedan ser interpretados y utilizados para apoyar decisiones de Marketing, manteniendo al mismo tiempo control sobre la calidad de los datos, la privacidad y los posibles sesgos.

Por lo tanto, una correcta definición del alcance y el uso de un marco de trabajo como CRISP-DM aumentan la **viabilidad del proyecto**, permiten un mejor **control de los riesgos** y ayudan a que el resultado final genere **valor real para el cliente**.
