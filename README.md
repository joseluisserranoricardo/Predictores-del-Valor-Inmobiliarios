# 📊 Análisis de Correlación y Regresión: Predictores del Valor Inmobiliario

## 📝 Descripción
Este proyecto se enfoca en el análisis estadístico avanzado para identificar las variables que tienen un impacto directo en el precio de venta de las viviendas. Se aplicaron técnicas de correlación de Pearson y modelos de regresión polinómica para validar hipótesis de mercado.

---

## 📈 1. Matriz de Correlación
Se generó una matriz para cuantificar la fuerza de la relación entre el precio (`SalePrice`) y las características clave.
![matriz correlacion](https://github.com/user-attachments/assets/88d115ed-a47d-43e5-8d33-1d1424c0df18)

### Hallazgos Principales:
* **Calidad General (`OverallQual`):** Correlación de **0.79**. Es el predictor más fuerte; la percepción de lujo y materiales domina el precio.
* **Superficie Habitable (`GrLivArea`):** Correlación de **0.71**. Una relación lineal sólida: a más metros cuadrados, mayor precio.
* **Antigüedad (`YearBuilt`):** Correlación de **0.52**. Existe una relación moderada, indicando que el mercado valora las construcciones más recientes.



---

## 📉 2. Modelo de Regresión (Antigüedad vs. Precio)
Para entender cómo la edad de una propiedad afecta su valor, se desarrolló un gráfico de dispersión comparando `YearBuilt` contra `SalePrice`.

![grafico dispersion](https://github.com/user-attachments/assets/2ebe9b08-05ba-4401-a69f-e8fdaf2eb23b)

### Detalles del Modelo:
* **Tipo de Ajuste:** Polinómico de 2do Grado.
* **Coeficiente de Determinación ($R^2$):** **0.35**.
* **Análisis:** El modelo explica el 35% de la variabilidad del precio basándose solo en el año. Se optó por un ajuste polinómico para capturar mejor el comportamiento de los **outliers** (valores atípicos), reconociendo que las casas históricas y las ultra-modernas rompen la tendencia lineal simple.



---

## 🛠️ Metodología Técnica
1. **Extracción de Datos:** Se transformaron los datos del modelo relacional de Power Pivot a una tabla plana para análisis estadístico.
2. **Tratamiento de Datos Atípicos:** Se identificaron y analizaron outliers que distorsionaban la línea de tendencia inicial.
3. **Herramientas de Análisis:** Uso del complemento "Análisis de Datos" de Excel para la generación de coeficientes estadísticos de alta precisión.

---

## 💡 Conclusión del Analista
El precio de una vivienda es un fenómeno multivariante. Mientras que el **año de construcción** es un factor base importante ($R^2=0.35$), la **calidad de los acabados** y el **área habitable** son los verdaderos motores que impulsan el valor hacia los rangos superiores. Este análisis permite a un inversionista priorizar remodelaciones (calidad) sobre la simple antigüedad del activo.

---

