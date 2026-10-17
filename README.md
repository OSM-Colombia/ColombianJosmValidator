# ColombianJosmValidator
Reglas de validación de mapeo en Colombia para JOSM.

Estas reglas están basadas en la guía de mapeo de Colombia:

* Spanish: [Guía para mapear](https://wiki.openstreetmap.org/wiki/ES:Colombia/Gu%C3%ADa_para_mapear).
* English: [Guide_for_mapping](https://wiki.openstreetmap.org/wiki/Colombia/Guide_for_mapping).

Agradecimientos a todos los participantes de las sesiones de MaptimeBogota, con quienes hemos hablado de varios lineamientos de mapeo en Colombia, lo cual se ha convertido en este conjunto de reglas.
Nuestro objetivo es que el mapa de Colombia esté estructurado, y que no se sigan adicionando elementos que ya hemos corregido.

Cualquier cambio en las reglas o adición de reglas es bienvenido.
Lo puedes reportar creando un Issue aquí en GitHub o escribiéndonos en nuestro canal de Telegram.

Este validador fue hecho basado en la [documentación de JOSM](https://josm.openstreetmap.de/wiki/Help/Validator/MapCSSTagChecker) y en las reglas de Brazil y de otros países.

Muchas de las reglas están descritas con expresiones regulares, que permiten describir cadenas de caracteres.
Si quieres aprender de ellas, hay muchos recursos en Internet como https://regexone.com/

Si consideras que el validador debe tener más reglas, puedes crear un issue describiendo al escenario, y posibles casos de uso.
También puedes crear un fork de este proyecto, adicionar las reglas, y crear un pull request.
Si tienes dudas, no dudes en contactarnos por redes sociales @MaptimeBogota.

Este conjunto de reglas está listado en https://josm.openstreetmap.de/wiki/RulesSource

## Activación en JOSM

Para utilizarlo asegúrate que esté activo en JOSM. Para eso, sigue estos pasos:

* Ventana principal de JOSM.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/1-JOSM.png?raw=true)

* Abres las preferencias, ya sea desde el menú editor o de imágenes.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/2-Preferencias.png?raw=true)

* Cambias la pestaña izquierda a la de validador de datos, o en otros términos hacer click, lo que en Colombia llamamos, el chulito.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/3-Validator.png?raw=true)

* Así aparece cuando no está activado lo de Colombia. Buscamos las reglas a la izquierda.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/4-Lista.png?raw=true)

* Debe aparecer a la derecha y seleccionado.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/5-Activada.png?raw=true)

## Reglas que valida

* Nombre incorrecto en ríos.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/1-rios.png?raw=true)

* Nombre incorrecto en quebradas.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/2-quebradas.png?raw=true)

* Mapeo de autopistas inexistentes. En Colombia como tal no hay.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/3-autopista.png?raw=true)

* Living streets como tal no existen en Colombia, son las residenciales.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/4-livingStreetName.png?raw=true)

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/5-livinStreetNoName.png?raw=true)

* Las vías no categorizadas muchas veces pueden ser un error de categorización. Por lo que aquí es una advertencia.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/6-unclassified.png?raw=true)

* Los nombres de las vías tienen una estructura bien definida: tipo número.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/7-nombreVia.png?raw=true)

* El nombre alterno no puede ser el nombre numérico.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/8-nombreAlternoVia.png?raw=true)

* La dirección completa no puede ir en el campo calle de dirección.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/9-streetName.png?raw=true)

* La dirección completa no puede ir en el campo número.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/10-houseNumber.png?raw=true)

* Los números de teléfono tienen una estructura definida.

![](https://github.com/OSM-Colombia/ColombianJosmValidator/blob/main/images/reglas/11-telephone.png?raw=true)
