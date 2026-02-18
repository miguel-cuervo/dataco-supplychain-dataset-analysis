# DataCo Supply Chain Analysis
## Introducción
El siguiente proyecto cuenta con un enfoque dirigido completamente al análisis mediante SQL de un dataset de cadena de suministro. Alineados con el objetivo central y fundamental de la cadena de suministro siendo optimizar flujos de información, productos e ingresos; el objetivo de este proyecto es optimizar el flujo de la cadena de suministro de DataCo, reduciendo entregas retrasadas e identificando regiones con la rentabilidad más alta.
## Procedimiento
Antes de comenzar con el análisis real, se debía importar el dataset dentro de nuestra nueva base de datos (denominada supply_chain) creada en la herramienta DBeaver. Al importar la información, se realizan los cambios necesarios a los nombres de columnas, procurando mantener un formato snake_case, además del tipo de data correspondiente.
Antes de continuar con la sección analítica de nuestro proceso, debemos asegurarnos de que no se encuentren datos sucios entre nuestra información. Para esto, corremos una query que nos permita identificar valores vacíos o menores a 0. El resultado nos muestra que no existen dichos valores. 

<img width="370" height="323" alt="image" src="https://github.com/user-attachments/assets/5fcb7afd-8a54-4596-826e-51270c6d4181" />

Ahora continuaremos con la parte analítica de nuestro proceso, añadiendo un query que nos arroje un total dependiendo del tipo de estatus de envío de cada pedido, podemos notar que los envíos retrasados son un gran porcentaje del total, siendo más del triple de los pedidos a tiempo y el doble de los anticipados. 

<img width="373" height="393" alt="image" src="https://github.com/user-attachments/assets/ee27e74b-d144-47d0-b886-4838ec2f7859" />

Procedemos con otro query que nos detalla los totales tanto de ventas como ganancia. Podemos notar que la región de Europa Occidental es la que se encuentra en la primera posición con más ventas y ganancias, seguida de Centroamérica y bastante por debajo, Sudamérica.

<img width="440" height="554" alt="image" src="https://github.com/user-attachments/assets/0ba34e39-e5cd-4c85-b789-3b774c531510" />

Para concluir con la parte de SQL, insertamos una última query que nos arroje el total de productos con mayores retrasos, identificando las raíces de los problemas por producto específico.

<img width="360" height="500" alt="image" src="https://github.com/user-attachments/assets/5c2cb16a-a5f9-46d1-be65-3c4ede876e01" />

## Conclusiones
Para cerrar este proyecto de análisis, podemos notar que, basándonos en la información recolectada y analizada, la empresa sufre gravemente de envíos retrasados. De 180,000 órdenes analizadas aproximadamente, más del 50% de los pedidos han sido retrasados. Al adentrarnos un poco más en las categorías de producto con mayores problemas, podemos encontrar que en primer lugar tenemos el calzado para hombres (siendo el primer lugar los tacos deportivos), seguidos de la ropa para dama. 
Por consiguiente, se deben atacar directamente las causas de los retrasos para esos productos en las regiones que generan más ingresos para la empresa, se puede comenzar con las primeras 2 que abarcan la mayor parte del porcentaje de las ganancias, estas siendo Europa Occidental y Centroamérica. Esto nos desbloquearía un incremento inmediato de ganancias adicionales en las regiones, seguido con un proceso de ampliación a más regiones siguiendo la guía de productos con mayores problemas. 
