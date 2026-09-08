1. ¿Por qué usaste LEFT JOIN para la Consulta 1 y no INNER JOIN? ¿Qué se perdería si usaras INNER JOIN?
  porque LEFT JOIN me permite ver todos los registros de la tabla izquierda (Productos) con las coincidencias de la tabla de la derecha (Ventas) y los registros sin coincidencias son NULL (productos sin ventas registradas).
2. ¿Por qué usaste RIGHT JOIN para la Consulta 2? ¿Qué tabla está a la izquierda y cuál a la derecha en tu consulta?
   porque RIGHT JOIN me permite ver todos los registros de la columna derecha (ventas) y las coincidencias de la tabla de la izquierda (productos), asi puedo ver todas las ventas incluidas las que no tienen un productoID vinculado.
3. ¿Qué representan los valores NULL en cada resultado? Explicá con un ejemplo concreto de los datos qué significa que venta_id sea NULL en la Consulta 1 y que producto_id de productos sea NULL en la Consulta 2.
   En la primer consulta, que venta_id sea NULL significa que no hay registros de ventas asociados a esos producto_id, es decir que nunca se vendieron esos productos_id. Y que producto_id sea NULL en la consulta 2 significa que ese registro de venta no esta vinculado a ningun producto_id de la base de datos, lo que puede representar un mal registro en el producto_id de la venta. 
4. ¿Cuándo usarías FULL OUTER JOIN en un caso real de negocio?
   Cuando necesito ver todos los registros, sin que se eliminen por ser NULL en las vinculaciones. 
