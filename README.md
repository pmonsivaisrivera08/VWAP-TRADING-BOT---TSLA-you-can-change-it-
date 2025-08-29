
📈 Bot de Trading de VWAP
Este bot de trading automatizado, escrito en Python, implementa una estrategia de ruptura de VWAP (Volumen Ponderado por Precio), ideal para el trading intradiario. El código realiza un backtest de la estrategia y evalúa su rendimiento con datos históricos.

Funcionamiento de la Estrategia
Identificación de Tendencia: La estrategia determina la tendencia a corto plazo comparando el precio con el VWAP. Si el precio está por encima del VWAP, se considera una tendencia alcista; si está por debajo, una tendencia bajista.

Señales de Entrada:

Compra (Largo): El bot abre una posición de compra cuando el precio de cierre de la vela cruza por encima del VWAP y la vela es alcista (verde).

Venta (Corto): El bot abre una posición de venta cuando el precio de cierre de la vela cruza por debajo del VWAP y la vela es bajista (roja). El backtest sugiere que eliminar la condición del color de la vela puede mejorar el rendimiento.

Gestión de Operaciones:

Stop-Loss Dinámico: Se utiliza un trailing stop basado en el indicador Average True Range (ATR) para proteger las ganancias a medida que la operación avanza.

Cierre al Final del Día: Todas las operaciones abiertas se cierran automáticamente antes del final de la sesión de trading para evitar riesgos durante la noche.

Resultados del Backtest
El backtest realizado con datos de acciones de Apple en un marco de tiempo de 15 minutos muestra que, sin considerar las comisiones, la estrategia puede ser rentable. Sin embargo, el bot es muy sensible a las comisiones de trading, lo cual debe ser considerado al usarlo.


Cómo Usar
Instalar Dependencias: Asegúrate de tener instaladas las librerías necesarias, incluyendo backtesting.py.

Configuración: Modifica los parámetros en el script para ajustar el activo, el marco de tiempo y los parámetros de gestión de riesgos según tus preferencias.

Ejecutar el Bot: Corre el script en un entorno como Jupyter Notebook para realizar el backtest y analizar los resultados.

Este proyecto es una excelente base para aprender sobre estrategias de trading cuantitativo. Se recomienda optimizar los parámetros y probarlo en diferentes mercados para mejorar su rendimiento.

_________________________________________________________________________________________________________________________________________________________________________________________________

📈 VWAP Trading Bot
This is an automated trading bot written in Python that implements a "VWAP Breakout" strategy, designed for intraday trading. The code includes a backtesting framework to evaluate the strategy's performance using historical data.

Strategy Explained
Trend Identification: The strategy determines the short-term trend by comparing the asset's price to its VWAP (Volume-Weighted Average Price). If the price is above the VWAP, it's considered an uptrend; if it's below, it's a downtrend.

Entry Signals:

Buy (Long): The bot opens a buy position when the candle's closing price crosses above the VWAP and the candle is bullish (green).

Sell (Short): The bot opens a sell position when the candle's closing price crosses below the VWAP and the candle is bearish (red).

Trade Management:

Dynamic Stop-Loss: It uses a trailing stop-loss based on the Average True Range (ATR) indicator to protect gains as the trade moves in a profitable direction.

End-of-Day Closure: All open positions are automatically closed before the end of the trading session to avoid overnight risk.

How to Use
Install Dependencies: Ensure you have the necessary libraries installed, including backtesting.py.

Configure Parameters: Modify the script to adjust the asset, timeframe, and risk management parameters to fit your trading style.

Run the Bot: Execute the script in an environment like a Jupyter Notebook to perform backtesting and analyze the results.

This project is an excellent starting point for learning about quantitative trading strategies. Feel free to modify and optimize it for your specific needs.
