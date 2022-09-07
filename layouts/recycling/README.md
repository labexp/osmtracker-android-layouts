# Disposición de botones de reciclaje y gestión de residuos sólidos

<!--
Una vez descargada la disposición de botones ser verá como la siguiente:

<img src="captura_pantalla.jpg" style="zoom: 50%;" />
-->

Estos son los botones y su descripción para tomar en terreno elementos asociados al reciclaje y la gestión de residuos sólidos (basuras). Igualmente indica cómo se deben mapear en OSM.

# Main page / Pantalla principal

| Icon / Ícono  | Example / Ejemplo  | Description / Descripción  | Text on the GPX point / Texto del punto en el GPX (waypoint)  | OSM mapping schema / Esquema de mapeo sugerido en OSM  |
| ------ | -------- | ------------ | ------------------------------------- | --------------------------------- |
| Page / página ![Canecas](recycling_icons/waste_basket.png) | ![Caneca](https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/Vuilnisbak-Lebbeke.JPG/179px-Vuilnisbak-Lebbeke.JPG)  | Waste basket / Caneca  | - | - |
| ![Distribuidor de bolsas](recycling_icons/dog_excrement_bag_vending.png) | ![Distribuidor de bolsas](https://wiki.openstreetmap.org/w/images/8/8c/Dog_excrement_bags.jpg) | Place with available bags for pickup and collection of animal waste. / Distribuidor de bolsas para excrementos de perros | Vending excrement bags / Distribuidor de bolsas | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `vending=excrement_bags` |
| Page / página ![Contenedor de reciclaje](recycling_icons/container.png) | ![Contenedor de reciclaje](https://wiki.openstreetmap.org/w/images/8/80/Altglas.jpg) | Recycling container / Contenedor de reciclaje |  | - | - |
| ![Contenedor para camión de basuras](recycling_icons/waste_disposal.png) | ![Contenedor para camión de basuras](https://wiki.openstreetmap.org/w/images/6/6b/Waste_container.jpg) | Waste disposal is used for medium and large waste bins, typically for bagged up household or industrial waste. They may be in the street, but they are not primarily for use by passing pedestrians. / Contenedor para camión de basuras | Waste container / Contenedor para camión de basuras | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=waste_disposal` |
| - | ![Centro de reciclaje](https://wiki.openstreetmap.org/w/images/c/c2/WertstoffhofWeitnau.jpg) | These centres are dedicated areas for collecting a wider range of recyclable household materials / Centro de reciclaje | Recycling center / Centro de reciclaje | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=centre` |
| - | ![Centro de acopio](https://upload.wikimedia.org/wikipedia/commons/0/00/Ingram_Transfer_Station_-_Toronto_-_2019_-_02.jpg) | A waste transfer station is a location that accepts, consolidates and transfers waste in bulk, usually from government or commercial collections. / Centro de acopio | Waste transfer station / Centro de acopio | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=waste_transfer_station` |
| -| ![Relleno](https://upload.wikimedia.org/wikipedia/commons/a/ac/Landfill_Hawaii.jpg) | A site for permanent or long term storage of waste materials / Relleno | Landfill / Relleno | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `landuse=landfill` |
| - | ![PTAR](https://upload.wikimedia.org/wikipedia/commons/4/48/Klaerwerk_Buelk_nahe_Kiel.jpg) | A wastewater plant (also known as sewage works, sewage treatment plant, wastewater treatment plant, reclamation plant) is a facility used to treat wastewater / PTAR | Wastewater plant / PTAR | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `man_made=wastewater_plant` |

# Bins / Canecas

| Icon / Ícono  | Example / Ejemplo  | Description / Descripción  | Text on the GPX point / Texto del punto en el GPX (waypoint)  | OSM mapping schema / Esquema de mapeo sugerido en OSM  |
| ------ | -------- | ------------ | ------------------------------------- | --------------------------------- |
| ![Caneca para basuras](recycling_icons/waste_basket.png) | ![Caneca para basuras](https://upload.wikimedia.org/wikipedia/commons/6/62/Vuilnisbak-Lebbeke.JPG) | A waste basket is a single small container for depositing garbage that is easily accessible for pedestrians. / Caneca para basuras | Trash / Caneca para basuras | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=waste_basket` |
| ![Caneca sobre poste](recycling_icons/bin_on_lamp.png) | ![Caneca sobre poste](https://upload.wikimedia.org/wikipedia/commons/9/9f/Silberner_M%C3%BClleimer_Bushaltestelle_Hardenbergstra%C3%9Fe_Kiel-Bl%C3%BCcherplatz.jpg) | Bin on streetlamp / Caneca sobre poste | Bin on streetlamp / Caneca sobre poste | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg), way ![](https://wiki.openstreetmap.org/w/images/2/2a/Mf_way.svg), area ![](https://wiki.openstreetmap.org/w/images/0/0f/Mf_area.svg): (`bench=*`, `shelter=*`, `public_transport=platform`) + `bin=yes` |
| ![Caneca para desecho de animal](recycling_icons/dog_excrement.png) | ![Caneca para desecho de animal](https://wiki.openstreetmap.org/w/images/8/84/Dog_waste_bin.jpg) | Dog excrement bin / Caneca para desecho de animal | Dog excrement bin / Caneca para desecho de animal | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=waste_basket` + `waste=dog_excrement` |
| ![Caneca para cigarrillos](recycling_icons/cigarretes_basket.png) | ![Caneca para cigarrillos](https://upload.wikimedia.org/wikipedia/commons/a/ab/Cigarette_waste_bin%2C_Oude_Pekela_%282019%29_01.jpg) | Cigarettes bin / Caneca para cigarrillos | Cigarettes bin / Caneca para cigarrillos | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=waste_basket` + `waste=cigarettes` |

# Recycling containers / Contenedores de reciclaje

| Icon / Ícono  | Example / Ejemplo  | Description / Descripción  | Text on the GPX point / Texto del punto en el GPX (waypoint)  | OSM mapping schema / Esquema de mapeo sugerido en OSM  |
| ------ | -------- | ------------ | ------------------------------------- | --------------------------------- |
| Page / página | - | Plastic/Batteries/Oil / Plástico/Baterías/Aceite |  |  |
| - | ![Papel](https://upload.wikimedia.org/wikipedia/commons/5/59/Pekelder_paper_recycling_container.jpg) | Paper / Papel | Paper / Papel | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + (`recycling:paper` or `recycling:cardboard` or `recycling:cartons` or `recycling:paper_packaging` or `recycling:magazines` or `recycling:newspapers`) |
| ![Vidrio](recycling_icons/glass.png) | ![Vidrio](https://upload.wikimedia.org/wikipedia/commons/2/2e/Glass_recycling_container%2C_Barendrecht_%282020%29_03.jpg) | Glass / Vidrio | Glass / Vidrio | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:glass_bottles` or `recycling:glass_bottles:colour` |
| Page / página  | ![Eléctricos/Electrónicos](https://upload.wikimedia.org/wikipedia/commons/c/c6/Handy_schrott_mobile_phone_scrap.jpg) | Electrical/Electronics / Eléctricos/Electrónicos |  |  |
| ![Llantas](recycling_icons/tyres.png) | ![Llantas](https://upload.wikimedia.org/wikipedia/commons/8/81/Tyres_in_the_recycling_shed_at_Greenhead_landfill_site%2C_Lerwick_-_geograph.org.uk_-_1905862.jpg) | Tyres / Llantas | Tyres / Llantas | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:tyres` |
| ![Medicinas](recycling_icons/drugs.png) | ![Medicinas](https://upload.wikimedia.org/wikipedia/commons/a/a4/Drug_disposal_receptacle.jpg) | Drugs / Medicinas | Drugs / Medicinas | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:drugs` |
| - | ![Compostaje](https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/Prospect_Av_Greenwood_Av_td_%282019-09-16%29_05_-_Compost_Bins.jpg/320px-Prospect_Av_Greenwood_Av_td_%282019-09-16%29_05_-_Compost_Bins.jpg) | Compost / Compostaje | Compost / Compostaje | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:green_waste` |

# Plastic-Batteries-Oil / Plásticos-baterías-aceite

| Icon / Ícono  | Example / Ejemplo  | Description / Descripción  | Text on the GPX point / Texto del punto en el GPX (waypoint)  | OSM mapping schema / Esquema de mapeo sugerido en OSM  |
| ------ | -------- | ------------ | ------------------------------------- | --------------------------------- |
| - | ![Plástico general](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9b/Jerusalem_Musrara_Shivtei_Israel_street_plastic_bottles_recycling.jpg/320px-Jerusalem_Musrara_Shivtei_Israel_street_plastic_bottles_recycling.jpg) | All plastic / Plástico general | All plastic / Plástico general | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + (`recycling:plastic` or `recycling:plastic_bags` or `recycling:plastic_bottles` or `recycling:plastic_packaging`) |
| - | - | Polystyrene foam / Icopor / poliestireno | Polystyrene foam / Icopor / poliestireno | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:polystyrene_foam` |
| ![Tapas de botellas](recycling_icons/plastic_bottle_cap.png) | ![Tapas de botellas](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6f/Bottle_Cap_Recycling_%2819740699084%29.jpg/320px-Bottle_Cap_Recycling_%2819740699084%29.jpg) | Plastic bottle caps / Tapas de botellas | Plastic bottle caps / Tapas de botellas | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:plastic_bottle_caps` |
| ![Baterías y pilas](recycling_icons/battery.png) | ![Baterías y pilas](https://upload.wikimedia.org/wikipedia/commons/a/a3/Vigo_-_reciclaje_de_residuos_urbanos_01.jpg) | Batteries / Baterías y pilas | Batteries / Baterías y pilas | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:batteries` |
| ![Baterías de carro](recycling_icons/car_battery.png) | ![Baterías de carro](https://upload.wikimedia.org/wikipedia/commons/thumb/4/49/Diamond_Energie_car_battery.jpg/310px-Diamond_Energie_car_battery.jpg) | Car batteries / Baterías de carro | Car batteries / Baterías de carro | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:car_batteries` |
| ![Aceite de cocina](recycling_icons/cooking_oil.png) | ![Aceite de cocina](https://upload.wikimedia.org/wikipedia/commons/b/b9/Alicante_-_Reciclaje_de_residuos_urbanos_03.jpg) | Cooking oil / Aceite de cocina | Cooking oil / Aceite de cocina | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:cooking_oil` |
| ![Aceite de carro](recycling_icons/engine_oil.png) | ![Aceite de carro](https://upload.wikimedia.org/wikipedia/commons/b/bb/Mobil_1_motor_oil.jpg) | Engine oil / Aceite de carro | Engine oil / Aceite de carro | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:engine_oil` |

# Electric and electronics / Eléctricos y electrónicos

| Icon / Ícono  | Example / Ejemplo  | Description / Descripción  | Text on the GPX point / Texto del punto en el GPX (waypoint)  | OSM mapping schema / Esquema de mapeo sugerido en OSM  |
| ------ | -------- | ------------ | ------------------------------------- | --------------------------------- |
| ![Computadores](recycling_icons/computers.png) | ![Computadores](https://upload.wikimedia.org/wikipedia/commons/a/a5/TV_and_Computer_Monitor_Recycling_Pen_-_geograph.org.uk_-_1025508.jpg) | Computers / Computadores | Computers / Computadores | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:computers` |
| ![Celulares](recycling_icons/mobile_phone.png) | ![Celulares](https://upload.wikimedia.org/wikipedia/commons/4/4d/Telenor_mobile_recycling_innsamling4.JPG) | Mobile phones / Celulares | Mobile phones / Celulares | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + `recycling:mobile_phones` |
| - | ![Electrónicos](https://upload.wikimedia.org/wikipedia/commons/c/c6/Waste_electrical_c.png) | Electronics / Electrónicos | Electronics / Electrónicos | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + (`recycling:small_electrical_appliances` or `recycling:small_appliances` or `recycling:electrical_appliances` or `recycling:electrical_items` or `recycling:electronics`) |
| <img src="recycling_icons/bulb.png" style="zoom:33%;background-color: gray;" /> | - | Bulbs / Bombillos | Bulbs / Bombillos | Node ![](https://wiki.openstreetmap.org/w/images/2/20/Mf_node.svg): `amenity=recycling` + `recycling_type=container` + (`recycling:light_bulbs` or `recycling:low_energy_bulbs` or `recycling:fluorescent_tubes`) |



