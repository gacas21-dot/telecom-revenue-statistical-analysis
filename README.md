# Análisis Estadístico de Rentabilidad: Planes Surf vs. Ultimate (Megaline) 📊

## 📄 Descripción del Proyecto
Este proyecto se enfoca en el análisis de rentabilidad y comportamiento del consumidor para **Megaline**, un operador de telecomunicaciones. El desafío principal fue determinar cuál de las dos tarifas prepago genera mayores ingresos, permitiendo al departamento comercial optimizar la asignación del presupuesto publicitario basado en evidencia de datos reales.

A través del análisis de consumo de **500 clientes** (llamadas, SMS y datos), apliqué técnicas de **estadística inferencial** para validar si las diferencias observadas en los ingresos eran estadísticamente significativas o simplemente resultado del azar.

## 🛠️ Habilidades Técnicas Aplicadas
* **ETL y Consolidación de Datos:** Procesé y uní 4 fuentes de datos independientes para generar un perfil de consumo mensual detallado por usuario.
* **Ingeniería de Características:** Calculé métricas de exceso de consumo por servicio (GB, minutos, mensajes) y los ingresos mensuales finales aplicando la lógica de negocio de cada plan.
* **Análisis de Distribución:** Utilicé histogramas y diagramas de caja (**boxplots**) para identificar sesgos en el consumo y gestionar valores atípicos (outliers).
* **Pruebas de Hipótesis (SciPy):**
    * Ejecuté pruebas **t-student** para comparar ingresos promedio entre planes.
    * Evalué diferencias regionales (Área de NY-NJ vs. Otras regiones) para segmentación de mercado.



## 💡 Conclusiones Estratégicas
* **Plan Surf como motor de ingresos variables:** Aunque su tarifa base es menor ($20), el exceso de consumo (especialmente en el paquete de datos) genera ingresos adicionales que superan con frecuencia la rentabilidad fija del plan Ultimate.
* **Estabilidad del Plan Ultimate:** Proporciona ingresos constantes y predecibles ($70), pero con una tasa de "upselling" casi nula, ya que los usuarios rara vez exceden sus límites incluidos.
* **Segmentación Geográfica:** Las pruebas estadísticas confirmaron que no hay diferencias significativas en el gasto de la región NY-NJ respecto al resto del país ($p > 0.05$), validando una estrategia de marketing nacional unificada en lugar de campañas locales costosas.



## 📂 Estructura del Repositorio
* `proyecto sprint 5.ipynb`: Pipeline completo desde la limpieza de datos hasta la validación estadística.
* `Datasets/`: Carpeta con los archivos CSV de llamadas, mensajes, planes y usuarios.
* `requirements.txt`: Dependencias del proyecto (Pandas, SciPy, Matplotlib, Seaborn).

---
**Nota:** Este proyecto forma parte de mi portafolio como Ingeniera Industrial y Analista de Datos, enfocado en el uso de la estadística para la toma de decisiones corporativas.
