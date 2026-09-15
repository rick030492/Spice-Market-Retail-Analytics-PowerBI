# 🌶️ Analytics Dashboard: Mercado de las Especias (Power BI & DAX)

Este proyecto desarrolla un **Dashboard de Analítica Comercial** para el segmento *Masalas & Spices* a partir de datos de retail de BigBasket. El objetivo principal es evaluar el volumen de ingresos, costos operativos y margen de beneficio comercial mediante el modelado de datos en Power Query y métricas calculadas en DAX.

---

## 📊 KPIs Principales

| Indicador | Valor Calculado | Descripción |
| :--- | :--- | :--- |
| **Ingresos Totales** | $1,27 Mill. | Suma total de los precios de venta (`sale_price`). |
| **Costo Total** | $93 Mil | Suma total de los costos de mercado (`market_price`). |
| **Ganancia / Margen Bruto** | $1,18 Mill. | Ganancia neta calculada (`Ingresos - Costos`). |
| **% Margen de Beneficio** | 92,7% | Eficiencia comercial de las ventas. |

---

## 📐 Medidas DAX Implementadas

```dax
Ingresos_Totales = SUM('BigBasket Products'[sale_price])

Costo_Total = SUM('BigBasket Products'[market_price])

Ganancia_Monto = [Ingresos_Totales] - [Costo_Total]

Porcentaje_Margen = DIVIDE([Ganancia_Monto], [Ingresos_Totales], 0)
```

---

## 🛠️ Herramientas Utilizadas
* **Power Query:** Limpieza, filtrado por subcategoría (*Masalas & Spices*) y transformación del esquema de datos.
* **Power BI Desktop:** Modelado de datos, creación de medidas DAX y desarrollo de la interfaz visual interactiva.
* **DAX (Data Analysis Expressions):** Cálculos financieros y relacionales.

---

## 📸 Vista Previa del Dashboard
*(Puedes tomar una captura de pantalla a tu Power BI terminado, pegarla dentro del repositorio y arrastrarla aquí)*# Spice-Market-Retail-Analytics-PowerBI
Dashboard de analítica comercial y margen de ganancia para el segmento de especias utilizando Power BI y DAX.
