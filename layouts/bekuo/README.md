# Disposición de botones Bëküo

Esta disposición de botones (DisBo) facilita la recolección de datos para mapear elementos de accesibilidad, hidrantes y movilidad. Esta DisBo ha sido creada por el grupo de investigación/extensión Bekuo del [Laboratorio Experimental](labexp.org) como parte de una [investigación sobre calidad de datos](https://github.com/labexp/pre-editor-osm). La DIsBo será utilizada en un ejercicio de mapeo en campo.  A continuación se ofrece una tabla que documenta los botones incluidos en la DisBo y su eventual uso al editar el mapa de Open Street Map (OSM).



| <img src="docu/bekuo1.jpg" style="zoom:25%;" /> | <img src="docu/bekuo2.jpg" style="zoom:25%;" /> | <img src="docu/bekuo3.jpg" style="zoom:25%;" /> |
| ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| DisBo de entrada                                | Hidrantes                                       | Movilidad.                                      |

La imagen de la izquierda es la DisBo de entrada, permite capturar elementos de accesibilidad y nos lleva a las otras dos pantallas: la de hidrantes y de movilidad. Estas últimas dos serán explicadas más abajo en este archivo.  

Las siguientes tablas pretenden guiar la asociación entre distintos tipos de elementos encontrados en el campo con las etiquetas a utilizar para describir los elementos en el mapa de OSM. La primera columna presenta el ícono que aparecen en la disposición de botones. La segunda y tercera columna describen con una imagen y texto las características de cada elemento para identificarlo en el campo mientras se capturan datos.  La cuarta columna indica el texto que aparecerá en el archivo en el punto del GPX  (*waypoint*) luego de presionar el botón. La última columna es una sugerencia de esquema de mapeo para incorporar los datos capturados a OSM.



## Entrada

| Ícono  |Ejemplo| Texto del punto en el GPX (waypoint)  | Descripción   | Esquema de mapeo sugerido en OSM   |
|--------|-------|---------------------------------------|---------------|------------------------------------|
|<img src="https://github.com/EmmanuelAB/Pruebas/blob/master/negros/obstaculo.png?raw=true" width="100" heigth="100">|<img src="https://www.jacksons-fencing.co.uk/-/media/jacksons-products/timber/footpath--row/5888.jpg?mh=460&mw=690&hash=29B1C023A25AE85F6CCC985590743B4133B42F4D" width="250" heigth="250"> | Obstáculo  | Cualquier tipo de obstáculo en una acera o zona de paso que dificulte o imposibilite el paso accesible.  | Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): ` barrier=chain` `barrier=cable_barrier` `barrier=handrail` `barrier=kerb` `barrier=cattle_grid` `barrier=debris`[1] |
|<img src="https://github.com/EmmanuelAB/Pruebas/blob/master/negros/semaforo.png?raw=true" width="100" heigth="100">|<img src="https://globalaccessibilitynews.com/files/2014/05/DSC_012.jpg" width="150" heigth="150">|  Semáforo audible  | Semáforo peatonal con un nivel de sonido claro. |Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): ` crossing=traffic_signals`  `traffic_signals:sound=walk` `traffic_signals:sound=yes` |



El esquema de mapeo sugerido está basado en las páginas Wiki:

