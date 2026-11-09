# Bitácora AI-Mastery - Plan 24 meses / 624 horas

## HORA 6 - Revisión EDA + 3 aprendizajes
Fecha: 04/11/2026
Archivos verificados: datasets/finanzas_mensuales.csv, notebooks/02_analisis_exploratorio.ipynb

### Lo que verifiqué
- `df` es el DataFrame, la tabla de finanzas cargada en pandas. Es como el Excel en código.
- `df.shape` me dice el número de filas y columnas de mi df. En mi caso 10 meses y 4 columnas.
- `df.isnull().sum()` me dice si hay huecos en mi df. En mi caso 0 en todo, todas las celdas están ocupadas.

### Mis 3 aprendizajes
1. En mi plan de estudios, sesión equivale a hora. 1 sesión = 1 hora.
2. `Get-ChildItem` sirve para ver qué hay dentro de una carpeta en VS Code. `.venv` es el entorno virtual activo, la cajita aislada donde trabajan las herramientas de este proyecto.
3. Todavía me cuesta escribir todo el código sin IA guiándome. Es natural porque estoy empezando a entenderlo. Primer paso: sentar bases para ir familiarizándome cada vez más.

### Regla IA que estoy usando
Primero pienso yo, después pido pista a la IA, después verifico ejecutando. Nunca acepto código sin explicarlo.
## HORA 7 - Semana 02 · NumPy y arreglos - COMPLETADA 05/11/2026

Práctica: Creé mi primer arreglo a = np.array([10, 20, 30, 40, 50]) con NumPy 2.5.4.
Verifiqué a.shape = (5,), a.dtype = int64, a.sum() = 150.
Operaciones: a + 10 = [20, 30, 40, 50, 60], a * 2 = [20, 40, 60, 80, 100], a.mean() = 30.0.

Aprendizajes:
1. Aprendí que un arreglo es una estructura de datos, en el caso de NumPy sin comas.
2. Aprendí que NumPy sirve para la computación científica.
3. Todavía me cuesta las entradas a la terminal vía New Terminal, pero ya me automatizaré al respecto.

IA: Pedí guía paso a paso a Meta AI, ejecuté cada comando en mi entorno y verifiqué los resultados yo mismo.
## HORA 8 - Semana 02 · NumPy y arreglos - COMPLETADA 09/11/2026

Práctica guiada: Ejemplo de finanzas con NumPy.
Creé ingresos = np.array([1200, 1350, 1100, 1500, 1400]) y gastos = np.array([900, 1000, 950, 1100, 1050]).
Calculé ahorro = ingresos - gastos y salió [300 350 150 400 350].
Verifiqué ahorro.sum() = 1550 (total ahorrado en 5 meses) y ahorro.mean() = 310.0 (promedio por mes).
Entendí int64 = entero en 64 bits sin decimales, float64 = número con decimales en 64 bits, con unos 15 dígitos de precisión, no 64 decimales.

Aprendizajes:
1. Aprendí que NumPy se puede usar a la manera de nuestro ejemplo guiado en finanzas.
2. Aprendí que for no es necesario en estos casos porque aunque trabajamos con Python, tenemos las ventajas de abreviación de trabajo de NumPy para estos casos.
3. Todavía me cuesta cosas elementales como discernir que podía usar la terminal sin incidencia en lo que llamaste el editor, que espero que se me grabe en la memoria, que así se llama precisamente ese sector de VS Code.

IA: Pedí guía paso a paso a Meta AI, ejecuté cada comando en mi entorno y verifiqué los resultados yo mismo.
