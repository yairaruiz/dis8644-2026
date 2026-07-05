# examen-grupo-01

## integrantes

- Benjamín Alonso Álvarez Pavez / [benjaminalvarez21](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/03-benjaminalvarez21>)
- Anays Valentina Cornejo Candia / [Anaysval](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/09-Anaysval>)
- Bruno Ferrari Meyer / [chknngttts](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/11-chknngttts>)
- Lucas Ignacio Ortiz Aguirre / [ryukivol](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/21-ryukivol>)
- Nicolás Elías Valdés Greve / [nicolasvaldesgreve](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/31-nicolasvaldesgreve>)

## criterios de diseño del sistema

### de donde partimos?

No teniamos conocimientro previo antes de entrar al taller, fue nuestra primera vez trabajando con y soldando componentes electronicos a placas. Aparte de las clases que dieron los profesores buscamos inspiración en paginas web como foros y canales de youtube que mostraban como hacer partes de sintetizadores (ej; filtros, amplificadores, reguladores etc...).

Todo este proceso ha sido prueba y error, si no funciona, se cambia y se vuelve a intentar. Gran parte de la ayuda fue entre compañeros, nos apoyamos para arreglar problemas comunes, compartíamos datos de lugares de compra y paginas web para buscar circuitos interesantes.

------------

## referentes

### white sample

artista chileno que usa sintetizadores analogicos

ha trabajado con lollapalooza con estructuras interactivas y ha tocado en eventos

su musica es experimental/electronica

![whitesample](./imagenes/whitesample.jpg) (cita)

-------------

### anthony1

dj/productor chileno

ha hecho tocatas ambientales donde utiliza sintetizadores analogicos y efectos digitales

forma parte de un colectivo de varios artistas electronicos chilenos (Team Mekano)

![anthony1](./imagenes/anthony1.png) (cita)

----------------

## disponibilidad material

en cuanto a la disponibilidad material en chile nos ubicamos principalmente en 2 lugares/tienda; "San Diego" y "Victronics". en San Diego se encuentran varias tiendas de electronicas que ofrecen distintos componentes, la gracia es los distintos lugares y sus especialidades.

"Victronics" es una tienda online, por eso pueden ofrecer precios más bajos, además tienen accesorios como espaciadores y pernos para armar las carcasas.

### BOM PCB MAINCRA

| Componente | Cantidad | PCB | Valor unitario | Link | ¿Hay stock en LID? |
| --- | --- | --- | --- | --- | --- |
| Chip NE555P | 1 | U1 | $490 | <https://www.victronics.cl/circuitos-integrados/lm555cngeneralpurposebipolartimerdip8/> | Sí |
| Chip TL072CP | 1 | U4 | $990 | <https://www.victronics.cl/circuitos-integrados/tl072cpdualjfetlowpoweropamplifierdip8/> | No |
| Regulador L7805CV | 1 | U3 | $350 | <https://www.victronics.cl/reguladores/reguladorvoltl7805cv5v-15ato220/> | No |
| Diodo 1N4007 | 1 | D5 | $200 | <https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/> | Sí |
| Diodo 1N5819 | 2 | D6, D7 | $586 | <https://cl.rsdelivers.com/product/nexperia/bat85113/nexperia-diodo-bat85113-diodo-schottky-200-ma-30-v/0300978> | No |
| Transistor 2N2222 | 1 | Q1 | $200 | <https://www.mechatronicstore.cl/transistor-2n2222/> | Sí |
| Potenciómetro B10K | 1 | RV1 | $495 | <https://altronics.cl/potenciometro-lineal-10k-b10k> | No |
| Potenciómetro B500K | 1 | RV2 | $495 | <https://altronics.cl/potenciometro-lineal-500k-b500k?search=b500k> | Sí |
| LED 3mm | 3 | D1, D2, D8 | $100 | <https://www.mechatronicstore.cl/led-3mm-5mm/> | Sí |
| Resistencia 47 Ω | 1 | R12 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | No |
| Resistencia 100 Ω | 1 | R18 |  $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 220 Ω | 1 | R14 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 1 KΩ | 6 | R1, R3, R6, R7, R8, R11 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 2,2 KΩ | 1 | R13 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | No |
| Resistencia 10 KΩ | 2 | R4, R5 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 100 KΩ | 3 | R2, R16, R17 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 2,2 MΩ | 1 | R15 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | No |
| Condensador cerámico 1 µF | 1 | C9 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | No |
| Condensador cerámico 4.7 nF | 1 | C12 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | No |
| Condensador cerámico 10 nF | 1 | C13 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | No |
| Condensador cerámico 100 nF | 3 | C1, C7, C10 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | Sí |
| Condensador polarizado 10 µF | 2 | C9, C11 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> | Sí |
| Condensador polarizado 100 µF | 3 | C2, C3, C5 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> | Sí |
| Piezo | 1 | J8 | $990 | <https://www.mechatronicstore.cl/sensor-piezoelectrico-27mm-con-cable/> | Sí |
| Cables dupont 40 uni. | 1 | - | $2.990 | <https://mcielectronics.cl/shop/product/cable-dupont-macho-macho-20cm-pack-40-unidades-2/> | Sí |
| Batería 9V recargable | 1 | BT1 | $7.990 | <https://www.sodimac.cl/sodimac-cl/articulo/110251085/bateria-recargable-9v/110251089> | Sí |
| Interruptor Switch | 1 | SW3 | $570 | <https://www.katode.cl/switches/1339-interruptor-switch-2-pines-on-off-corto.html?srsltid=AfmBOorJlIeUySzAORFwXSattHKE4BKH2LmhhXZS_8fZ4MW-G6kwnxqA> | No |

