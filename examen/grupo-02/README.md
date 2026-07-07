# examen-grupo-02

## integrantes

- Isidora Alvarez / [isidoraalvarez](https://github.com/isidoraalvarez/dis8644-2026-1)
- Dayana Pañitrur / [dayanapanitrur](https://github.com/dayanapanitrur/dis8644-2026-1)
- Camila Ramírez / [Estrabismx](https://github.com/Estrabismx/dis8644-2026-1)
- Angel Sabogal / [angel-udp](https://github.com/angel-udp/dis8644-2026-1)
- Tomas Catrileo / [tomascatri](https://github.com/tomascatri/dis8644-2026-1)

## Proyecto

Este proyecto consiste en el diseño y construcción de un instrumento musical interactivo compuesto por siete módulos electrónicos que trabajan de forma coordinada. Cada uno cumple una función distinta y, al prenderse, permiten generar ritmos, sonidos y composiciones musicales que pueden modificarse en tiempo real.

El objetivo fue transformar un conjunto de módulos desarrollados por distintos grupos en un único instrumento funcional. Además de integrar todas las partes del sistema, buscamos crear una forma de interacción con la iluminacion, reemplazando las perillas tradicionales por sensores de luz. De esta manera, el sonido puede controlarse mediante gestos, haciendo que la interpretación sea más expresiva.

Para lograrlo construimos y conectamos todos los módulos, definiendo la forma en que se comunican entre sí para coordinar la generación de ritmos y sonidos. También adaptamos los controles para incorporar sensores de luz e integramos todas las salidas de audio en un único sistema de reproducción. Durante el desarrollo resolvimos distintos desafíos de integración y funcionamiento hasta obtener un instrumento estable y completamente operativo.

## Referentes

| Enlace | Imagen |
|--------|--------|
| [https://www.lovehulten.com/](https://www.lovehulten.com/) | ![Imagen](./imagenes/love-hulten-00.jpg) |
| [My First Modular by Oficina de Sonido](https://www.kickstarter.com/projects/oficinadesonido/1007031649) | ![Imagen](./imagenes/oficina-sonido.jpg) |
| [https://github.com/misaaaaaa/ritmo_etc](https://github.com/misaaaaaa/ritmo_etc) | ![Imagen](./imagenes/ritmo-etc.jpg) |
| [https://www.morelmusiq.de/news-horizon-1-1](https://www.morelmusiq.de/news-horizon-1-1) | ![Imagen](./imagenes/morelmusiq.jpg) |
| [https://proyectosonec.org/artista/monica-bate/](https://proyectosonec.org/artista/monica-bate/) | ![Imagen](./imagenes/monica-bate.jpg) |
| [https://uchile.cl/noticias/202394/en-atenas-se-presentaran-obras-del-nucleo-sonoro-del-dav](https://uchile.cl/noticias/202394/en-atenas-se-presentaran-obras-del-nucleo-sonoro-del-dav) | ![Imagen](./imagenes/dav.jpg) |
| [https://uchile.cl/noticias/223150/discom-tr-de-lucas-soffia-arte-sonido-y-experimentacion-mecanica](https://uchile.cl/noticias/223150/discom-tr-de-lucas-soffia-arte-sonido-y-experimentacion-mecanica) | ![Imagen](./imagenes/lucas-soffia.jpg) |


## Cultura de los sintetizadores en Chile

La cultura de los sintetizadores en Chile ha crecido gracias al trabajo de músicos, diseñadores, ingenieros y artistas que desarrollan proyectos relacionado a esto. A pesar de que el país no cuenta con grandes empresas dedicadas a fabricar sintetizadores, existe una comunidad que diseña, construye y modifica sus propios instrumentos, especialmente en el ámbito de sintetizadores modulares y la electrónica experimental.

Igualmente, los sintetizadores también son usados para el aprendizaje y experimentación; es de lo más normal encontrar por ahí talleres, charlas, exposiciones y encuentros. Inclusive en la misma UDP se dan estos espacios de creación y de enseñanza sobre electrónica, programación y diseño de instrumentos musicales, fomentando el intercambio de conocimientos entre las comunidades.

En Chile hay nuevas iniciativas como **GC Lab Chile**, que enseña a construir sintetizadores y otros dispositivos electrónicos; también existe **Orion Network**, que difunde proyectos y actividades relacionadas con la música electrónica y la tecnología sonora; y artistas como **Polwor**, quienes demuestran cómo los sintetizadores pueden utilizarse para crear nuevas experiencias musicales.

Gracias a este cúmulo de cosas, la comunidad de sintetizadores albergada en territorio chileno sigue creciendo y promoviendo la innovación, la fabricación local y el desarrollo de nuevas propuestas que combinan música, diseño y tecnología.



## Placas usadas

| Placas    | Categoría       | Diseñada por | Imagen                           |
| :-------- | :---------------| :----------- | :------------------------------- |
| 01        | **RELO** (Reloj) | Docentes     | ![Placa01](./imagenes/relo.jpeg) |
| 02        | **secuenciador binario** (Secuenciador 02) | Grupo 02     | ![Placa02](./imagenes/secuenciado-binario-gr-02.jpeg)  |
| 03        | Chirihue Mecanizado (Oscilador 01)    | Grupo 04     | ![Placa05](./imagenes/chirihue-gr-04.jpeg) |
| 04        | **Barry Benson** (Percusión 02)    | Grupo 06     | ![Placa07](./imagenes/barry-benson-gr-03.jpeg) |
| 05        | **Comunicaciones espaciales** (Oscilador 02) | Grupo 04     | ![placa06](./imagenes/comunicaciones-especiales-gr-04.jpeg) |
| 06        | **Comando Estelar** (Oscilador 01)    | Grupo 03     | ![Placa03](./imagenes/comando-estelar-gr-03.jpeg)  |
| 07        | **Resonancia** (Oscilador 02)    | Grupo 03     | ![Placa04](./imagenes/resonancia-gr-03.jpeg) |

<br>

## Explicación de flujo de señal de audio:

ordenado a grandes rasgos: gesto humano a fuentes de tiempo, a secuenciador, a osciladores, a filtros, a mezcladores, a parlante.

- La placa 01 corresponde al reloj. Desde ella salen dos señales hacia la placa 02 secuenciador: una entrega el voltaje de alimentación y la otra envía la señal de reloj (clock), que proporciona los pulsos necesarios para el conteo binario del secuenciador. 
- La placa 02 corresponde al secuenciador. Alimentado por el reloj, utiliza la señal de clock para realizar un conteo binario, avanzando un paso con cada pulso recibido. A partir de este conteo, sus salidas generan las señales de control que se distribuyen hacia los cuatro osciladores y la placa de percusión. Una de las salidas se deja sin conexión para incorporar un paso de silencio dentro de la secuencia.

- Las placas: 03, 04, 05, 06 y 07 corresponden a fuentes sonoras, reemplazamos todas las conexiones que correspondían a potenciómetros por LDR para regular de forma gestual con luz los parámetros del sonido de cada una de las placas.

- La salida tanto de los cuatro osciladores como del percutor es audio que va a la siguiente placa de amplificador o amplificador comercial, lo cuál está aún en veremos debido a dudas sobre el funcionamiento de parla (placa docentes).
**Arquitectura general del sistema:**
 
```
Usuario
   │
   ▼
Sensores de luz (LDR)
   │
   ▼
Reloj
   │
   ▼
Secuenciador
   │
   ├────────► Oscilador 1
   ├────────► Oscilador 2
   ├────────► Oscilador 3
   ├────────► Oscilador 4
   └────────► Percusión
                     │
                     ▼
                   Mixer
                     │
                     ▼
               Amplificador
                     │
                     ▼
                  Parlante
```

<br>

## Estado de construcción (6 de Julio)

| Placas    | Categoría       | Diseñada por | Estado de construcción          |
| :-------- | :-------------- | :----------- | :------------------------------ |
| 01        | **Relo** (Reloj)           | Docentes     | Funcional                       |
| 02        | **Secuenciador binario** (Secuenciador 02) | Grupo 02     | Funciona, pero estamos revisando la interconexión con otras PCB mediante el uso de relés |
| 03        | **Barry Benson** (Percusión 02)    | Grupo 06     | Funciona individualmente / Se deben cambiar conectores adaptados para la carcasa |
| 04        | **Chirigüe mecanizado** (Oscilador 01)    | Grupo 04     | Funciona individualmente / Se deben cambiar conectores adaptados para la carcasa |
| 05        | **Comunicaciones espaciales** (Oscilador 02)    | Grupo 04     | Funciona individualmente / Se deben cambiar conectores adaptados para la carcasa |
| 06        | **Comando estelar** (Oscilador 01)    | Grupo 03     | Funciona individualmente / Se deben cambiar conectores adaptados para la carcasa |
| 07        | **Resonancia** (Oscilador 02)    | Grupo 03     | Funciona individualmente / Se deben cambiar conectores adaptados para la carcasa |

<br>

## Resolucion de problemas

Como en cualquier proyecto de electrónica y en la vida, durante el proceso aparecieron varios problemas que tuvimos que ir resolviendo sobre la marcha. Algunos fueron fallas de componentes, otros de conexiones y varios surgieron al integrar todas las placas en un solo sistema. A continuación se muestran los principales problemas que enfrentamos y cómo los solucionamos:

<br>



**Problema 1**

Queríamos utilizar relés para conectar el secuenciador con los osciladores y la placa de percusión.

Tras conversar con Misaa y revisar el funcionamiento del circuito, entendimos que la forma correcta de conectar los osciladores al secuenciador era mediante relés que actuaran como interruptores, encendiendo y apagando cada placa cuando el secuenciador lo indicara. Después de varios intentos, logramos hacer funcionar este sistema agregando un transistor **2N2222A**, que permitía aumentar el voltaje de salida de cada _step_ desde **4 V** hasta **9 V**.

Posteriormente, consultamos a Aaron para verificar si las conexiones estaban correctamente realizadas y si era posible optimizar y estandarizar el montaje de los relés y transistores.

**Resolución**

Aaron confirmó que el circuito estaba correctamente conectado y que no presentaba problemas de funcionamiento. Sin embargo, recomendó mejorar el orden y la seguridad del montaje utilizando una placa de soldadura punto a punto, con el objetivo de organizar mejor las conexiones y reducir la cantidad de cables sueltos.

Intentamos implementar esta solución, pero durante el montaje en la PCB de prototipado se produjeron falsos contactos que impedían el funcionamiento correcto del circuito. Por este motivo, decidimos volver a la configuración inicial, utilizando relés y transistores independientes, pero mejorando el aislamiento con cinta aislante y replicando esta solución en cada _step_.

---

**Problema 2**

La placa **Chirigüe mecanizado** presentaba un volumen considerablemente menor al esperado.

**Resolución**

A pesar de realizar distintas pruebas e intentos de reparación, no fue posible solucionar el problema. Concluimos que se trata de una falla interna de la placa.

---

**Problema 3**

El parlante producía una cantidad importante de estática durante su funcionamiento.

**Resolución**

Identificamos que el parlante estaba configurado para una entrada estéreo, mientras que nuestra salida de audio era mono. Esta incompatibilidad generaba la estática observada. Al utilizar un sistema de amplificación compatible con una señal mono, el problema quedó resuelto.

---

**Problema 4**

Necesitábamos conectar la salida de audio de todos los osciladores y la placa de percusión a un mezclador de audio.

**Resolución**

Utilizamos un **mixer** facilitado por el Laboratorio de Interacciones Digitales, lo que permitió integrar correctamente todas las salidas de audio del sistema.

---

**Problema 5**

Necesitábamos comprobar si la placa **Parla** funcionaba correctamente o si era necesario utilizar otro amplificador.

**Resolución**

Finalmente utilizamos un amplificador proporcionado por el Laboratorio de Interacciones Digitales, el cual cumplió correctamente la función de amplificación del sistema.

---

**Problema 6**

Problemas de conexiones constantes, los cable que usamos en su mayoria ocurrian problemas debio a que o se cortaban o causaban falso contacto

**Resolucion**

Reforzamos las conexiones soldando cable a cable con estaño y reemplazando los cables dañados por conectores Dupont macho adaptados.

**Problema 7**

Placa Relo dejo de funcionar, ya no prendian los LEDs y no mandaba señal a las otras placas.

**Resolucion**

A pesar de diagnosticar y ver que todo se encontraba en buen estado, seguia sin funcionar, por lo que dimos por muerta la placa y la replicamos en otra placa Relo que habia, luego de cambiarla funciono.

**Problema 8**
No encontrábamos cables compatibles para conectar el amplificador, el parlante y el mixer. Los conectores tenían distintos tamaños, por lo que necesitábamos cables con adaptadores específicos.
**Resolucion**
Decidimos usar cables caimán para unir las distintas conexiones. La conexión quedó de la siguiente forma: 
```
Cable pequeño → Caimán sujetando ambos extremos → Cable grande → Amplificador
```
Con esta solución logramos conectar correctamente todos los dispositivos y el sistema funcionó sin problemas.

<br>

---


## Criterios de diseño del sistema

### Inspiración para construir


El desarrollo del sistema se inspiró en proyectos de Misaa que exploran la creación de instrumentos electrónicos modulares y experimentales.

- **ritmo_etc** fue un referente por su uso de circuitos CMOS para la generación de sonido y secuenciación, demostrando que es posible construir sintetizadores experimentales mediante electrónica accesible.

- **22machines** fue el principal referente para la arquitectura del sistema. Este proyecto propone un conjunto de módulos independientes que cumplen funciones específicas y trabajan de manera coordinada. Además, plantea una alternativa latinoamericana al formato Eurorack, utilizando componentes disponibles en Santiago de Chile y privilegiando la fabricación local.

Como referencia para la interacción, también se consideró **Botanika**, proyecto que utiliza sensores para transformar fenómenos físicos en sonido. Esta idea inspiró el uso de sensores LDR en nuestro instrumento, permitiendo controlar distintos parámetros mediante la luz en lugar de potenciómetros tradicionales.

---

### Contexto desde Chile y disponibilidad material

El sistema fue construido considerando la disponibilidad de componentes electrónicos presentes en el mercado nacional. Se utilizaron circuitos integrados CMOS, componentes discretos y materiales de fácil acceso, permitiendo fabricar el instrumento sin depender de piezas especializadas difíciles de conseguir.

Este enfoque sigue la filosofía presentada en **22machines**, priorizando la accesibilidad, la modularidad y la posibilidad de replicar el proyecto utilizando recursos disponibles en Chile.

---

### Sistema modular interno

Nuestro instrumento está compuesto por siete módulos electrónicos independientes que trabajan de forma coordinada:

- Reloj
- Secuenciador
- Cuatro osciladores
- Módulo de percusión

Cada módulo cumple una función específica dentro del sistema. El reloj genera el pulso principal, el secuenciador organiza el ritmo y activa los distintos módulos, mientras que los osciladores y la percusión producen el sonido. Finalmente, todas las señales son mezcladas y amplificadas para obtener una única salida de audio.

Esta estructura modular facilita la comprensión del funcionamiento del instrumento, permite reemplazar o modificar módulos individuales y hace posible futuras ampliaciones del sistema.

## Constructivo

| Enlace | Imagen |
|--------|--------|
| [Orchid – Love Hultén](https://www.lovehulten.com/orchid) | ![Imagen](./imagenes/orchid.jpg) |
| [Ryk – Love Hultén](https://www.lovehulten.com/ryk) | ![Imagen](./imagenes/ryk.jpg) |
| [https://www.yankodesign.com/2023/01/24/this-strange-looking-plant-box-uses-science-to-create-eerie-music/](https://www.yankodesign.com/2023/01/24/this-strange-looking-plant-box-uses-science-to-create-eerie-music/) | ![Imagen](./imagenes/yankodesign.jpg) |
| [https://www.matrixsynth.com/2013/04/folktek-feedscape-one-of-kind-hand-made.html?m=1](https://www.matrixsynth.com/2013/04/folktek-feedscape-one-of-kind-hand-made.html?m=1) | ![Imagen](./imagenes/folktek-feedscape.jpg) |

## placas soldadas

Reloj / Docentes: *Relo* 

**Principio de funcionamiento:** Recibe la corriente inicial y permite iniciar el parpadeo del reloj, el cual conduce a una salida de corriente que transfiere los datos de la oscilación y corriente constante para alimentar todo lo subsiguiente.

Secuenciador 01 / Grupo 2: *Secuenciador 4040*

**Principio de funcionamiento:** Recibe pulsos del reloj y, con cada uno, avanza un paso en un conteo binario. Sus salidas cambian siguiendo esa secuencia, permitiendo activar los distintos módulos en un orden determinado y controlar el ritmo del sintetizador. 

Oscilador 01 / Grupo 03: *Comando estelar*

**Principio de funcionamiento:** Genera un sonido cuya frecuencia cambia según el voltaje que recibe. Esto permite modificar el tono del sintetizador de forma continua mediante potenciómetros o señales de control.
 
Oscilador 02 / Grupo 03: *Resonancia*

**Principio de funcionamiento:** Genera un sonido cuya frecuencia puede variar y, al mismo tiempo, usa un secuenciador para activar diferentes pasos en orden. Así crea patrones y cambios de sonido de forma automática.

Oscilador 01 / Grupo 04: *Chirigüe mecanizado*

**Principio de funcionamiento:** Genera sonidos con un oscilador y modifica su tono mediante el circuito, permitiendo obtener diferentes efectos sonoros. 

Oscilador 02 / Grupo 04: *Comunicaciones espaciales*

**Principio de funcionamiento:** Genera una señal de sonido de forma continua y permite cambiar su tono mediante los potenciómetros, creando diferentes efectos y variaciones sonoras. 

Percusión 02 / Grupo 06: *Barry Benson*

**Principio de funcionamiento:** Genera sonidos de percusión al recibir una señal de activación. Sus controles permiten modificar el tono y el carácter del sonido para obtener diferentes tipos de golpes. 

## Tiempo de soldadura

| Proceso | Integrantes | Duración | Horas por integrante | Total equipo |
|----------|:-----------:|:--------:|----------------------:|-------------:|
| Soldadura, corrección de errores y soluciones de todas las PCB | 5 | 3 semanas | 120 hrs | 120 hrs × 5 = 600 h |

## BOM (Bill Of Materials)

### Reloj

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C polarizado   | 47µF   |  1   | C1          |
| C polarizado   | 100µF  | 1    | C2          | 
| C polarizado   | 10µF   | 1    | C4          |
| C polarizado   | 220µF  | 1    | C5          |
| Capacitor      | 100nF  | 2    | C3 C6       |
| LED            | -----  | 2    | D2 D3       |
| Diodo          | 1N4007 | 1    | D1          |
| Resistencia    | 1kΩ    | 4    | R1 R2 R3 R4 |
| LDR            | ------ | 1    | RV1         | 
| Switch         | SPDT   | 1    |  SW1        |
| Chip           | 555    | 1    | U1          |
| Chip           | L7805  | 1    | U2          |
| Base Dip       | 8 pin  | 1    | U1          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J1 J2       |
| Conector       | Jack   | 1    | J3          |

<br>

### Secuenciador 1 / Grupo 02

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C polarizado   | 100µF  |  1   | C4          |
| C polarizado   | 10µF   | 1    | C5          |
| Capacitor      | 100nF  | 1    | C6          |
| Led            |        | 7    | D8 D9 D10 D11 D12 D13 D14 |
| Diodo          | 1N4007 | 1    | D6          |
| Transistor     | 2N2222 | 6    | Q1 Q2 Q3 Q4 Q5 Q6 |
| Resistencia    | 1KΩ    | 19   | R7 R8 R9 R10 R11 R12 R13 R14 R15 R16 R17 R18 R19 R21 R22 R23 R24 R25 R26 |
| Resistencia    | 100KΩ  | 1    | R20         |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 4040   | 1    | U2          |
| Chip           | L7805  | 1    | U4          |
| Base Dip       | 16 pin | 1    | U2          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J2 J3       |
| Conector       | Jack   | 8    | J6 J7 J8 J9 10 J11 J12 |

<br>

### Oscilador 01 / Grupo 03

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| Capacitor      | 10nF   | 1    | C1          |
| Capacitor      | 100nF  | 1    | C5          |
| C. polarizado  | 100µF  | 3    | C2 C6 C7    |
| C. polarizado  | 10µF   | 2    | C3 C4       |
| Diodo          | 1N4007 | 1    | D1          |
| LED            | ------ | 1    | D2          |
| Resistencia    | 100KΩ  | 1    | R1          |
| Resistencia    | 1KΩ    | 1    | R2          |
| LDR            | ------ | 2    | RV1 RV2     |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 4046   | 1    | U1          |
| Chip           | L7805  | 1    | U2          |
| Chip           | 40106  | 1    | U3          |
| Base Dip       | 16 pin | 1    | U1          |
| Base Dip       | 14 pin | 1    | U3          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J2 J3       |
| Conector       | Jack   | 1    | J1          |

<br>

### Oscilador 02 / Grupo 03

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| Capacitor      | 1µF    | 2    | C2 C7       |
| C. polarizado  | 4µF    | 1    | C3          |
| C. polarizado  | 100µF  | 1    | C4          |
| C. polarizado  | 10µF   | 2    | C5 C8       |
| Capacitor      | 100nF  | 1    | C6          |
| Led            | -----  | 2    | D1 D3       |
| Diodo          | 1N4007 | 1    | D2          |
| Resistencia    | 470KΩ  | 2    | R1 R2       |
| Resistencia    | 330KΩ  | 1    | R3          |
| Resistencia    | 1KΩ    | 1    | R4          |
| LDR            | ------ | 2    | RV1 RV2     |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 4017   | 1    | U1          |
| Chip           | 4046   | 1    | U2          |
| Chip           | 40106  | 1    | U3          |
| Chip           | L7805  | 1    | U4          |
| Base Dip       | 16 pin | 2    | U1 U2       |
| Base Dip       | 14 pin | 1    | U3          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J1 J3       |
| Conector       | Jack   | 1    | J4          |

<br>

### Oscilador 01 / Grupo 04

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C. polarizado  | 10µF   | 3    | C2 C3 C10   |
| Capacitor      | 100nF  | 2    | C4 C11      |
| C. polarizado  | 100µF  | 1    | C9          |
| Diodo          | 1N4007 | 1    | D1          |
| LED            | -----  | 1    | D2 D8       |  
| Diodo          | 1N4148 | 4    | D3 D4 D5 D6 |
| Resistencia    | 1KΩ    | 7    | R2 R3 R4 R5 R6 R7 R8 |
| LDR            |        | 4    | RV1 RV2 RV3 RV4 |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 40106  | 1    | U1          |
| Chip           | L7805  | 1    | U2          |
| Chip           | LM324  | 1    | U3          |
| Base Dip       | 14 pin | 2    | U1 U3       |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J1 J3       |
| Conector       | Jack   | 1    | J4          |

<br>

### Oscilador 02/ Grupo 04

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C. polarizado  | 1µF    | 3    | C1 C2       |
| C. polarizado  | 10µF   | 2    | C3 C5       |
| C. polarizado  | 100µF  | 1    | C4          |
| Capacitor      | 100nF  | 1    | C6          |
| Diodo          | 1N4148 | 1    | D1          |
| Diodo          | 1N4007 | 1    | D2          |
| LED            | ------ | 1    | D8          |
| Resistencia    | 1KΩ    | 3    | R1 R2 R9    |
| LDR            |        | 2    | RV1 RV2     |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 40106  | 1    | U1          |
| Chip           | L7805  | 1    | U5          |
| Base Dip       | 14 pin | 1    | U1          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J1 J3       |
| Conector       | Jack   | 1    | J4          |

<br>

### Percusión 02 / Grupo 06

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C. polarizado  | 10µF   | 3    | C1 C4 C6    |
| C. polarizado  | 100µF  | 2    | C2 C5       |
| C. polarizado  | 1µF    | 1    | C3          |
| Capacitor      | 100nF  | 1    | C7          |
| Diodo          | 1N4007 | 1    | D1          |
| Led            |        | 2    | D8 D9       |
| Resistencia    | 1KΩ    | 2    | R4 R5       |
| LDR            |        | 4    | RV1 RV2 RV3 RV4 |
| Switch         | SPDT   | 1    | SW3         |
| Chip           | 40106  | 1    | U1          |
| Chip           | L7805  | 1    | U8          |
| Chip           | 4070   | 1    | U9          |
| Base Dip       | 14 pin | 2    | U1 U9       |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J2 J3       |
| Conector       | Jack   | 1    | J4          |


## BOM General

| Componente | Valor | Cantidad | Valor Unitario | Valor Total |
|------------|-------|---------:|---------------:|------------:|
| Capacitor Polarizado | 220µF | 1 | 100 | 100 |
| Capacitor Polarizado | 100µF | 9 | 100 | 900 |
| Capacitor Polarizado | 47µF | 1 | 100 | 100 |
| Capacitor Polarizado | 10µF | 14 | 100 | 1400 |
| Capacitor Polarizado | 4µF | 1 | 100 | 100 |
| Capacitor Polarizado | 1µF | 4 | 100 | 400 |
| Capacitor Polarizado | 0.22µF | 3 | 100 | 300 |
| Capacitor | 1µF | 2 | 740 | 1480 |
| Capacitor | 100nF | 10 | 100 | 1000 |
| Capacitor | 10nF | 1 | 100 | 100 |
| Diodo | 1N4007 | 7 | 200 | 1400 |
| Diodo | 1N4148 | 5 | 120 | 600 |
| LED | - | 16 | 100 | 1600 |
| LDR | - | 15 | 990 | 14850 |
| Resistencia | 220Ω | 10 | 100 | 1000 |
| Resistencia | 1kΩ | 37 | 100 | 3700 |
| Resistencia | 100kΩ | 2 | 100 | 200 |
| Resistencia | 330kΩ | 1 | 100 | 100 |
| Resistencia | 470kΩ | 2 | 100 | 200 |
| Transistor | 2N2222 | 13 | 390 | 5070 |
| Switch | SPDT | 7 | 300 | 2100 |
| Chip | NE555 | 1 | 490 | 490 |
| Chip | CD4017 | 1 | 890 | 890 |
| Chip | CD40106 | 5 | 750 | 3750 |
| Chip | CD4040 | 1 | 390 | 390 |
| Chip | CD4046 | 2 | 700 | 1400 |
| Chip | CD4070 | 1 | 2080 | 2080 |
| Chip | LM324 | 1 | 590 | 590 |
| Regulador de Voltaje | L7805 | 7 | 490 | 3430 |
| Base DIP | 8 pines | 1 | 450 | 450 |
| Base DIP | 14 pines | 6 | 600 | 3600 |
| Base DIP | 16 pines | 4 | 640 | 2560 |
| Conector | Barrel | 14 | 150 | 2100 |
| Conector | Jack | 14 | 180 | 2520 |
| Perno | M3 | 28 | 39,9 | 1117,2 |
| **TOTAL GENERAL** |  |  |  | **$61.597** |

<br>

### Costos finales

| Categoria   | Costo    |
| ----------- | -------- |
| Componentes | $61.597  |
| Materiales  | $31.590  |
| PCB         | $3.089   | 
| Hora humana | $400.000 |
| **Total**   | 493.190  |

---

## Carcasa

Nuestra carcasa consta de 2 estructuras principales, una interna que soporta las PCB y sus conexiones modulares, además de una externa que encapsula todo lo anterior. 


### Materialidad

| Material / Proveedor | Imagen |
|----------------------|--------|
| [Acrilico](https://www.acryl.cl/) | ![Imagen](./imagenes/acryl.jpg) |
|[ Terciado eucaliptus rosado 3 mm 1.44 × 2.20 m ](https://www.imperial.cl/terciados/terciado-eucaliptus-rosado-3mm-144x220mt/product/104758)| ![Imagen](./imagenes/terciado-eucalipto.jpg) |
| [Filamento PLA Gris](https://www.todotoner.cl/impresoras/impresoras-3d/filamentos/pla-gris-1kg-todotoner)  \| TodoToner.cl | ![Imagen](./imagenes/pla-gris.jpg) |

Los materiales vistos en la tabla se utlizaron porque responden a una desición de diseño importante. **La rapidez de fabricación**. Esto se debe a la cantidad de horas que requiere la construcción de los módulos (algo que se puede apreciar en la tabla que contabiliza la cantidad de horas)

Para enfocarnos en lo anterior mencionado, se prefirió optimizar procesos y por ende se opto por la fabricación digital. Sumado a esto se consideró que las piezas a utilizar tambien deberían funcionar bajo la lógica modular

Esto significó tener las piezas necesarias para la carcasa en menos de 3 horas. Lo que obviamento nos ayudó a dedicarle más tiempo a la fabricación de nuestro sintetizador




---

## Proceso

| Proceso 1 | Proceso 2 | Proceso 3 | Proceso 4 |
|-----------|-----------|-----------|-----------|
| ![Proceso01](./imagenes/pr-01.jpeg) | ![Proceso02](./imagenes/pr-02.jpeg) | ![Proceso03](./imagenes/pr-03.jpeg) | ![Proceso04](./imagenes/pr-04.jpeg) |

| Proceso 5 | Proceso 6 | Proceso 7 | Proceso 8 |
|-----------|-----------|-----------|-----------|
| ![Proceso05](./imagenes/pr-05.jpeg) | ![Proceso06](./imagenes/pr-06.jpeg) | ![Proceso07](./imagenes/pr-07.jpeg) | ![Proceso08](./imagenes/pr-08.jpeg) |

| Proceso 9 | Proceso 10 | Proceso 11 | Proceso 12 |
|-----------|------------|------------|------------|
| ![Proceso09](./imagenes/pr-09.jpeg) | ![Proceso10](./imagenes/pr-10.jpeg) | ![Proceso11](./imagenes/pr-11.jpeg) | ![Proceso12](./imagenes/pr-12.jpeg) |

| Proceso 13 | Proceso 14 | Proceso 15 | Proceso 16 |
|------------|------------|------------|------------|
| ![Proceso13](./imagenes/pr-13.jpeg) | ![Proceso14](./imagenes/pr-14.jpeg) | ![Proceso15](./imagenes/pr-15.jpeg) | ![Proceso16](./imagenes/pr-16.jpeg) |

| Proceso 17 | Proceso 18 | Proceso 19 | Proceso 20 |
|------------|------------|------------|------------|
| ![Proceso17](./imagenes/pr-17.jpeg) | ![Proceso18](./imagenes/pr-18.jpeg) | ![Proceso19](./imagenes/pr-19.jpeg) | ![Proceso20](./imagenes/pr-20.jpeg) |

| Proceso 21 | Proceso 22 | Proceso 23 | Proceso 24 |
|------------|------------|------------|------------|
| ![Proceso21](./imagenes/pr-21.jpeg) | ![Proceso22](./imagenes/pr-22.jpeg) | ![Proceso23](./imagenes/pr-23.jpeg) | ![Proceso24](./imagenes/pr-24.jpeg) |

| Proceso 25 | Proceso 26 | Proceso 27 | Proceso 24 |
|------------|------------|------------|------------|
| ![Proceso25](./imagenes/pr-25.jpeg) | ![Proceso26](./imagenes/pr-26.jpeg) | ![Proceso27](./imagenes/pr-27.jpeg) |![Proceso28](./imagenes/pr-28.jpeg) |


---


| Video 1 | Video 2 | Video 3 |
|:-------:|:-------:|:-------:|
| [![Video 1](https://img.youtube.com/vi/JmE9NbwjoMs/hqdefault.jpg)](https://youtube.com/shorts/JmE9NbwjoMs) | [![Video 2](https://img.youtube.com/vi/Sk7TLUBUIL0/hqdefault.jpg)](https://youtube.com/shorts/Sk7TLUBUIL0) | [![Video 3](https://img.youtube.com/vi/-w2bnB7ahFI/hqdefault.jpg)](https://youtube.com/shorts/-w2bnB7ahFI) |
| **Video 4** | **Video 5** | **Video 6** |
| [![Video 4](https://img.youtube.com/vi/Z8LjF2_bu-w/hqdefault.jpg)](https://youtube.com/shorts/Z8LjF2_bu-w) | [![Video 5](https://img.youtube.com/vi/l9U1S9-KGVk/hqdefault.jpg)](https://youtube.com/shorts/l9U1S9-KGVk) | [![Video 6](https://img.youtube.com/vi/rXEYtkrxyr4/hqdefault.jpg)](https://youtube.com/shorts/rXEYtkrxyr4) |
| **Video 7** | **Video 8** | **Video 9** |
| [![Video 7](https://img.youtube.com/vi/mTNN9lAFyIs/hqdefault.jpg)](https://youtube.com/shorts/mTNN9lAFyIs) | [![Video 8](https://img.youtube.com/vi/chz79BSDsxw/hqdefault.jpg)](https://youtube.com/shorts/chz79BSDsxw) | [![Video 9](https://img.youtube.com/vi/vpFVOLXRS30/hqdefault.jpg)](https://youtube.com/shorts/vpFVOLXRS30) |
| **Video 10** | **Video 11** | **Video 12** |
| [![Video 10](https://img.youtube.com/vi/bo8u3_Ju_fE/hqdefault.jpg)](https://youtube.com/shorts/bo8u3_Ju_fE) | [![Video 11](https://img.youtube.com/vi/CvPNiDL23gA/hqdefault.jpg)](https://youtube.com/shorts/CvPNiDL23gA) | [![Video 12](https://img.youtube.com/vi/T8TXoX9cu-E/hqdefault.jpg)](https://youtube.com/shorts/T8TXoX9cu-E) |

---

## composición

### Contexto

Al desarrollar este sintetizador nos percatamos que ocurrian muchas situaciones que afectan el flujo de trabajo, esto nos hizo cuestionarnos como el ambiente influye en el proceso de creación. Por lo que durante diversas conversaciones nació la idea de que este sintetizador generara su sónido en base a cada entonrno, nunca se podría replicar el mismo resultado. Finalmente esto es algo único, que tambien notamos en el proceso de fabricación de PCB, hacer algo de la misma manera no te asegura tener el mismo resultado, siempre hay elementos fuera de tu poder que interfieren en el desarrollo

### Referente

Estas partituras no solo se basaron en el trabajo de Yoko Ono con Grapefruit, sino que además nos basamos en el texto de Pauline Oliveros, Sonic Meditations. Ambos utilizan poesia para poder expresar y representar situaciones que se relacionan al sonido, algo más allá de la música convencional. Esto se relaciona directamente con el sentido del sintetizador, el cual no busca manipularse para generar música convencional, sino que hacer ruido que se relaciona directamente con el ambiente.

La idea de traer de vuelta la conciencia de los sentidos, desde el encuentro entre el ambiente, el sintetizador y los intérpretes, ha sido algo con lo que hemos querido trabajar, con el concepto de la “Escucha profunda”, de Pauline Oliveros que es un conjunto de meditaciones a través del sonido. nos ayudaron a recrear lo que se quería lograr con estas partituras, ya sea en solitario como en grupo. Cada una de las partes de la partitura va tomando una idea, que puede ser material o no, a lo que se le puede prestar atención, aunque sea un día, aunque sean 5 minutos.

### Partitura 

*"Para esta partitura se consideran 5 roles, en el que cada uno posee su propia partitura"*

1. Tiempo

Amanece para el dispositivo

Se le hace tarde al dispositivo

Corre y corre

...

Camina y camina

Observa su entorno

Tiene miedo

...

Se acabó 

¿Se acabó?

A dormir

<br>

2. Entorno

Se abre el telón

Los reflectores se encienden

Los nervios aparecen

...

Se cierra el telón

Queda gente

Menos gente

¿vuelven?

...

Toca limpiar

Toca ordenar

Toca cerrar


<br>

3. Volumen 

Hay que escalar

Hay que seguir el sendero

Todo difuso

... 

No queda nadie

Hay eco

¿o es alguien más?

...

Reencuentro

Descanso

Retomar recorrido

<br>

4. Experiencia 

30 ojos

No todos abiertos

Tiene sueño

...

Algo brilla

Desaparece

Se acerca veloz

...

Quedas bizco

Observas 

Analizas

<br>

5. Curiosidad

¿Se puede comer?

¿A que huele?

¿Habla mi idioma?

...

¿Es amigable?

¿Es solitario?

¿Se aburre?

...

¿Piensa?

¿Vuela?

¿?

<br>

### Simbología

Para entender la partitura, debemos entender que estas 5 aventuras tienen duraciones independientes, cada una puede tener más de un protagonista, además de que poseen 3 actos

La idea es que las personajes encuentren y junten sus historias, además de que pueden haber 2 personas siguiendo la misma partitura en el mismo momento, además estas aventuras pueden repetirse infinitamente

Los puntos suspensivos buscan separar cada partitura en 3 espacios, donde realizar algún cambio de rol o inluso abandonarlo, acá la interpretación es totalmente libre 



---

## bibliografía

- Abingraf. (s. f.). Acrílico MGRAF blanco fundido 3 mm liner plástico 1.22 × 2.44 mts. <https://abingraf.cl/collections/planchas-de-acrilico/products/acrilico-mgraf-blanco-fundido-3-mm-liner-plastico-1-22-x-2-44-mts>
- Acryl. (s. f.). Acryl. <https://www.acryl.cl/>
- GC Lab. (s. f.). GC Lab. <https://gclab.cl/>
- Kickstarter. (s. f.). My First Modular. <https://www.kickstarter.com/projects/oficinadesonido/my-first-modular>
- Love Hultén. (s. f.). Love Hultén. <https://www.lovehulten.com/>
- Maderas Imperio. (s. f.). Terciado eucaliptus rosado 3 mm 144 × 220. <https://maderasimperio.cl/producto/terciado-eucaliptus-rosado-3-mm-144x220/>
- Maker Faire Santiago. (s. f.). Pablo Palominos. <https://makerfairesantiagodotcom1.wordpress.com/participantes/expositores-nacionales/pablo-palominos/>
- Matrixsynth. (2013, abril). Folktek Feedscape – One of a Kind Hand Made. <https://www.matrixsynth.com/2013/04/folktek-feedscape-one-of-kind-hand-made.html?m=1>
- Proyecto SONEC. (s. f.). Mónica Bate. <https://proyectosonec.org/artista/monica-bate/>
- Pueblo Nuevo. (s. f.). Polwor. <https://pueblonuevo.cl/bios/polwor/>
- SCD. (s. f.). Originario SCD. <https://orionnetwork.cl/originario-scd/>
- TodoToner. (s. f.). Filamento PLA gris 1 kg. <https://www.todotoner.cl/filamento-pla-gris-1kg-tod>
- Universidad de Chile. (s. f.). DISCOM_TR de Lucas Soffia: arte, sonido y experimentación mecánica. <https://uchile.cl/noticias/223150/discom-tr-de-lucas-soffia-arte-sonido-y-experimentacion-mecanica>
- Universidad de Chile. (s. f.). En Atenas se presentarán obras del Núcleo Sonoro del DAV. <https://uchile.cl/noticias/202394/en-atenas-se-presentaran-obras-del-nucleo-sonoro-del-dav>
- Yanko Design. (2023, 24 de enero). This strange-looking plant box uses science to create eerie music. <https://www.yankodesign.com/2023/01/24/this-strange-looking-plant-box-uses-science-to-create-eerie-music/>


