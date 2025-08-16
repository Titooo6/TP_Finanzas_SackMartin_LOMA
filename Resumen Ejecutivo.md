# Informe Ejecutivo – Loma Negra (LOMA.BA)

## 1. Resumen Ejecutivo

El presente informe evalúa **Loma Negra (LOMA)** integrando análisis de cartera, técnico y fundamental, con el objetivo de formular una recomendación de inversión sólida.

Durante todo el proceso se utilizó el **ADR cotizante en NYSE** para trabajar en dólares, evitando distorsiones por inflación y volatilidad cambiaria del peso argentino. Esto permitió una medición más estable y comparable con empresas internacionales.

En el **análisis de cartera**, se construyeron y evaluaron diferentes combinaciones de activos, aplicando restricciones y buscando el **máximo Ratio de Sharpe**. Se optó por un portafolio **50% Argentina / 50% Internacional**, equilibrando el potencial de crecimiento local con la estabilidad de mercados desarrollados.

En el **análisis técnico**, se optimizaron indicadores de tendencia, momentum y volatilidad (**SMA**, **RSI**, **MACD**, **ADX**, **Bandas de Bollinger**). El *backtesting* mostró que la combinación de señales mejoró la consistencia de las entradas y salidas, reduciendo falsos positivos y controlando *drawdowns*.

En el **análisis fundamental**, LOMA mostró múltiplos de valuación bajos frente a sus comparables globales y fortalezas como liderazgo de mercado e integración vertical. Sin embargo, enfrenta riesgos elevados por la coyuntura macroeconómica argentina, la inflación y la volatilidad cambiaria. El **DCF simplificado** arrojó un precio objetivo superior al actual, respaldando una recomendación de compra, aunque con cautela.

En conjunto, los tres enfoques sugieren que **LOMA ofrece potencial de apreciación significativo**, condicionado a mejoras en el entorno económico y estabilidad regulatoria. La **diversificación internacional** sigue siendo clave para mitigar riesgos país.

---

## 2. Metodología Utilizada

El análisis se desarrolló en tres ejes complementarios: **cartera**, **técnico** y **fundamental**, integrando datos históricos y métricas financieras para sustentar la recomendación de inversión.

### Selección de activos
- Loma Negra como activo principal y cuatro comparables internacionales (**CRH, CX, VMC, Pampa Energía**) más los índices **MERVAL USD** y **S&P 500**.
- Para las empresas argentinas e índice local se utilizó la **cotización en dólares** (ADR o índice en USD), evitando distorsiones por inflación y volatilidad cambiaria.

### Obtención y tratamiento de datos
- Precios diarios desde el **1/07/2020** descargados de **Yahoo Finance** mediante código en Python.
- Limpieza del dataset: eliminación de valores faltantes, unificación de fechas y ajuste por dividendos/splits.

### Análisis de cartera
- Cálculo de retornos, volatilidades y correlaciones.
- Construcción de la **frontera eficiente** bajo distintas restricciones.
- Evaluación de métricas como el **Ratio de Sharpe**.

### Análisis técnico
- Optimización y combinación de indicadores (**SMA, RSI, MACD, ADX, Bollinger**).
- *Backtesting* para evaluar rendimiento ajustado por riesgo y control de *drawdowns*.

### Análisis fundamental
- Elaboración de **FODA** y comparación sectorial de múltiplos.
- **DCF simplificado** con análisis de sensibilidad sobre el **WACC** para obtener un precio objetivo.

**Herramientas y entorno de trabajo:**  
- Python: Pandas, NumPy, Matplotlib, yfinance, scipy.  
- Jupyter Notebooks para desarrollo y visualización interactiva.  
- GitHub para control de versiones y almacenamiento del código/resultados.

---

## 3. Principales Hallazgos

- **Correlaciones y diversificación:** Alta correlación entre activos argentinos (LOMA, PAMP, MERVAL USD) y menor con internacionales (CRH, CX, VMC, S&P500).  
- **Optimización de cartera:** El portafolio **50/50** alcanzó el máximo Sharpe bajo esa restricción.  
- **Indicadores técnicos:** Estrategia combinada (SMA+RSI+MACD+ADX+Bollinger) superó al *buy & hold* en rendimiento ajustado por riesgo.  
- **Valuación fundamental:** El **DCF** arrojó un precio objetivo en USD muy superior al de mercado; múltiplos bajos reflejan la prima de riesgo argentino.  
- **Factores macroeconómicos:** Pandemia 2020, rally pospandemia 2021–2022 e inestabilidad argentina 2022–2023 fueron drivers clave.

**Conclusión:** LOMA combina **potencial de valorización** y **alto riesgo país**; útil para diversificación si se gestiona exposición de forma activa.

---

## 4. Recomendación de Inversión

### Estrategia de asignación
- Peso recomendado: **10-15% del portafolio** dentro del bloque argentino.  
- Estructura sugerida: **50% Argentina (LOMA, PAMP)** y **50% internacional (CRH, CX, VMC, S&P500)**.

