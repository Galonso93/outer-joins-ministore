# outer-joins-ministore

¿Por qué usaste LEFT JOIN para la Consulta 1 y no INNER JOIN? ¿Qué se perdería si usaras INNER JOIN?
Si hubiera usado INNER JOIN no podría ver nunca los productos 108 y 109 porque no tuvieron ventas. INNER JOIN solo trae cuando encuentra valores NO NULL en ambas tablas.

¿Por qué usaste RIGHT JOIN para la Consulta 2? ¿Qué tabla está a la izquierda y cuál a la derecha en tu consulta?
Usé RIGHT JOIN para la Consulta 2 porque necesitaba ver todas las ventas para así identificar los NULL. Es la venta 10. A la izquierda está la tabla productos y a la derecha la tabla ventas

¿Qué representan los valores NULL en cada resultado? Explicá con un ejemplo concreto de los datos qué significa que venta_id sea NULL en la Consulta 1 y que producto_id de productos sea NULL en la Consulta 2.
Los valores NULL en cada resultado son celdas vacías. Que venta_id sea NULL en la Consulta 1 tiene que ver con que esos productos (108 y 109) no tuvieron ventas en el período analizado. Que producto_id sea NULL en la Consulta 2 significa que se realizaron ventas de productos que no estaban registrados en la tabla productos (La venta 10). 

¿Cuándo usarías FULL OUTER JOIN en un caso real de negocio?
Lo usaría cuando necesito un panorama completo de ventas y productos. Revisar inventarios y cantidades vendidas de cada productos.