### BOM PCB 02, GRUPO 02: REGISTRO DE DESPLAZAMIENTO ESTÁTICO / NYAN CAT

| Componente | Cantidad | PCB | Valor unitario | Link | ¿Hay stock en LID? |
| --- | --- | --- | --- | --- | --- |
| Chip 4015 | 1 | U2 | $1.400 | <https://www.mactronica.com.co/cd4015?srsltid=AfmBOopMDQhFv0vy6tj-sATCKe9rcEpOGbsfz7VMFRrBPl9Yq3KS80wU> | No |
| Regulador L7805CV | 1 | U4 | $350 | <https://www.victronics.cl/reguladores/reguladorvoltl7805cv5v-15ato220/> | No |
| Transistor 2N2222 | 8 | Q3, Q4, Q5, Q6, Q7, Q8, Q9, Q10 | $220 | <https://www.cabezacuadrada.cl/product/pn2222a/> | Sí |
| Transistor BC548 | 1 | Q1 | $200 | <https://www.mechatronicstore.cl/transistor-bc548/?srsltid=AfmBOorIdGTZFY0mLCpBPP8JWl9WGDELQa-iZIZ95pKPjncWCgmXklr3> | No |
| LED 3mm | 9 | D1, D2, D3, D4, D5, D6, D7, D8, D12 | $100 | <https://www.mechatronicstore.cl/led-3mm-5mm/> | Sí |
| Resistencia 220 Ω | 8| R4, R5, R6, R7, R8, R9, R10, R11 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 1 KΩ | 18 | R3, R12, R15, R16, R17, R18, R19, R20, R21, R22, R23, R24, R25, R26, R27, R28, R29, R30 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 10 KΩ | 1 | R2 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 100 KΩ | 1 | R13 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Diodo 1N4007 | 1 | D11 | $200 | <https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/> | Sí |
| Condensador cerámico 100 nF | 1 | C9 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | Sí |
| Condensador polarizado 10 µF | 1 | C8 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> | Sí |
| Condensador polarizado 100 µF | 1 | C7 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> | Sí |
| Interruptor Switch | 1 | SW4 | $570 | <https://www.katode.cl/switches/1339-interruptor-switch-2-pines-on-off-corto.html?srsltid=AfmBOorJlIeUySzAORFwXSattHKE4BKH2LmhhXZS_8fZ4MW-G6kwnxqA> | No |

### BOM PCB 03, GRUPO 03: COMANDO ESTELAR

(hay q organizarlo aun)

