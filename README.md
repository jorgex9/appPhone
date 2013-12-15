appPhone
========

Aplicacion de pruebas Phonegap

Se realizo el consumo de datos desde un server php pasando los datos en json
para la utilizacion de la App, debe tener un servidor web con php 5.2.* o superior
en el debe agregar el archivo reply.php.

configurar en config.xml el acceso a su servidor, de la siguiente manera 

 access origin="http://192.168.1.102/appPhoneServer/"

cambiando la ip de su server y el path donde haya creado el reply.php

luego debe tambien hacer las mismas modificaciones en la funcion connect
que se encuentra en index.htm, de forma similar pero aqui ya haciendo referencia
al archivo reply.php

url:'http://192.168.1.102/appPhoneServer/reply.php', 

con esto logramos consumir info desde un server.Podemos acceder a el, que este consulte
a una BD y luego devolver lo que quermos con la funcion json_encode()

