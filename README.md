# 📞 Identificación de Operadores Ineficaces - CallMeMaybe

### 📊 Descripción del Proyecto
Este proyecto final de formación como **Data Analyst** se centra en ayudar al servicio de telefonía virtual *CallMeMaybe* a optimizar su servicio al cliente. El objetivo principal es identificar a los operadores con un desempeño inferior basándose en métricas de productividad y calidad de atención.

### 🎯 Objetivos
* Definir criterios técnicos y KPIs para la "ineficiencia" operativa.
* Identificar operadores con alta tasa de llamadas perdidas y tiempos de espera excesivos.
* Validar estadísticamente las diferencias entre operadores eficientes e ineficientes.

### 🛠️ Herramientas y Librerías Utilizadas
* **Python:** Lenguaje principal de análisis.
* **Pandas & NumPy:** Limpieza y manipulación de grandes volúmenes de datos.
* **Matplotlib & Seaborn:** Visualización de distribuciones y patrones de comportamiento.
* **SciPy:** Implementación de pruebas estadísticas no paramétricas.

### 🧪 Metodología y Pruebas Estadísticas

1. Generar la lista de operadores ineficaces:
* Aplicar filtros para etiquetar a cada operador según los umbrales investigados
* Crear una tabla con los IDs de los operadores ineficaces y su razón (tasa alta de llamadas perdidas, espera prolongada, número reducido de llamadas salientes)

2. Comparar los operadores eficaces e ineficaces para demostrar estadísticamente que hay diferencias:
* Proporción de llamadas perdidas: **Z-Test** porque trabajamos con proporciones de eventos
* Tiempo de espera promedio: **Prueba Mann-Whitney U** Dado que los datos presentaban una distribución sesgada y presencia de valores atípicos (*outliers*)
* Llamadas salientes: **T‑Test** para comparar medias de llamadas salientes, **Mann‑Whitney** como respaldo por la distribución es sesgada.

### 📈 Conclusiones Clave
* Se segmentó con éxito a los operadores bajo tres criterios: alta tasa de abandono, espera prolongada y baja actividad saliente.
* Los resultados permiten a la gerencia de *CallMeMaybe* realizar intervenciones dirigidas y programas de capacitación específicos para mejorar la satisfación al cliente.

---
## 📂 Estructura del Repositorio
* `notebook.ipynb`: Jupyter Notebook con el código completo, limpieza de datos y análisis.
* `datasets`: Carpeta con los datasets utilizados (*telecom_clients.csv*, *telecom_dataset_us.csv*).
* `Proyecto-Final-Telecomunicaciones.pdf`: Presentación ejecutiva con los hallazgos.
---
