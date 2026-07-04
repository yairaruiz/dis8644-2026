# examen-grupo-06

## Integrantes

- Catalina Catalán / [06-terroiblea](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/06-terroiblea)
- Martina Echavarría / [10-martinaechavarria-stack](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/10-martinaechavarria-stack)
- Nicolás Miranda / [18-Nicolas-Miranda1312](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/18-Nicolas-Miranda1312)
- Vania paredes / [24-paredesvania](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/24-paredesvania)
- Carla Pino / [25-coff4](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/25-Coff4)

## Problemas 04.07

Nosotros hemos tenido varios problemas con las pcb, de los cuales ya logramos resolver muchos coon ayuda de nuestros compañeres (sobre todo Cami Ramirez) y mucha prueba y error, ahora mismo ya nos funciona Barry Benson, ludup nos funciona a medias, funciona pero en una cierta posición, creímos que era la soldadura pero se reforzó y seguía igual o peor, creemos ahora que pueden ser unos cables, por lo que mañana los cambiaremos y veremos si se soluciona. Respecto a la tercera placa que queríamos utilizar, la del Chirihue, no  os funciona, prendía la luz pero no oscilaba ni sonaba, mucho estrés, no logramos hacerla funcionar y nos rendimos, por lo que tenemos pensado en armar el circuito en protoboard para ver si nos funciona, si es así, luego soldarlo en una placa verde para soldar y presentarlo de esa manera. Estos problemas han hecho que no podamos avanzar con nuestra carcasa ya que esta depende de cuantas placas y potenciometros usaremos, por lo que nos ha atrasado ;(

## Biofonía

> “Lo que late, lo que vuela, lo que canta”

![biofonia](./imagenes/biofonia.png)

### ¿Qué es Biofonía?

La biofonía es el conjunto de sonidos emitidos por los seres vivos en su hábitat natural. Estos sonidos son producidos tanto por grupos de animales como por individuos aislados, y en conjunto crean una sinfonía característica de cada lugar. Es un término clave en la ecología acústica (Paisajes Sonoros, s.f.).

Biofonía, el sintetizador, es una reinterpretación artificial de ese concepto: tres módulos que imitan procesos biológicos (un latido, un zumbido, un canto) sin ser vivos. Suena a naturaleza. No lo es.

## Criterios de diseño del sistema

Biofonía nació como una coincidencia, durante el desarrollo de los circuitos, nos dimos cuenta de que dos de las placas que habíamos construido sonaban, sin haberlo planeado, como seres vivos. Cuando apareció un tercer módulo capaz de imitar el canto de un pájaro, dejamos de ver tres circuitos independientes y empezamos a ver un mismo sistema.

A partir de esa coincidencia surgió la pregunta que dio forma al proyecto: si tenemos lo que late, lo que vuela y lo que canta, ¿dónde viven? La respuesta fue imaginar un ecosistema propio. No uno natural, sino uno construido con cobre, silicio y componentes electrónicos. Un jardín artificial donde cada módulo representa una forma distinta de vida y donde las flores no son flores, sino interfaces de control que permiten modificar el comportamiento sonoro de cada criatura.

El concepto de biofonía apareció después, al intentar nombrar ese paisaje. En ecología acústica, la biofonía corresponde al conjunto de sonidos producidos por los seres vivos de un ecosistema. Nuestro instrumento no busca una imitación perfecta; el interés está precisamente en esa distancia entre lo vivo y lo electrónico, donde un circuito puede recordar a un insecto, un corazón o un ave sin dejar de evidenciar que es una máquina.

Esta lógica también definió las decisiones materiales y técnicas del proyecto. Biofonía fue posible gracias al contexto actual de acceso abierto a información y documentación en internet. En lugar de diseñar los circuitos desde cero, pudimos investigar referentes existentes, analizar sintetizadores DIY y placas ya desarrolladas por la comunidad, comprender sus principios de funcionamiento y adaptarlos a nuestro proyecto. Esa disponibilidad de conocimiento permitió centrar el proceso en reinterpretar y combinar módulos ya probados para construir un sistema con una identidad propia. Del mismo modo, la elección de componentes respondió a la disponibilidad del contexto chileno, privilegiando piezas de fácil acceso en tiendas nacionales de electrónica, haciendo que el instrumento no sólo fuera reproducible, sino también reparable y replicable por otras personas. 

### Usuario

Biofonía es para quien escucha el mundo con atención. Para quien alguna vez se quedó parado escuchando el sonido de un transformador eléctrico en la calle y pensó que era interesante. Para quien no necesita que un sonido sea bonito para que le importe.

No tiene un perfil fijo. Puede venir de la música, del diseño, de la biología, o de ningún lugar en particular. Lo que tiene en común con cualquier otro usuario de Biofonía es que le interesa hacer cosas, entender cómo funcionan, y que no le asusta que el resultado sea raro.

Le atrae la idea de que un circuito pueda imitar algo vivo. Le atrae más todavía que no lo logré del todo, y que en esa distancia entre la naturaleza y la máquina viva algo interesante.

Biofonía es para esa persona; la que escucha la diferencia entre un zumbido y otro, y quiere saber de dónde viene.

## Partes de Bíofonia 

### Placa 01:  Barry Benson (percutor)

Barry Benson no es una abeja. Es peor que una abeja, es una abeja con complejos, quiere ser una mosca. Tiene la capacidad sobreinsectoide de reproducir exactamente ese sonido de mosca agonizante atrapada entre tu oreja y la almohada a las 3 de la madrugada. Es la representación en silicio de ese sonido, Barry Benson pega zumbidos. Un zumbido ondulante que sube y baja de intensidad como si el insecto se acercara y alejara de tu oído a voluntad propia. La ciencia no puede explicar del todo por qué suena exactamente así. Nosotros tampoco. Pero lo hace.

#### ¿Qué hace Barry Benson por ti?

- Reproduce con fidelidad perturbadora el sonido de un insecto atrapado entre tu oreja y la almohada.
- Permite ajustar el zumbido con cuatro potenciómetros para encontrar el tono exacto que más molesta a tu compañero de pieza.
- Según investigaciones del prestigioso Instituto de Zumbidología Aplicada de Concepción, la exposición prenatal al sonido de Barry Benson produce niños con oído absoluto y una relación complicada con los insectos.
- Suena como bzzzZZZzzzbzzZZZZzbzz. Como si alguien hubiera atrapado una abeja en un sintetizador analógico y ninguno de los dos estuviera contento con la situación.

#### Funcionamiento

Barry Benson recibe 12V por un jack de alimentación, que el circuito reduce internamente a 5V usando un regulador L7805. Su único output es una señal de audio por un jack estéreo.

Cuando alguien usa Barry Benson, interactúa con cuatro potenciómetros. Cada uno controla la frecuencia de un oscilador independiente, en otras palabras, es básicamente qué tan rápido vibra cada "ala" de la abeja. El chip que hace posible todo esto es el 40106, que contiene seis inversores Schmitt-trigger, componentes que deciden cuándo una señal es alta o baja, produciendo oscilaciones estables. Las cuatro señales resultantes se mezclan a través de compuertas XOR del chip 4070. Una XOR produce señal sólo cuando sus entradas son distintas, así que al combinar frecuencias similares pero no idénticas, la salida fluctúa a una velocidad igual a la diferencia entre ambas. Ese fenómeno es lo que hace que el volumen suba y baje de forma orgánica y le da a Barry ese carácter de insecto vivo que ningún presente de sintetizador ha logrado replicar con tanta dignidad.

![barry benson](./imagenes/abeja.png)

![barry benson](./imagenes/abeja-esquematico.png)

### Placa 02: Lub-dub (percutor)

Lub-dub hace exactamente lo que hace un corazón: bombea. Pero en vez de bombear sangre, bombea pulsos eléctricos. En vez de mantener vivo a un organismo, mantiene vivo el ritmo. Lub-dub late. A veces Tac. Tac. Tac. Otras, Dumb. Dumb. Dumb. Con la misma indiferencia biológica con que tu corazón te despertó esta mañana, Lub-dub bombea energía guiada por un compás. Es un percutor. Es un metrónomo pero con actitud.

#### ¿Qué hace Lub-dub por ti?

- Permite ajustar el tempo y el carácter del golpe, desde un latido tranquilo de persona en reposo hasta los 180bpm de alguien que acaba de ver su nota de taller.
- Es clínicamente superior a un metrónomo porque suena cool y los metrónomos no.
- Científicos del Instituto Cardiovascular de Sonidos Raros han determinado que escuchar Lub-dub mientras estudias mejora la concentración en un 340%. Este dato no ha sido verificado.
  
#### Funcionamiento

Lub-dub recibe 12V por un jack de alimentación, regulados internamente a 5V con un L7805. Su output es una señal de audio por un jack estéreo. Tiene cuatro potenciómetros que en conjunto controlan el tempo y el carácter del golpe.

El corazón del circuito es un oscilador construido con inversores Schmitt-trigger de los chips 40106 y 4069UBE. Un condensador se carga y descarga continuamente a través de resistencias variables: los potenciómetros cambian esas resistencias, lo que cambia qué tan rápido se carga el condensador y por lo tanto qué tan rápido late y cómo suena ese latido. La ventaja del Schmitt-trigger es que conmuta en voltajes distintos al subir y al bajar, lo que produce ese golpe brusco y limpio en vez de una transición suave. Antes de llegar al output, la señal pasa por una red de condensadores y resistencias que recorta el pulso y lo convierte en un impulso corto y acentuado. Ese recorte es lo que transforma la oscilación en un tac o un dumb dependiendo de cómo estén ajustados los potenciómetros.

![Lub dub](./imagenes/corazon.png)

![Lub dub](./imagenes/corazon-esquematico.png)

### Placa 03: Chirihue Mecanizado (oscilador)

Inspirada en la canción *La Exiliada del Sur* de Inti-Illimani (compuesta a partir de un poema de Violeta Parra), se rescata el siguiente fragmento: 

```
"Desembarcando en Riñihue
Se vio la Violeta Parra
Sin cuerdas en la guitarra
Sin hojas en el coligüe
Una banda de chirigües
Le vino a dar un concierto"
```

El Chirihue Mecanizado no es un pájaro. Es la interpretación en cobre y silicio de uno. Lleva su nombre por el chirihue real, ese pájaro que repite sonidos cortos y agudos de manera continua, oscilando en tono y ritmo. El apellido "Mecanizado" es una confesión honesta: esto no es naturaleza, es naturaleza reinterpretada por una máquina que nunca ha visto un árbol.

#### ¿Qué hace el Chirihue Mecanizado por ti?

- Produce ese sonido agudo, corto y repetitivo que hace que la gente pregunte si hay un pájaro en la sala.
- Permite ajustar el tono y el ritmo del canto con sus perillas, desde un trino tranquilo hasta algo que suena a alarma de incendio con opiniones propias.
- Incluye control de ataque y decaimiento: el chirihue puede aparecer suavemente o llegar de golpe, y desvanecerse con el
egancia o cortarse sin aviso como cualquier ser vivo.
- Según la prestigiosa Sociedad Ornitológica de Sonidos Raros de Valdivia, escuchar al Chirihue Mecanizado en ayunas mejora el sentido de la orientación en un 280%. Este dato tampoco ha sido verificado.
- Suena como: tiiit-tiiit-tiiit-tiiit. Pero sintético. Como si Violeta Parra hubiera compuesto para un microcontrolador. 

#### Funcionamiento

El Chirihue Mecanizado recibe 9V por un jack de alimentación y entrega su output como señal de audio. Tiene cinco potenciómetros: dos controlan la frecuencia del oscilador (el tono del canto), dos controlan el ataque y el decaimiento de la señal, y uno controla el volumen de salida.

El corazón del circuito es el chip CD40106, un inversor Schmitt-trigger que genera una oscilación continua cargando y descargando un condensador a través de resistencias variables. Los diodos D3 y D4 separan los caminos de carga y descarga del condensador, lo que permite que los potenciómetros RV2 y RV3 controlan la frecuencia de forma independiente: girar una perilla cambia el tono del canto. La señal resultante es una onda cuadrada que, al pasar por la segunda etapa del circuito formada por los diodos D5 y D6, los potenciómetros RV4 y RV5 y el condensador C3, adquiere un comportamiento de ataque y decaimiento: el sonido aparece progresivamente y se desvanece hasta el silencio, lo que le da ese carácter orgánico de nota que nace y muere. Finalmente, la señal pasa por el chip LM324 funcionando como seguidor de voltaje, que estabiliza la señal antes de enviarla al output sin alterar su forma, entregando un sonido limpio y estable hacia el resto del sistema.

![Chirihue](./imagenes/pajaro.png)

![Chirihue](./imagenes/pajaro-esquematico.png)

### Mixer 

![mixer](./imagenes/mixer.jpg)

<https://diystrat.blogspot.com/2008/08/two-channel-mini-mixer.html> 

### Placa 04: Amplificador/salida 

Parla  

![parla](./imagenes/parla.png)

![parla](./imagenes/parla-esquematico.png)

### Diagrama unión y esquemático 

![diagrama](./imagenes/diagrama.png)

![esquematico](./imagenes/esquematico.png)

### BOM

| Componente                      | Cantidad  | Valor unitario  | Link compra                                                                                           |
|---------------------------------|-----------|-----------------|-------------------------------------------------------------------------------------------------------|
| Placa Barry Benson              | 1         | -               | -                                                                                                     |
| Placa Lub-dub                   | 1         | -               | -                                                                                                     |
| Placa Chirihue Mecanizado       | 1         | -               | -                                                                                                     |
| Chip 4069UBE                    | 1         | $1.100          | <https://www.cabezacuadrada.cl/product/cd4069/>                                                       |
| Chip CD40106BE                  | 3         | $750            | <https://www.cabezacuadrada.cl/product/cd40106be/>                                                    |
| Chip CD4070BE                   | 1         | $2.080          | <https://www.maspotencia.cl/circuito-integrado-cd4070be-14-pines>                                     |
| Chip LM324                      | 1         | $590            | <https://www.mechatronicstore.cl/amplificador-operacional-lm324/>                                     |
| Potenciometro 100K              | 8         | $490            | <https://www.mechatronicstore.cl/potenciometro-rotacional-10k/>                                       |
| Potenciometro 250K              | 4         | $495            | <https://altronics.cl/potenciometro-lineal-250k-b250k\>                                               |
| Capacitor no polarizado 10nf    | 1         | $100            | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/>                          |
| Capacitor no polarizado 100nF   | 7         | $100            | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/>                          |
| Capacitor polarizado 0.22uF 50V | 1         | $100            | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> |
| Capacitor polarizado 1uF 50V    | 1         | $100            | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> |
| Capacitor polarizado 10uF 50V   | 8         | $100            | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> |
| Capacitor polarizado 100uF 50V  | 4         | $100            | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> |
| Resistencia 1K                  | 9         | $100            | <https://www.mechatronicstore.cl/resistencias-electricas-3w-por-unidad/>                              |
| Resistencia 100K                | 2         | $100            | <https://www.mechatronicstore.cl/resistencias-electricas-1-2-w-1-unidad/>                             |
| Led 3mm/5mm                     | 5         | $100            | <https://www.mechatronicstore.cl/led-3mm-5mm/>                                                        |
| Diodo 1N4007                    | 3         | $200            | <https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/>                              |
| Diodo 1N4148                    | 4         | $120            | <https://www.cabezacuadrada.cl/product/diodo-1n4148/>                                                 |
| Regulador de Voltaje L7805      | 3         | $490            | <https://www.mechatronicstore.cl/regulador-limitador-de-voltaje-5v-dc/>                               |
| Barrel Jack Switch              | 6         | -               | -                                                                                                     |
| Audio Jack                      | 5         | -               | -                                                                                                     |
| Conector Pinsocket  (placa)     | 6         | $400            | <https://www.ebay.com/itm/125539599767>                                                               |
| Pernos 3mm (para mountinghole)  | 13        | $39,9           | <https://www.mercadolibre.cl/pack-x100u-perno-allen-m3-negro-cabeza-boton-8mm/>                       |
| Switch encendido/apagado        | 3         | -               | -                                                                                                     |

Armar un “Biofonía” cuesta: $ 

(Incluir tiempo de soldadura)

![soldadura](./imagenes/procreso-soldadura.png)

## Carcasa

El objetivo desde el principio fue que Biofonía no pareciera un sintetizador. Que alguien lo viera sobre una mesa y no supiera inmediatamente qué es, pero que quisiera tocarlo igual.
El principal referente para el desarrollo de la carcasa fue el trabajo de **Kelly Heaton**, cuya práctica transforma circuitos electrónicos en organismos que parecen pertenecer al mundo natural. En particular, *Circuit Garden* y *Electronic Naturalism* sirvieron como guía para pensar la electrónica no como algo que debe ocultarse o disfrazarse, sino como una forma de vida propia. Más que replicar su estética, nos interesó su manera de construir un ecosistema donde tecnología y naturaleza dejan de ser opuestos y comienzan a convivir, una idea que terminó definiendo el jardín donde habita Biofonía. 

![referentes carcasa](./imagenes/referentes-carcasa.png)

Siguiendo la lógica del sistema, si los módulos imitan seres vivos y el conjunto forma un ecosistema, la carcasa tenía que ser el lugar donde ese ecosistema existe. La respuesta fue un jardín: una base verde de la que emergen flores, y en cada flor vive una perilla. Las criaturas no flotan en el aire, habitan algo.

![ideas carcasa](./imagenes/ideas-carcasa.png)

Para que todo correspondiera con precisión a las medidas reales de los componentes, potenciómetros, jacks y switches, se decidió utilizar impresión 3D. Es el método que mejor permite iterar rápido, ajustar medidas y garantizar que cada pieza encaje donde tiene que encajar sin improvisaciones. *La naturaleza es imprecisa. La carcasa no puede serlo.*

![proceso carcasa](./imagenes/proceso-carcasa.png)

![proceso carcasa 02](./imagenes/proceso-carcasa-2.png)

Cada módulo tiene su propio grupo de flores, agrupadas por criatura. Lub-dub en el centro, como corresponde a un corazón. Berry Benson a un costado, como si revoloteara. El Chirihue Mecanizado arriba, donde estaría un pájaro.

![resultado carcasa](./imagenes/carcasa.png)

## Composición

### Partitura 1

Esta no tiene pentagramas, no tiene corcheas, no tiene nada que te haga sentir mal por no saber solfeo. Es una partitura para tres criaturas electrónicas que nunca han tomado clases de música y están muy bien así.

El sintetizador se toca en tiempo real, ajustando las perillas de cada módulo según las instrucciones de cada acto. La obra dura 24 horas y está pensada para ser tocada una vez al día, todos los días.

- Todas las perillas parten en 0°, es decir, giradas completamente hacia la izquierda. Los grados indicados en la tabla se cuentan desde ese punto girando en sentido horario. Por ejemplo, 180° es exactamente la mitad del recorrido de la perilla.

#### 08:00 – 12:00

El Chirihue Mecanizado está despertando pero no quiere molestar a nadie. Berry Benson apenas se escucha, como una abeja muy educada que recién llega al trabajo. Lub dub está ansioso. Son las 8am.

| Módulo | Perilla 1 | Perilla 2 | Perilla 3 |
|--------|-----------|-----------|-----------|
| Chirihue Mecanizado | 240° | 220° | 60° |
| Berry Benson | 220° | 240° | 60° |
| Lub dub | 240° | 220° | 200° |

#### 12:01 – 16:00

El Chirihue canta con energía. Es mediodía y tiene cosas que decir. Berry se está acomodando: más lenta, pero más fuerte. Lub dub ya almorzó.

| Módulo | Perilla 1 | Perilla 2 | Perilla 3 |
|--------|-----------|-----------|-----------|
| Chirihue Mecanizado | 280° | 260° | 200° |
| Berry Benson | 140° | 160° | 180° |
| Lub dub | 160° | 140° | 160° |

#### 16:01 – 20:00

El Chirihue canta lento y bajito, se está yendo. Berry es muy lenta pero reina con volumen, es la hora de la abeja. Lub dub está cansado pero presente.

| Módulo | Perilla 1 | Perilla 2 | Perilla 3 |
|--------|-----------|-----------|-----------|
| Chirihue Mecanizado | 80° | 60° | 40° |
| Berry Benson | 60° | 80° | 260° |
| Lub dub | 80° | 100° | 240° |

#### 20:01 – 07:59

El Chirihue se fue a su nido de cables a descansar. Berry también se fue. Lub dubgft sigue. Los corazones no saben lo que es el descanso.

| Módulo | Perilla 1 | Perilla 2 | Perilla 3 |
|--------|-----------|-----------|-----------|
| Chirihue Mecanizado | 0° | 0° | 0° |
| Berry Benson | 0° | 0° | 0° |
| Lub dub | 40° | 40° | 180° |

#### Notas de interpretación

- Las perillas no mencionadas en la tabla se dejan fijas en la posición que suene mejor al momento de armar el instrumento. No se tocan durante la interpretación.
- Las transiciones entre actos no son abruptas. Las perillas se giran despacio, como quien no quiere que nadie se dé cuenta de que algo cambió.
- Los grados son un punto de partida, no una ley. Si al girar una perilla suena horrible, gírala hasta que suene bien y anótalo. La partitura es un ser vivo.
- Si en algún momento los tres módulos suenan al mismo tiempo en su punto más alto, eso no es un error. Ese es el clímax. Felicitaciones.
- El silencio de 20:01 a 07:59 no es silencio total: Lub dub sigue latiendo. Siempre sigue latiendo.

(VIDEO!!!)

### Partitura 2

![partitura 2](./imagenes/partitura-2-1.jpg)

Cada una de las líneas en la partitura representan ciertas cosas:

- Para las abejas, representadas de color amarillo (🟡), se hicieron las líneas que se usan para ilustrarlas de manera caricaturesca.
- El corazón, representado en color rojo (🔴) utiliza las líneas de signos vitales que se pueden ver en una máquina de signos vitales.
- Para el pájaro, representado en color naranjo (🟠), se hizo una variación de un espectrograma que captaba el sonido de las aves. (*Los espectrogramas son un gráfico visual que muestran los sonidos o señales acústicas registradas.*). 

![partitura 2 referencias](./imagenes/partitura-2-referencias.jpg)

![partitura 2 desglose](./imagenes/partitura-2-2.jpg)

#### Notas de interpretación

- Por el lado izquierdo de la partitura, se dividió en 5 partes iguales para medir el volumen, siendo la línea del centro el valor medio del volumen en general, considerando el valor mínimo (0) y el máximo (100).
- En medio de la partitura, está igualmente se parte en 5, pero en este caso, cada separación representa un minuto de la partitura.

(VIDEO!!!)

## Bibliografía

- Akther, S. (s.f). Vectores corazón real. Vecteezy. <https://es.vecteezy.com/arte-vectorial/67973094-anatomico-humano-corazon-ilustraciones-anatomia-medico>
- DIY Strat. (2008, 17 de agosto). Two-channel mini-mixer. Guitar and effects DIY. <https://diystrat.blogspot.com/2008/08/two-channel-mini-mixer.html>
- Heaton, K. (s.f.). Kelly Heaton Studio. <https://www.kellyheatonstudio.com/>
- Inti-Illimani. (s.f.). La Fiesta de San Benito. Letras.com. <https://www.letras.com/inti-illimani/516597/>
- Modern Met, M. (2021, 22 de abril). Esta artista crea "aves electrónicas" impresas en 3D que cantan como pájaros reales. My Modern Met en Español. <https://mymodernmet.com/es/kelly-heaton-aves-circuitos/>
- Pearson, K. (2024). Make: Electronic Music from scratch. Make Community, LLC.
- Stock, M. (25 de Febrero, 2026). Silueta simple en negro y blanco de una abeja. Shutterstock. <https://www.shutterstock.com/es/image-vector/simple-black-white-silhouette-bee-representing-2743356303>
- Williams, E. (25 de Marzo, 2015). Logic Noise: Filters And Drums. Hackaday. <https://hackaday.com/2015/03/25/logic-noise-filters-and-drums/>