### Estrategia operativa
- Entradas cuando confluyan señales técnicas: SMA 50>200, MACD>0, RSI saliendo de sobreventa, compresión de Bollinger con confirmación de volumen.
- Salidas parciales cerca del precio objetivo si hay señales de agotamiento.

### Gestión de riesgo y horizonte
- Horizonte mediano/largo plazo.
- Diversificación geográfica como protección ante eventos macro locales.

**Benchmark:** MERVAL USD y S&P 500.

---

## 5. Anexos

### Eventos Macroeconómicos Relevantes

| Evento                                 | Fecha principal | Afectados principales              | Breve descripción                                                                 | Impacto resumido                                                                 |
| -------------------------------------- | --------------- | ---------------------------------- | --------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| Pandemia COVID-19 y crash global       | Marzo 2020      | Todas las acciones e índices       | Caída abrupta global por cuarentenas y freno económico.                           | Caídas >30% en semanas; alta volatilidad y posterior rebote parcial.             |
| Rally pospandemia + inflación global   | 2021-2022       | CRH, CX, VMC, S&P500 (+ globales)  | Rebote de demanda, suba de precios y luego corrección por tasas altas e inflación | Fuertes subas en 2021; corrección en 2022; oportunidad para trading activo.      |
| Crisis argentina 2022/23 (devaluación) | 2022-2023       | LOMA, PAMP, MERVAL                 | Inflación, devaluaciones, controles cambiarios y crisis política en Argentina     | Alta volatilidad y caída en USD; aumento del riesgo país y correlación local.    |

### Cartera
<img width="1315" height="701" alt="Precios normalizados" src="https://github.com/user-attachments/assets/264d2ec9-81ff-437c-b90a-d4204268518b" />

<img width="764" height="682" alt="Matriz de correlacion" src="https://github.com/user-attachments/assets/9574a5d0-b4b3-4b35-b0a3-3d866f9a44c1" />

<img width="952" height="702" alt="Frontera eficiente" src="https://github.com/user-attachments/assets/b1ca32e1-c808-4563-9a11-1c9bf041a4d1" />

### Tecnico

<img width="1589" height="690" alt="SMA" src="https://github.com/user-attachments/assets/f549163b-9928-4e0d-8ca2-0ccdfe1055fd" />

<img width="1510" height="890" alt="MACD" src="https://github.com/user-attachments/assets/57bc0db5-789b-44b4-88e8-de621f57a2ea" />

<img width="1489" height="490" alt="RSI" src="https://github.com/user-attachments/assets/a6b315d5-d407-4b7b-98bb-8a8856836b3a" />

<img width="1490" height="490" alt="ADX" src="https://github.com/user-attachments/assets/f1bcc65b-f3cc-4131-a439-2b8f7e8c464b" />

<img width="1589" height="690" alt="Bandas" src="https://github.com/user-attachments/assets/99d35e3c-e57f-4531-9408-7e1c7ed0fb85" />

<img width="1489" height="690" alt="Resumen" src="https://github.com/user-attachments/assets/15a19e00-5b85-4187-becc-7aa4a6ef9879" />

### Fundamentals

| **Métrica**             | **LOMA**    | **CRH**     | **VMC**     | **CX**      |
|-------------------------|-------------|-------------|-------------|-------------|
| EV/EBITDA               | 56.91600    | 1.77600     | 12.89300    | 20.12800    |
| Forward P/E             | 11.68493    | 12.06897    | 18.26030    | 32.11674    |
| Price/Book               | 0.00131     | 3.33946     | 4.57881     | 9.26167     |
| Operating Margin         | 0.18822     | 0.22279     | 0.10207     | 0.08484     |
| Profit Margin            | 0.09909     | 0.12523     | 0.09608     | 0.07760     |
| ROA                      | 0.06232     | 0.05953     | 0.03014     | 0.04119     |
| ROE                      | 0.14782     | 0.11870     | 0.07033     | 0.06625     |
| Total Debt/Equity        | 29.42900    | 50.67900    | 65.38400    | 74.47300    |
| Interest Coverage        | 7.61031     | 3.32310     | 9.33579     | 10.17021    |
| Beta                     | 0.96600     | 1.19500     | 0.83200     | 1.07800     |
| Market Cap               | $1,246,381,000 | $74,493,570,000 | $38,530,000,000 | $12,672,930,000 |


| **Variable**        | **Valor**           |
|---------------------|---------------------|
| FCF TTM             | $150,000,000        |
| WACC Base           | 10%                 |
| Growth Rate         | 5%                  |
| Terminal Growth     | 2%                  |
| Valor Empresa       | $2,169,317,835      |
| Precio Objetivo     | 18.59 USD           |
| Precio Mercado      | 10.50 USD           |
| Diferencia %        | 77%                 |
| **Recomendación**   | **COMPRAR**         |





---