| Componente | Cantidad | PCB | Valor unitario | Link | ¿Hay stock en LID? |
| --- | --- | --- | --- | --- | --- |
| Chip CD4046 | 1 | U1 | $700 | Electrónica Real | |
| Chip CD40106 | 1 | U4 | $1200 | Electrónica Real | |
| L7805 | 1 | U2 | $350 | Victronics | |
| Diodo 1N4007 | 1 | D1 | $790 | Victronics | |
| LED | 1 | D2 | $920 | Electrónica Real | |
| Resistencia 100kΩ | 1 | R1 | $890 | Electrónica Real | |
| Resistencia 1kΩ | 1 | R2 | $890 | Electrónica Real | |
| Potenciómetro 100Ω | 2 | RV1, RV2 | $500 | Afel a Ingeniería | |
| Capacitor 10nF | 1 | C1 | $520 | Victronics | |
| Capacitor 100nF | 1 | C5 | $500 | Victronics | |
| Capacitor 100uF | 2 | C2, C6 | $670 | Victronics | |
| Capacitor 10uF | 2 | C3, C4  | $330 | Victronics | |
| Capacitor 1uF | 1 | ?? | $300 | Victronics | |
| Jack DC | 2 | J2, J3 | $150 | Electrónica Real | |
| Jack de audio | 1 | J1 | $150-$300 | Victronics | |

Soldado 6 Horas

 Según yo esto no va

| Interruptor de palanca SPDT ON-ON | 1 | SW1 | $590 | Electrónica Real | |
| Separador o tornillo de montaje (M3*8) | 4 | 4 | $54 | Pernos Alameda | |
| Cable Dupont | 19 | 19 | $1190 (pack 10) | MCI Electronics | |

----------------

Fuerte arraigo con lo modular, desde un principio creamos sistemas modulares hasta llegar a estas distintas placas cada una con diferentes chips y componentes pero oara llegar al mismo fin, un sintetizador modular capaz de interconectarse con nuevas partes de nuestras placas realizadas

El diy vs eurorack, precios, diferencias
Ante la barrera del eurorack salen las placas mas diy (como las de este taller) ya que los componentes son baratos de conseguir, aqui el contexto chileno brillante por la necesidad y creatividad,
La existencia de iniciativas locales como talleres y la misma comunidad

Jose vicente asuar

nombre de sistema/instrumento construido por medio de módulos

??? AL FINAL PONER ESTO

----------------

## placas soldadas

principio de funcionamiento de cada una, qué tipo de señal entrega a la salida, qué recibe
lista de materiales con costos. Incluir tiempo de soldadura

Nuestro sintetizador está formado de 4 modulos:

> ## **maincra (Piezo/entrada)**
>
> *un microfono de contacto que detecta vibraciónes, manda señales a un amplificador e inversor de señales. estos convierten la corriente la cual entra a un reloj interno que lo camba a pasos para que un sequenciador pueda funcionar.*
>
> ## **nyan cat (Sequenciador)**
>
> *un sequenciador de 8 pasos (y dos fases) que permite la conexión de multiples osciladores.*
>
> ## **comando estelar (Oscilador)**
>
> *esta placa utiliza 2 chip para general oscilaciónes que alteran a traves de potenciómetros que permiten cambiar tanto la frecuencia como la modulación del sonido.*
>
> ## **parla (Amplificador/Salida)**
>
> *es un amplificador de señal que permite escuchar las oscilaciónes del modulo anterior con mayor volumen.*
>

-------------

## procesos

![test](./imagenes/procesos-largo.png)

![test gif-1](./imagenes/corte-laser-1.gif) ㅤㅤㅤㅤㅤㅤㅤ ![test gif-2](./imagenes/grito-test-medio.gif)

(MAS PROCESO ESCRITO)

> *para tener un flujo de trabajo más ordenado pusimos todos los conmponentes necesarios para armar una placa de lado.*
>
> *soldamos los componentes por tamaño (de más pequeño a más grande) y cables para los que van montados en la carcasa. al tener todo soldado en la placa se empezó a armar la cubierta de acrílico con los separadores, pusimos los potenciómetros, entradas/salidas de audio y switch conectados con los cables.*

