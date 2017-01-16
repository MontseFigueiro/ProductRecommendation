SISTEMAS DE RECOMENDACION
-------------------------

Un recomendador es un sistema que selecciona un producto que si se
compra maximiza el valor tanto para comprador como para vendedor. El
sistema procesa información histórica de los usuarios, de los productos
y la transforma en información para predecir que producto puede ser
interesante para el usuario y para la empresa.

Son de dos tipos:

-   **Filtros Colaborativos**

Basan su lógica en las características del usuario.

-   **Filtros basados en contenido**

Utilizan las características del artículo (marca, precio, tamaño....)
para hacer la recomendación.

Un filtro es un algoritmo matemático que decide cual es la
recomendación.

CASO SANTANDER
--------------

En éste caso la información de la que disponemos es del usuario no del
producto, tenemos:

-   fecha\_dato
-   ncodpers
-   ind\_empleado: A active, B ex employed, F filial, N not employee, P
    pasive
-   pais\_residencia
-   sexo
-   age
-   fecha\_alta
-   ind\_nuevo: 1 si el cliente se registró en los últimos 6 meses
-   antiguedad: en meses
-   indrel: 1(principal), 99(principal cliente durante el mes pero no al
    final del mes)
-   ult\_fec\_cli\_1t: ultima fecha como cliente principal
-   indrel\_1mes: tipo cliente, 1(principal), 2(co-propietario),
    P(potencial), 3(ex principal), 4 (ex- copropietario)
-   tiprel\_1mes: relacion del cliente, A (activo), I (inactivo), P(ex
    cliente), R(potencial)
-   indresi: residencia S o N si el país de residencia es el misma que
    el del banco
-   indext: S o N si el país de nacimiento es el mismo que el país
    del banco.
-   conyuemp: 1 si el cliente está casado con un trabajador
-   canal\_entrada: canal elegido por el cliente para unirse
-   indfall: indice fallecido S/N
-   tipodom: tipo direccion, 1 principal
-   cod\_prov: provincia cliente
-   nomprov
-   ind\_actividad\_cliente: 1 cliente activo, 0 cliente inactivo
-   renta: ingresos brutos de la unidad familiar
-   segmento: 01-VIP, 02-individuals, 03-college graduated

Si indrel tiene como valor 1, es cliente principal, son la mayoría de
las observaciones, entonces la última fecha como cliente principal está
vacía. Si ya no es cliente principal el valor de indrel es 99 entonces
figura fecha en esta columna.
