# telecom-revenue-statistical-analysis
## 📄 **Descripción del Proyecto**
Este proyecto se enfoca en el análisis de rentabilidad y comportamiento del consumidor para Megaline, un operador de telecomunicaciones. El desafío principal fue determinar cuál de las dos tarifas prepago (Surf y Ultimate) genera mayores ingresos, permitiendo al departamento comercial optimizar su presupuesto publicitario.

A través del análisis de consumo de 500 clientes (llamadas, SMS y datos), apliqué técnicas de estadística inferencial para validar si las diferencias observadas en los ingresos eran resultado de patrones reales o del azar.

## 🛠️ **Lo que hice (Habilidades Técnicas)**
ETL y Consolidación de Datos: Procesé y uní 4 fuentes de datos independientes para generar un perfil de consumo mensual detallado por usuario.

Ingeniería de Características: Calculé métricas clave como el exceso de consumo por servicio (GB, minutos, mensajes) y los ingresos mensuales finales aplicando las reglas de cada plan.

Análisis de Distribución: Utilicé histogramas y diagramas de caja (boxplots) para entender la dispersión y sesgo en el uso de datos e identificar valores atípicos.

Pruebas de Hipótesis (SciPy):

Ejecuté pruebas t-student para comparar los ingresos promedio entre ambos planes.

Evalué la diferencia de ingresos entre usuarios de la región NY-NJ frente al resto de las ciudades para segmentar el mercado.

## 💡**Conclusiones Estratégicas**
Plan Surf como motor de ingresos variables: Aunque el plan Surf tiene una tarifa base menor, los usuarios tienden a exceder sus límites con frecuencia, generando ingresos adicionales significativos por GB extra.

Estabilidad del Plan Ultimate: Los usuarios de Ultimate casi nunca exceden sus límites, lo que proporciona ingresos constantes y predecibles, pero con menor "upselling".

Segmentación Geográfica: Se demostró que no existe una diferencia significativa de consumo en la zona de Nueva York-Nueva Jersey, lo que sugiere que las campañas nacionales pueden ser igual de efectivas que las locales.

## 📂 **Estructura del repositorio**
proyecto sprint 5.ipynb: Análisis completo, desde la limpieza hasta la validación de hipótesis.

Datasets/: Datos de llamadas, mensajes, planes y usuarios (archivos CSV).

requirements.txt: Librerías necesarias para replicar el análisis.