----------------

## carcasa

decisiones materiales y formales de la carcasa
inspiración y referentes (con cita)

> *escogimos trabajar con acrilico ya que eramos familiares con el material. es fácil de trabajar por su compatibilidad con el corte laser que nos permitía cortar varias carcasas, grabar y lograr un buen oficio. el material es firme, perfecto para lo que teniamos en mente, además es economico.*
>
> *una cualidad del acrílico que utilizamos es la transparencia. buscamos celebrar el diseño de las PCB a través de la transparencia de este, rompiendo la caja negra e invitando a la apreciación integral de cada placa y sus distintos componentes.*

### referentes carcasa

> para la carcasa usamos estos 3 ejemplos:
>
> cmf phone - Nothing
>
> microKorg crystal - Korg
>
> gameboy transparente - Nintendo

![test](./imagenes/referencias-modulos.png)

(muy grande --> cambiar a 550px ancho / añadir citas)

## composición

### Referentes

- **Yoko Ono:**

> ### **"pieza de escondite"**
>
> *"esconderse hasta que todos se vayan a sus casas."*
>
> *"esconderse hasta que todos se olviden de uno."*
>
> *"esconderse hasta que todos todos se mueran"*
>

??? 1 MAS

#### Simbología

QUE ES ESTO LOL

---

#### Integración a la vida diaria

TERMINAR DE ESCRIBIR

Al hacer brainstorming de que podriamos hacer como partitura nos dimos cuenta que nuestras ideas eran actividades ????

---

#### Ping Pong

*(ver. literal examen 1) Como grupo-01 vamos a ir a República 180, Santiago de Chile con “maincra” (piezo-01), el parlante, “nyan cat” (secuenciador-2) y "comando estelar" (oscilador-1). Poner un piezo en cada lado superior de la mesa al centro, y pegarlo en la mesa con cinta adhesiva. Jugar una partida con paletas y pelota de Ping Pong que se piden donde los guardias. Con el impacto de la pelota en la mesa el secuenciador avanza, haciendo que el oscilador pueda funcionar. Jugar durante 5 minutos. Al perder, se cambian los jugadores. Al finalizar los 5 minutos se devuelven las paletas y pelota a los guardias.*

*(ver. literal 1) Como grupo-01 vamos a ir a República 180, Santiago de Chile con “maincra” (piezo-01), el parlante, RELO y “nyan cat” (secuenciador-2). Poner un piezo en cada lado superior de la mesa al centro, y pegarlo en la mesa con cinta adhesiva. Jugar una partida completa de Ping Pong de 21 puntos con las paletas y pelota que se piden con los guardias. Con el impacto de la pelota en la mesa el secuenciador avanza, haciendo que el oscilador pueda funcionar. Al terminar la partida devolver las paletas y pelota a los guardias.*

**(ver. literal 2) Como grupo-01 vamos a ir a República 180, Santiago de Chile con “maincra” (piezo-01), el parlante, “nyan cat” (secuenciador-2) y "comando estelar" (oscilador-1). Pedir las paletas y pelotas donde los guardias. Pondremos un piezo en cada paleta de ping pong con masking tape. Situar el sintetizador bajo la mesa, asegurar que los cables no se enreden entre sí. Jugar una partida completa de Ping Pong de 21 puntos, con el impacto de la pelota en las paletas el secuenciador avanza, haciendo que el oscilador pueda funcionar. Al terminar la partida devolver las paletas y pelota a los guardias.**

(ver. poética)

>**Ve a República 180 y ubica el piezo en la mesa de ping pong**

>**Invita a alguien a jugar**

>**Jueguen durante 5 minutos o hasta que se aburran**

## dificultades

- organización de compra de componentes
- tener los componentes a mano para soldar
- soldar los componentes en la dirección correcta
- corte laser de acrilico
  - archivos en formato correcto
- funcionamiento correcto de las PCB
  - conexiónes peculiares en la PCB

------------------



-----------------

## bibliografía

PEGAR DEL DOC YA ESTAN CASI TODAS
