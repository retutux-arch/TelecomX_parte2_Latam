# Análisis Predictivo de Fuga de Clientes (Churn Prediction) - Telecom X

![Stars](https://img.shields.io/github/stars/retutux-arch/TelecomX_parte2_Latam?style=social)
![License](https://img.shields.io/github/license/retutux-arch/TelecomX_parte2_Latam?color=blue)
![Machine Learning](https://img.shields.io/badge/Focus-Machine%20Learning-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

## 📝 Resumen Ejecutivo
Este proyecto se enfoca en la predicción de la fuga de clientes (**churn**) para la empresa **Telecom X**, con el objetivo de identificar a los usuarios en riesgo y desarrollar estrategias de retención proactivas. 

A través de un análisis exhaustivo, se entrenaron y evaluaron múltiples modelos de Machine Learning utilizando diversas técnicas de balanceo para abordar el desequilibrio de clases.

---

## 🛠️ Metodología

El proyecto se desarrolló siguiendo un pipeline de ciencia de datos estructurado:

### 1. Extracción y Preprocesamiento
* **Limpieza:** Carga de `clientes_telecom_x.csv` y eliminación de `ID_Cliente`.
* **Transformación:** `Genero` a numérico e imputación de nulos en `Cargos_Totales` utilizando la **media**.
* **Codificación:** Aplicación de `OneHotEncoder` a variables categóricas.

### 2. División de Datos
* **Split:** 70% entrenamiento y 30% prueba.
* **Selección de Características:** Uso de `RandomForestClassifier` para extraer las **10 variables más influyentes**.

### 3. Modelado y Evaluación
Estrategias de balanceo evaluadas: Unbalanced, Undersampling, SMOTE y **SMOTEENN** (ganadora).

---

## 📊 Hallazgos Clave

### Rendimiento de Modelos (Estrategia SMOTEENN)

| Modelo | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **RandomForest** | **0.7607** | **0.5325** | 0.7352 | **0.6172** |
| LogisticRegression | 0.7241 | 0.4851 | 0.8093 | 0.6062 |
| LinearSVC | 0.7200 | 0.4807 | **0.8153** | 0.6045 |

### Factores Críticos
* **Riesgo:** Contratos mes a mes, Fibra Óptica y pagos por cheque electrónico.
* **Retención:** **Soporte Técnico**, contratos a 2 años y antigüedad del cliente.

---

## 💡 Estrategias de Retención Propuestas

* **Fidelización:** Migrar contratos "Mes a Mes" a planes anuales con descuentos.
* **Calidad:** Auditar el servicio de Fibra Óptica para reducir puntos de dolor.
* **Pagos:** Incentivar el débito automático sobre el cheque electrónico.
* **Soporte:** Fortalecer el Soporte Técnico como barrera principal contra la fuga.

---

## ✍️ Autoría

Este proyecto fue desarrollado por:

* **Nombre:** [Tu Nombre Completo]
* **LinkedIn:** [https://www.linkedin.com/in/ariel-lobos/](https://www.linkedin.com/in/ariel-lobos/)
* **GitHub:** [https://github.com/retutux-arch](https://github.com/retutux-arch)
* **Email:** [retutux@gmail.com]

---

## 📄 Licencia
Este proyecto está bajo la Licencia [MIT] - mira el archivo [LICENSE.md](LICENSE.md) para detalles.
