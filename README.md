# 📶 Proyecto de Análisis de Datos: Megaline — ¿Cuál es la mejor tarifa?

## 📖 Introducción

Como analista de datos en **Megaline**, una empresa de telecomunicaciones que ofrece dos planes de prepago —**Surf** y **Ultimate**—, el objetivo de este proyecto es identificar cuál de las tarifas genera **mayores ingresos**.
A partir de una muestra de **500 clientes**, se analizó su comportamiento durante 2018: llamadas realizadas, mensajes enviados y consumo de datos.

El resultado permitirá orientar las **estrategias publicitarias** y optimizar la distribución del presupuesto de marketing.

---

## 🎯 Objetivos del Proyecto

1. **Limpieza de datos:**

   * Unificar unidades de medida y corregir tipos de datos.
   * Asegurar que cada DataFrame contenga información coherente y precisa.

2. **Integración de bases de datos:**

   * Combinar los DataFrames en una sola estructura consolidada para facilitar el análisis.

3. **Análisis descriptivo:**

   * Calcular estadísticas clave (promedios, máximos, distribuciones) para comprender el comportamiento de los usuarios.

4. **Pruebas de hipótesis:**

   * Validar si las diferencias entre los planes son estadísticamente significativas.

---

## 🧮 Metodología

Para calcular los ingresos mensuales por usuario:

* Se restaron los límites del paquete gratuito (llamadas, SMS y GB) del uso total de cada cliente.
* El exceso se multiplicó por la tarifa correspondiente según el plan.
* Se sumó la **tarifa base mensual** (20 USD para Surf, 70 USD para Ultimate).

Los usuarios que no superaron los límites solo generaron ingresos por la tarifa base.
Así se obtuvo el **ingreso total mensual por cliente** y luego el promedio por plan.

---

## 📊 Resultados Principales

### 🔸 Duración de llamadas

Los usuarios de ambos planes tienen comportamientos similares.

* **Surf:** promedio de 354.9 min.
* **Ultimate:** promedio de 358.1 min.
  No hay diferencias significativas en el uso del servicio de llamadas.

### 🔸 Mensajes de texto

* **Surf:** promedio de 22.8 SMS/mes.
* **Ultimate:** promedio de 28.7 SMS/mes.
  Los usuarios de **Ultimate** envían más mensajes en promedio.

### 🔸 Consumo de Internet

* **Surf:** 13.5 GB/mes.
* **Ultimate:** 15.1 GB/mes.
  Ambos grupos consumen cantidades similares, aunque Ultimate ofrece el doble de capacidad mensual.

### 🔸 Ingresos mensuales

* **Surf:** promedio de **48.99 USD**
* **Ultimate:** promedio de **71.86 USD**

Los usuarios de **Surf**, pese a tener un plan más económico, generan mayores ingresos adicionales por excedentes.
En cambio, los de **Ultimate** pagan más tarifa base pero casi no incurren en cargos extra.

---

## 🌍 Análisis por Región

No se encontraron diferencias significativas en los ingresos promedio entre los usuarios de **NY/NJ** y los de otras regiones.
Esto sugiere que la **ubicación geográfica no influye** en el comportamiento de consumo.

---

## 🧠 Conclusiones Generales

* El **plan Ultimate** genera mayores ingresos totales por su tarifa base más alta.
* El **plan Surf** genera más ingresos adicionales gracias al uso extra de servicios.
* El comportamiento general de los usuarios (llamadas, mensajes, datos) es **similar** entre ambos planes.
* El equipo comercial podría **incentivar a los usuarios de Surf a migrar a Ultimate**, aumentando los ingresos globales y promoviendo la fidelización.

En resumen, el proyecto demostró cómo un análisis riguroso de datos puede ofrecer **insights estratégicos** para la toma de decisiones en marketing y gestión comercial.

---

## 🛠️ Tecnologías Utilizadas

* **Python 3.x**
* **pandas**, **NumPy**, **Matplotlib**, **Seaborn**, **SciPy**
* **Jupyter Notebook**

---

## 🚀 Autor

Proyecto desarrollado por **Carlos Ortiz** como parte del módulo de **Análisis de Datos en Telecomunicaciones**.
El análisis fue realizado con datos simulados representativos de los clientes de Megaline durante 2018.
