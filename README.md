# Analisis_de_riesgo-de_prestamos_de_un_banco
# Introducción
El proyecto consiste en preparar un informe para la división de préstamos de un banco.
Contestaremos las siguientes hipotesis:
- ¿Existe una correlación entre tener hijos y pagar a tiempo?
- ¿Existe una correlación entre la situación familiar y el pago a tiempo?
- ¿Existe una correlación entre el nivel de ingresos y el pago a tiempo?
- ¿Cómo afecta el propósito del crédito a la tasa de incumplimiento?
 
todas estas tienen un impacto en el incumplimiento de pago de un préstamo??. 
El banco ya tiene algunos datos sobre la solvencia crediticia de los clientes.
El informe tendrá en cuenta la puntuación de crédito para un cliente potencial. 
# Descripción de los datos
- `children` - el número de hijos en la familia
- `days_employed` - experiencia laboral en días
- `dob_years` - la edad del cliente en años
- `education` - la educación del cliente
- `education_id` - identificador de educación
- `family_status` - estado civil
- `family_status_id` - identificador de estado civil
- `gender` - género del cliente
- `income_type` - tipo de empleo
- `debt` - ¿había alguna deuda en el pago de un préstamo?
- `total_income` - ingreso mensual
- `purpose` - el propósito de obtener un préstamo
- # Habilidades técnicas
- Phyton
- Pandas
  # Conclusión General
**Realizamos una exploración inicial de los datos:**

Viendo las siguientes inconsistencias;

- En la columna de `days_employed`, no tienen sentido los valores negativos y el entero máximo (son muchísimos los días para que una persona pueda trabajar en vida)
- En la columna `children` el valor -1 tampoco tiene sentido
- valores ausentes en `days_employed` y `total_income`
- valores simétricos en la columna 'days_employed' y 'total_income'.
- mala captura a la hora del registro de los datos 
- El porcentaje de valores ausentes fue del 10%


**Realizamos una transformacion de los datos:**
- corrregimos errores tipográficos y de ortografia
- cambiamos valores que no tenian ningun sentido probablemente por errores de captura
- Eliminamos datos duplicados
- Agregamos valores más descriptivos a ciertas columnas
- Añadimos nuevas caracteristicas a nuestra tabla
- Trabajamos con los valores ausentes


**Trabajamos con las hipótesis:**

Pudimos evidenciar que las mayores tasas de impago son: 

- Las personas con rango de 1 a 2 hijos.
- Las personas Solteras
- Las personas con ingresos medios
- Las personas con credito para un carro

