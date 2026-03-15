# AI Technical Room Builder
### Generador Inteligente de Presupuestos para Salas Técnicas de Infraestructura

**Autor:** Diego A. Godoy  
**Curso:** Inteligencia Artificial – Generación de Prompts - Comisión: N° 86420 
**Repositorio Drive:** https://drive.google.com/drive/folders/1FYNcTPh0Cvxc8RIB5anVgdl6v9RZXKw0?usp=sharing
**Proyecto Final**

---

# 📌 Resumen

En proyectos de infraestructura técnica, como la construcción de salas de energía, salas de racks, salas para grupos electrógenos o plateas de hormigón para equipamiento industrial, es fundamental realizar una correcta planificación previa de la obra civil.

Sin embargo, muchas veces resulta complejo estimar rápidamente los materiales necesarios, las etapas de construcción y el costo aproximado del proyecto, especialmente en las primeras fases de planificación o ante consultas preliminares.

AI Technical Room Builder es una Prueba de Concepto (POC) que utiliza inteligencia artificial generativa para asistir en la planificación inicial de este tipo de proyectos. A partir de una descripción textual del proyecto, el sistema genera automáticamente una estimación de materiales de obra civil, una guía básica de construcción, un rango aproximado de presupuesto y un prompt optimizado para generar una visualización del proyecto mediante herramientas de generación de imágenes.

---

# 📖 Introducción

## Nombre del proyecto

AI Technical Room Builder: Generador Inteligente de Presupuestos y Pliegos para Salas Técnicas de Infraestructura

---

## Presentación del problema a abordar

En proyectos de infraestructura tecnológica y energética, es común la necesidad de construir espacios técnicos específicos como:

- salas de energía
- salas de racks o telecomunicaciones
- salas para grupos electrógenos
- plateas de hormigón para grupos electrógenos
- pequeñas salas técnicas de soporte

Estos espacios requieren una planificación adecuada de la obra civil, incluyendo fundaciones, estructuras, cerramientos, ventilación y distribución del equipamiento técnico.

En las primeras etapas de un proyecto, muchas veces es necesario realizar estimaciones rápidas de:

- materiales de construcción
- dimensiones aproximadas
- etapas de obra
- costos preliminares

Sin embargo, esta información no siempre está disponible de forma inmediata, lo que puede generar dificultades en la planificación inicial o en la elaboración de presupuestos preliminares.

La inteligencia artificial generativa permite abordar esta problemática generando recomendaciones técnicas iniciales y estimaciones preliminares a partir de una simple descripción del proyecto.

---

## Desarrollo de la propuesta de solución

La solución propuesta consiste en desarrollar una Prueba de Concepto (POC) mediante una Jupyter Notebook que utilice modelos de inteligencia artificial generativa para analizar la descripción de una sala técnica o infraestructura energética.

El sistema utilizará dos tipos de modelos de inteligencia artificial:

### Modelo texto-texto

El modelo de lenguaje generará información técnica estructurada relacionada con el proyecto, incluyendo:

- lista estimada de materiales de obra civil
- etapas principales de construcción
- recomendaciones de infraestructura
- estimación aproximada de presupuesto

### Modelo texto-imagen

A partir del análisis del proyecto, el sistema generará un prompt optimizado que podrá utilizarse en herramientas externas de generación de imágenes para visualizar conceptualmente la sala técnica o la infraestructura propuesta.

De esta forma, se podrá obtener una representación visual preliminar del proyecto antes de su construcción.

---

## Justificación de la viabilidad del proyecto

El proyecto resulta viable por diversas razones.

**Viabilidad técnica**

Los modelos actuales de inteligencia artificial poseen suficiente conocimiento general sobre construcción, infraestructura técnica y equipamiento energético, lo que permite generar recomendaciones preliminares coherentes sin necesidad de entrenamiento adicional.

**Recursos disponibles**

El proyecto utiliza herramientas tecnológicas accesibles como:

- Python
- Jupyter Notebook
- modelos de inteligencia artificial generativa
- herramientas externas de generación de imágenes

Esto permite desarrollar la prueba de concepto sin requerir infraestructura compleja.

**Tiempo de desarrollo**

El alcance del proyecto se centra en el diseño de prompts y el análisis de respuestas generadas por la IA, lo que permite implementar y evaluar la solución dentro del tiempo disponible del curso.

---

# 🎯 Objetivos

## Objetivo general

Desarrollar una prueba de concepto que demuestre cómo la inteligencia artificial generativa puede asistir en la planificación preliminar de infraestructura técnica mediante el uso de técnicas de Fast Prompting.

---

## Objetivos específicos