*  [Key:barrier](https://wiki.openstreetmap.org/wiki/ES:Key:barrier).
* [crossing=traffic_signals](https://wiki.openstreetmap.org/wiki/ES:Tag:crossing%3Dtraffic_signals)

[1] Al encontrar un nodo de tipo obstáculo, es necesario indicar que solo se debe utilizar una de las etiquetas ejemplificadas en la tabla.



## Hidrantes


| Ícono                                                        | Ejemplo                                                      | Descripción                                                  | Texto del punto en el GPX (waypoint) | Esquema de mapeo sugerido en OSM                             |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------ | ------------------------------------------------------------ |
| (<u>Por hacer</u>: incluir ícono) Hidrante Seco              | ![](https://wiki.openstreetmap.org/w/images/thumb/3/33/Hydrants_20130326_112938.JPG/150px-Hydrants_20130326_112938.JPG) | También conocido como "hidrante seco", necesario una bomba.  | Hidrante Seco                        | Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `emergency=fire_hydrant` `fire_hydrant:type=pipe` |
| <img src="bekuo_icons/App-01.png" style="zoom:33%;background-color: gray;" /> Hidrante de Pilar | ![](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fd/Downtown_Charlottesville_fire_hydrant_1.jpg/150px-Downtown_Charlottesville_fire_hydrant_1.jpg) | Un hidrante de tipo pilar. Para información específica leer [`pillar:type=*`](https://wiki.openstreetmap.org/w/index.php?title=ES:Tag:emergency%3Dfire_hydrant#pillar:type.3D.2A) | Hidrante de Pilar                    | Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `emergency=fire_hydrant` `fire_hydrant:type=pillar` |
| <img src="bekuo_icons/App-02.png" style="zoom:33%;background-color: gray;" /> Hidrante de Pared | ![](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9b/Guentherscheid_Tunnel_Rescue4.jpg/225px-Guentherscheid_Tunnel_Rescue4.jpg) | Hidrante colocado en una pared.                              | Hidrante de Pared                    | Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `emergency=fire_hydrant` `fire_hydrant:type=wall` |
| (<u>Por hacer</u>: incluir ícono) Hidrante Subterráneo       | ![](https://upload.wikimedia.org/wikipedia/commons/thumb/6/65/Berlin_hydrant_20050211_p1000517.jpg/200px-Berlin_hydrant_20050211_p1000517.jpg) | El hidrantes está bajo tierra, es necesario un tubo vertical. | Hidrante Subterráneo                 | Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `emergency=fire_hydrant` `fire_hydrant:type=underground` |
| <img src="bekuo_icons/App-04.png" style="zoom:33%;background-color: gray;" />Otro tipo de hidrante (desconocido): |                                                              | Tipo de hidrante desconocido.                                | Hidrante Desconocido                 | Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `emergency=fire_hydrant` `fire_hydrant:type=unknown` |
| <img src="bekuo_icons/App-10.png" style="zoom:33%;background-color: gray;" /> Hidrante fuera de servicio. |                                                              | Se supone que los hidrantes están en funcionamiento de manera  predeterminada. En caso contrario, si el hidrante está fuera de  servicio, use esta etiqueta. | Hidrante fuera de servicio           | Nodo ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `disused:emergency=fire_hydrant` |

El esquema de mapeo sugerido está basado en la [wiki de la etiqueta `emergency=fire_hydrant`](https://wiki.openstreetmap.org/wiki/ES:Tag:emergency%3Dfire_hydrant).



## Movilidad



| Ícono                                                        | Ejemplo                                                      | Descripción                                                  | Texto del punto en GPX (waypoint) | esquema de mapeo sugerido en osm                             |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | --------------------------------- | ------------------------------------------------------------ |
| ![](https://camo.githubusercontent.com/c037fdcd7751c13affbe6f2fc6a0fb9cbd3ade654c01fafb8e9e4bcdcfdc3546/68747470733a2f2f696d6167652e6962622e636f2f696e316172472f626f746f6e5f312e706e67) | ![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/ParadaBusesB%C3%A1sica.jpg/225px-ParadaBusesB%C3%A1sica.jpg) | Este tipo de parada se identifica porque únicamente existe una raya amarilla en la calle (con las letras CTP pintadas). Esta raya está ubicada al lado de la acera en el sentido que circula el bus. | PARADA DE BUS - TIPO 1            | Nodo [![img](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667)](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667): `public_transport=platform` `bus=yes` |
| ![](https://camo.githubusercontent.com/e079ec224c2ebea9cf49d9002d867523b4ccf8bd8e9b384f30188e611f3d7cca/68747470733a2f2f696d6167652e6962622e636f2f6d68434335622f626f746f6e5f322e706e67) |                                                              | Además de la raya amarilla en la calle, esta parada tiene algún techo o casetilla. | PARADA DE BUS - TIPO 2            | Nodo [![img](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667)](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667): `public_transport=platform` `bus=yes` `shelter=yes` |
| ![](https://camo.githubusercontent.com/80a3ef4d120ac46de7c81daa0a2eac72ee4b8177aef59c74ebf8110d8e8aa9ac/68747470733a2f2f696d6167652e6962622e636f2f66506e5a4a772f626f746f6e5f332e706e67) | ![](https://wiki.openstreetmap.org/w/images/thumb/b/b7/San_isidro1.jpg/236px-San_isidro1.jpg) | Además de la raya amarilla en la calle y el techo, esta parada tiene una banca. | PARADA DE BUS - TIPO 3            | Nodo [![img](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667)](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667): `public_transport=platform` `bus=yes ` `shelter=yes` `bench=yes` |
| ![](https://camo.githubusercontent.com/2166c9027b14c53febd1b35ccf129117215e8f340f89d4d98be2d4e5eed73a7d/68747470733a2f2f696d6167652e6962622e636f2f6a43504835622f626f746f6e5f372e706e67) |                                                              | Punto de alquiler bicicletas (recoger y dejar).              | ALQUILER BICICLETAS               | Nodo [![img](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667)](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667): `amenity=bicycle_rental` |
| ![](https://camo.githubusercontent.com/489b7691939202a35b847ba29714b2290503e4623c84142e46f983c9bd58ae6e/68747470733a2f2f696d6167652e6962622e636f2f64534c654a772f626f746f6e5f352e706e67) |                                                              | Paradas de taxis                                             | TAXIS                             | Nodo [![img](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667)](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667): `amenity=taxi` |
| ![](https://camo.githubusercontent.com/2263aa62c489f13a7b85a700374249288ba1c3b51054d2d43634e8176337a1cb/68747470733a2f2f696d6167652e6962622e636f2f6b6542456b622f626f746f6e5f382e706e67) |                                                              | Estacionamiento de bicicletas                                | PARQUEO BICICLETA                 | Nodo [![img](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667)](https://camo.githubusercontent.com/bd6b1b568387ada2e14bf83490363ec7882dea8f5283efcbe3369bace8e87610/68747470733a2f2f77696b692e6f70656e7374726565746d61702e6f72672f772f696d616765732f322f32302f4d665f6e6f64652e737667): `amenity=bike_parking` |

El esquema de mapeo sugerido está basado en las páginas wiki:

* [Transporte Público](https://wiki.openstreetmap.org/wiki/Public_transport)
* [amenity=taxi](https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dtaxi)
* [amenity=bicycle_parking](https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dbicycle_parking)
* [amenity=bicycle_rental](https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dbicycle_rental).  

