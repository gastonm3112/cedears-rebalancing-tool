# cedears-rebalancing-tool
# 📈 Rebalanceador de Cartera CEDEARs (Argentina)

Herramienta automatizada en Python para calcular el rebalanceo de una cartera de inversiones, conectándose directamente a Google Sheets y obteniendo precios de mercado en tiempo real.

## 🚀 Funcionalidades
* **Conexión Cloud:** Lee tu portafolio directamente desde Google Sheets.
* **Precios en Vivo:** Utiliza la API de Yahoo Finance (`yfinance`) para cotizaciones de CEDEARs en pesos (Ticker.BA).
* **Modo Híbrido:** Si Yahoo falla, permite usar un precio manual definido en el Excel.
* **Cash Flow:** Permite calcular el rebalanceo inyectando capital nuevo, priorizando compras y evitando ventas innecesarias.
* **Output Automático:** Genera una nueva pestaña en el Google Sheet con las órdenes de compra/venta exactas.

## 🛠️ Tecnologías
* Python 3
* Pandas
* Google Colab (Entorno de ejecución)
* Google Sheets API (`gspread`)

## 📋 Cómo usarlo
1.  Abre el archivo en Google Colab haciendo clic en el botón de arriba.
2.  Configura el nombre de tu archivo de Google Sheets en el formulario.
3.  Tu hoja de Google Sheets debe tener una pestaña con las columnas: `Ticker`, `Nominales`, `Objetivo` (y opcional `Precio_Manual`).
4.  Ejecuta el script y sigue las instrucciones de autenticación de Google.

---
*Este proyecto fue creado para automatizar la gestión de inversiones personales en el mercado argentino (BYMA).*