- Diseñar prompts optimizados para interpretar descripciones de salas técnicas e infraestructura energética.
- Utilizar modelos de IA para generar estimaciones preliminares de materiales y etapas de construcción.
- Generar automáticamente prompts para visualización mediante modelos texto-imagen.
- Aplicar técnicas de Fast Prompting para mejorar la calidad de las respuestas generadas.
- Evaluar los resultados obtenidos a partir de distintos prompts.

---

# ⚙️ Metodología

El proyecto se desarrollará mediante una metodología experimental basada en el diseño y evaluación de prompts.

El proceso se divide en las siguientes etapas:

1. Identificación de la problemática relacionada con la planificación de infraestructura técnica.

2. Diseño de prompts que permitan a la inteligencia artificial interpretar la descripción del proyecto.

3. Aplicación de técnicas de Fast Prompting para mejorar la calidad de las respuestas.

4. Implementación de los prompts en una Jupyter Notebook utilizando Python.

5. Generación de resultados estructurados que incluyan recomendaciones técnicas y prompts para generación de imágenes.

6. Evaluación de los resultados obtenidos.

Esta metodología permite analizar cómo el diseño de prompts influye en la calidad de las respuestas generadas por los modelos de inteligencia artificial.

---

# 🛠️ Herramientas y tecnologías

El proyecto utiliza las siguientes herramientas y tecnologías.

**Lenguaje de programación**

Python

**Entorno de desarrollo**

Jupyter Notebook / Google Colab

**Modelo de inteligencia artificial**

Modelos generativos de lenguaje (LLM)

---

## Técnicas de Fast Prompting utilizadas

### Role Prompting

Se asigna al modelo el rol de un profesional especializado en infraestructura técnica para generar respuestas más precisas.

Como por ejemplo:

"Actúa como un ingeniero civil especializado en construcción de salas técnicas, centros de energía e infraestructura para datacenters."

---

### Structured Output Prompting

El modelo devuelve la información en formato JSON estructurado, lo que permite que el código procese fácilmente los datos generados.

---

### Zero-Shot Prompting

Se generan respuestas a partir de una instrucción directa sin ejemplos previos.

---

# 💻 Implementación

La implementación se desarrolla en una Jupyter Notebook utilizando Python.

El sistema recibe como entrada una descripción del proyecto de infraestructura técnica que el usuario desea realizar.

Ejemplo de entrada:

"Construir una sala de energía de 6x4 metros para alojar UPS y tableros eléctricos."

o

"Construir una platea de hormigón para un grupo electrógeno de 800 kVA."

A partir de esta información, el modelo genera un objeto estructurado que contiene:

- lista estimada de materiales de obra civil
- etapas básicas de construcción
- estimación de presupuesto aproximado
- prompt optimizado para generación de imagen

El prompt generado puede utilizarse posteriormente en herramientas de generación de imágenes como NightCafe o Leonardo AI para visualizar conceptualmente la infraestructura.

---

# 📊 Resultados

Los resultados obtenidos muestran que la inteligencia artificial puede generar recomendaciones preliminares coherentes a partir de descripciones simples de proyectos de infraestructura técnica.

La implementación permite obtener rápidamente:

- una guía inicial de materiales
- etapas básicas de construcción
- estimaciones preliminares de costos
- prompts optimizados para visualización de la infraestructura

Esto facilita la planificación inicial de proyectos de salas técnicas o infraestructura energética.

---

# 🏁 Conclusiones

A lo largo del desarrollo de este proyecto se demostró el potencial de la inteligencia artificial generativa para asistir en la planificación preliminar de infraestructura técnica mediante el uso de prompts diseñados estratégicamente.

La aplicación de técnicas de Fast Prompting permitió orientar el comportamiento del modelo para generar respuestas estructuradas y útiles para el usuario.

Además, la generación automática de prompts para modelos de imagen permite complementar la información técnica con una representación visual conceptual del proyecto.

Los objetivos planteados al inicio del proyecto se lograron satisfactoriamente, demostrando que mediante una adecuada ingeniería de prompts es posible desarrollar herramientas que apoyen procesos de planificación inicial en proyectos de infraestructura técnica.

En el futuro, este tipo de soluciones podría integrarse con sistemas reales de presupuestos de obra, bases de datos de costos de materiales o herramientas de diseño de infraestructura.

---

# 📚 Referencias

- Material del curso **Inteligencia Artificial – Generación de Prompts Comisión: N° 86420 **
- Documentación sobre Prompt Engineering
- Recursos sobre inteligencia artificial generativa aplicada a ingeniería
- Documentación de modelos generativos de lenguaje

---

# 💻 Implementación

El código completo del proyecto se encuentra en la Jupyter Notebook incluido en este repositorio.
