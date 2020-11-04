## Disposición de Accesibilidad
Esta disposición nos ayudará a mapear objetos relacionados a la calidad de accesibilidad que se encuentra en un lugar, por ejemplo, nos permite registar que en cierto punto de una acera hay un obstáculo que imposibilita el paso de una silla de ruedas o que hay una rampa inadecuada. Estos datos son muy importantes a la hora de generar una ruta adecuada. Además cuenta con botones para registrar semáforos audibles y otros elementos relativos la accesibilidad de un sitio.

| Ícono  | Texto del botón y punto en el gpx  | Descripción   | Esquema de mapeo sugerido en OSM   |
|--------|------------------------------------|---------------|------------------------------------|
|<img src="https://github.com/EmmanuelAB/Pruebas/blob/master/negros/ba%C3%B1os.png?raw=true" width="100" heigth="100" style="border: 2px solid black;">| Baños |Baños accesibles: sin gradas bruscas, puertas adecuadas, sanitarios espaciosos.|    Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg)`amenity=toilet wheelchair=yes `| 
|<img src="https://github.com/EmmanuelAB/Pruebas/blob/master/negros/rampa.png?raw=true" width="100" heigth="100">   | Rampa  | Rampa de acceso: para sillas de ruedas: ángulo menor a 45º, en buen estado y de un ancho suficiente.|Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `ramp:wheelchair=yes`|
|<img src="https://github.com/EmmanuelAB/Pruebas/blob/master/negros/obstaculo.png?raw=true" width="100" heigth="100">  | Obstáculo  | Obstáculo: cualquier tipo de obstáculo en una acera o zona de paso que dificulte o imposibilite el paso accesible.  | Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): ` barrier=chain barrier=cable_barrier  barrier=handrail barrier=kerb barrier=cattle_grid barrier=debris`[1]|
|<img src="https://github.com/EmmanuelAB/Pruebas/blob/master/negros/touch_inicio.png?raw=true" width="100" heigth="100">|  Acera Táctil Inicio | **Inicio** de una acera táctil.| Vía ![](https://wiki.openstreetmap.org/w/images/0/0f/Mf_area.svg): `tactile_paving=yes tactile_paving=incorrect` [2] |
|<img src="https://github.com/EmmanuelAB/Pruebas/blob/master/negros/touch_fin.png?raw=true" width="100" heigth="100">  |  Acera Táctil Fin | **Fin** de una acera táctil.  | Vía ![](https://wiki.openstreetmap.org/w/images/0/0f/Mf_area.svg): `tactile_paving=yes tactile_paving=incorrect` [2] |
|<img src="https://github.com/EmmanuelAB/Pruebas/blob/master/negros/semaforo.png?raw=true" width="100" heigth="100">| Semáforo aud  | Semáforo audible, con un nivel de sonido claro.|Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): ` crossing=traffic_signals  traffic_signals:sound=walk traffic_signals:sound=yes` |


**Aclaraciones**

[1] Al encontrar un nodo de tipo obstáculo, es necesario indicar que solo se debe utilizar una de las etiquetas ejemplificadas en la tabla.

[2] Al establecer un punto de inicio para una acera táctil, se debe establecer su punto de fin donde corresponda, las etiquetas mostradas son utilizadas para describir el estado de dicha acera.
