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
## HORA 9 - Semana 02 · NumPy y arreglos - COMPLETADA 09/11/2026

Práctica sin copiar: Ventas de tienda con NumPy.
Creé ventas = np.array([250, 400, 180, 500, 320, 280]).
Verifiqué ventas.sum() = 1930 (total), ventas.mean() = 321.666... (promedio), ventas.max() = 500 (mayor), ventas.min() = 180 (menor).
Verifiqué ventas > 300 = [False True False True True False] y (ventas > 300).sum() = 3 días mayores a 300.
Errores que aprendí: mean(ventas) solo da NameError porque mean solo no existe, tiene que ser ventas.mean(). ventas.ventas da AttributeError porque es ventas una sola vez.

Aprendizajes:
1. Aprendí que sum() es de Python, pero que .sum() es de NumPy.
2. Aprendí que siguiendo la práctica .max(), .min() y > 300 por ejemplo, generan el máximo, el mínimo y los mayores que 300 en booleanos de un array.
3. Todavía me cuesta en este caso arrancar con el import de NumPy, pero ya empecé a automatizarme al respecto.

IA: Pedí guía paso a paso a Meta AI, resolví la práctica yo mismo sin copiar la solución, ejecuté cada comando en mi entorno y verifiqué los resultados yo mismo.
## HORA 10 - COMPLETADA el 11/11/2026
- Semana 02 · NumPy y arreglos - Sesión 4: Aplicar numpy y arreglos a un pequeño problema.
- Problema de finanzas, resuelto solo:
  ingresos = np.array([1200, 1350, 1100, 1500, 1400])
  gastos = np.array([900, 1000, 950, 1100, 1050])
  ahorro = ingresos - gastos -> [300 350 150 400 350]
  ahorro.sum() -> 1550 total ahorrado
  ahorro.mean() -> 310.0 promedio por mes
  ahorro.max() -> 400 mes que más ahorró
  ahorro.min() -> 150 mes que menos ahorró
  ahorro > 300 -> [False True False True True]
  (ahorro > 300).sum() -> 3 meses ahorraron más de 300
- Mis 3 aprendizajes HORA 10:
    1. Aprendí a automatizarme más, usando .max(), .min() y sobre todo (ahorro > 300).sum().
    2. Hice el problema completo de ahorro, total, promedio, mayor, menor y cuántos meses superaron 300.
    3. En la terminal me siguió costando ingresar a .venv.
    ## HORA 11 - COMPLETADA el 11/11/2026
- Semana 02 · NumPy y arreglos - Sesión 5: Consolidación de NumPy y manejo de arreglos.
- Problema A - Finanzas nuevas, resuelto solo:
  ingresos = np.array([3000, 3500, 3200, 4000, 3800])
  gastos = np.array([2100, 2400, 2200, 2600, 2500])
  ahorros = ingresos - gastos -> [900 1100 1000 1400 1300]
  ahorros.sum() -> 5700 total ahorrado
  ahorros.mean() -> 1140.0 promedio por mes
  ahorros.max() -> 1400 mes que más ahorró
  ahorros.min() -> 900 mes que menos ahorró
  ahorros[ahorros > 1000] -> [1100 1400 1300] = seleccionar cuáles superaron 1000
- Problema B - Ventas nuevas, resuelto solo:
  ventas = np.array([1200, 1800, 950, 2200, 1600, 800])
  ventas.sum() -> 8550 total
  ventas.mean() -> 1425.0 promedio
  ventas.max() -> 2200 venta más alta
  ventas[ventas > 1500] -> [1800 2200 1600] = seleccionar cuáles superaron 1500
- Concepto nuevo: seleccionar con máscara. (ahorros > 1000).sum() dice cuántos, ahorros[ahorros > 1000] dice cuáles son.
- Mis 3 aprendizajes HORA 11:
    1. Aprendí a automatizar mis inicios de sesión en VS Code para usar python.
    2. Aprendí el modo de seleccionar información numérica mediante los signos de mayor o menor que.
    3. Estoy aprendiendo que debo coordinar las horas de estudio unificando proyecto de estudio de chatgpt con meta ai.
    Mis 3 aprendizajes HORA 12:
1. Aprendí a hacer un entregable completo en un archivo .py y correrlo desde PowerShell, no solo en notebook.
2. Aprendí que una máscara devuelve True/False, .sum() dice CUÁNTOS y array[mascara] dice CUÁLES.
3. Aprendí a combinar condiciones con & y a usar f-string con {ventas.mean()} para que el texto se actualice solo.
Qué sugerencia de la IA acepté y por qué: Acepté usar {ventas.mean()} en la conclusión porque así no tengo que corregir el número a mano si cambian los datos.
Qué sugerencia rechacé y por qué: No rechacé ninguna, la única sugerencia fue la del f-string y la acepté.
Mis 3 aprendizajes HORA 13:
1. Aprendí a leer un CSV real con pd.read_csv() y guardarlo en df, con mis columnas reales: mes, ingresos, gastos, ahorro.
2. Aprendí que df.shape y df.dtypes son atributos sin paréntesis, y que en pandas 3.1.1 el texto es str, no object.
3. Aprendí que df[df["ingresos"] > 3500] me devuelve filas enteras, y que con & puedo combinar dos condiciones, ej: ingresos > 3500 y ahorro > 800 me dio 3 meses: Junio, Septiembre y Octubre.
HORA 14: Semana 03 · Pandas - Limpieza y orden de datos - COMPLETADA el 18/11/2026
- Archivo: datasets/finanzas_mensuales.csv
- Notebook: notebooks/03_pandas_finanzas.ipynb
- Cargué con: import pandas as pd / df = pd.read_csv("../datasets/finanzas_mensuales.csv")
- El ../ fue necesario porque el notebook está dentro de notebooks/ y tiene que subir un nivel para encontrar datasets/
- 1) Vacíos: df.isnull().sum() -> mes 0, ingresos 0, gastos 0, ahorro 0. No hay valores vacíos.
- 2) Duplicados: df.duplicated().sum() -> np.int64(0). No hay filas duplicadas.
- Al principio puse df.duplicated() y df.sum() en dos líneas separadas y solo me mostró el df.sum(). Aprendí que en el notebook solo muestra la última línea, hay que ponerlo junto: df.duplicated().sum()
- 3) drop_duplicates(): lo revisé, no había nada que borrar porque había 0 duplicados.
- 4) Ordenar: df.sort_values(by="ahorro", ascending=False)
- Al principio puse df.sort_values(900, 4000) y dio error porque sort_values ordena por nombre de columna, no por números sueltos.
- Resultado ordenado de mayor a menor: Abril 900, Junio 900, Septiembre 900, Octubre 900, Enero 800, Agosto 800, Febrero 700, Marzo 700, Mayo 500, Julio 500.
- Verificación: empieza en 900 y termina en 500. Los índices de la izquierda (3, 5, 8, 9...) son los originales, no se borran al ordenar.
- Problemas de hoy: VS Code se actualizó a 1.147 y dejó la terminal en blanco con 4 powershell colgadas. Lo arreglé con PowerShell fuera de VS Code y con Developer: Reload Window para que Jupyter volviera a abrir el notebook.
- Mis 3 aprendizajes HORA 14:
    1. Aprendí que isnull() busca nulos y duplicated() busca los duplicados.
    2. Aprendí que sort_values(by="ahorro", ascending=False) entrega los números de ahorro en orden descendente.
    3. Lo que más me costó hoy fue activar la terminal.