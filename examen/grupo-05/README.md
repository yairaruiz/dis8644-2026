# examen-grupo-05

# Sistema Modular — [Nombre del instrumento]

## Integrantes

| Nombre            | Cuenta de GitHub |
| ----------------- | ---------------- |
| Luisa Toro        |30-Luisaatoro9    |
| Antonia Améstica  |04-antoniaamc     |
| Sebastián Guevara |14-sebastianguevaralarotta|
| Catalina Jeria    |15-catalinajeria  |
| Catalina Balboa   |05-Catabalboa     |

---

# Criterios de diseño del sistema

El sistema fue concebido como un instrumento modular donde cada placa representa un universo independiente que, al conectarse con las demás, forma un ecosistema sonoro completo. Desde el inicio del proyecto buscamos que el diseño no fuera únicamente funcional, sino también narrativo, permitiendo que cada módulo aportara una identidad propia al conjunto.

El criterio principal consistió en comprender que un sintetizador modular no es una pieza única, sino un sistema compuesto por diferentes procesos electrónicos que interactúan entre sí. Esta lógica fue trasladada a la propuesta formal, donde cada módulo conserva su autonomía visual pero adquiere un nuevo significado al integrarse con los demás.

---

# Inspiración

La inspiración surgió durante las conversaciones del grupo acerca de nuestros intereses personales. Descubrimos que gran parte de ellos coincidían en universos de ciencia ficción presentes en películas y series.

La principal referencia fue la saga **Star Wars**, donde distintos planetas, personajes y tecnologías funcionan de manera independiente, pero forman parte de un mismo universo. Esta idea fue el detonante conceptual del proyecto: entender que cada placa electrónica corresponde a un "planeta" con una función específica y que, al conectarse entre sí, construyen un instrumento modular completo.

Nuestro aporte corresponde al módulo de filtro, concebido como una nave que viaja entre estos mundos sonoros e interviene el flujo del sonido antes de continuar hacia el siguiente proceso.

---

# Contexto de diseño

El proyecto fue desarrollado desde Chile considerando la disponibilidad de materiales accesibles y técnicas de fabricación de bajo costo.

Para construir la carcasa general se recurrió a materiales como alambre, arcilla y sistemas simples de ensamblaje manual, buscando demostrar que es posible desarrollar propuestas expresivas utilizando recursos fácilmente disponibles.

La carcasa adopta la forma de una geoda o un pequeño planeta cristalino. Los cristales representan la energía y la luz producida por el funcionamiento simultáneo de los distintos módulos electrónicos. Dentro de esta estructura aparece la carcasa del filtro, representada como una nave que atraviesa este planeta y completa el recorrido del sonido.

---

# Nombre del sistema

**________________________________________**

---

# Placas utilizadas

| Módulo              | Grupo     | Función       |
| ------------------- | --------- | ------------- |
| Chirigüe mecanizado | Grupo 4   | Oscilador     |
| Lub-dub             | Grupo 6   | Percutor      |
| ALO HOUSTON         | Grupo 5 | Filtro pasivo |
| PARLA               | LID     | Parlante de audio |

---

# Principio de funcionamiento

## Chirigüe mecanizado — Oscilador

El oscilador constituye la fuente principal de señal del sistema. Su función consiste en generar una señal eléctrica periódica cuya frecuencia determina la altura del sonido. Esta señal sirve como punto de partida para el resto de los módulos.

**Recibe:** alimentación eléctrica.

**Entrega:** señal de audio oscilante hacia el resto del sintetizador.

---

## Lub-dub — Percutor

El módulo percutor genera impulsos rítmicos o envolventes que permiten producir patrones repetitivos y eventos sonoros de carácter percusivo.

**Recibe:** alimentación y señales de sincronización.

**Entrega:** pulsos o señales rítmicas que modulan otros módulos del sistema.

---

## ALO HOUSTON — Filtro

El filtro pasivo modifica el contenido espectral de la señal proveniente del oscilador. Mediante dos controles variables (RV1 y RV2) atenúa determinadas frecuencias, alterando el color o timbre del sonido sin generar señal propia.

**Recibe:** señal de audio proveniente del oscilador.

**Entrega:** señal filtrada hacia la salida del sintetizador o hacia otros módulos posteriores.

---

# Flujo general del sistema

```text
Oscilador
      │
      ▼
Filtro
      │
      ▼
Percutor / Modulación
      │
      ▼
Salida de audio
```

---

# Lista de materiales

Aquí están todas las tablas reorganizadas con un formato consistente. También agregué una columna de **Subtotal** para que sea más fácil calcular el costo total de cada proyecto.

---

# Grupo 5 – Alo Houston

| Componente           | Valor / Referencia | Cantidad | Valor Unitario (CLP) | Subtotal (CLP) |
| -------------------- | ------------------ | :------: | -------------------: | -------------: |
| Capacitor cerámico   | 103                |     2    |                 $150 |           $300 |
| Capacitor cerámico   | 104                |     1    |                 $150 |           $150 |
| Capacitor cerámico   | 102                |     1    |                 $150 |           $150 |
| Capacitor polarizado | 4.7 µF / 16 V      |     2    |                 $140 |           $280 |
| Resistencia          | 10 kΩ              |     2    |                  $90 |           $180 |
| Resistencia          | 1 kΩ               |     1    |                 $100 |           $100 |
| Potenciómetro        | 100 kΩ             |     2    |                 $490 |           $980 |
| **TOTAL**            |                    |          |                      |     **$2.140** |

---

# Grupo 4 – Chirigüe Mecanizado (Oscilador)

| Componente                | Valor / Modelo | Cantidad | Valor Unitario (CLP) | Subtotal (CLP) | Link                                                                                                                                                                                         |
| ------------------------- | -------------- | :------: | -------------------: | -------------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Chip                      | CD40106        |     1    |               $1.200 |         $1.200 | [https://electronicareal.cl/producto/integrado-digital-cd-40106/](https://electronicareal.cl/producto/integrado-digital-cd-40106/)                                                           |
| Amplificador operacional  | LM324          |     1    |                 $590 |           $590 | [https://www.mechatronicstore.cl/amplificador-operacional-lm324/](https://www.mechatronicstore.cl/amplificador-operacional-lm324/)                                                           |
| Regulador                 | L7805          |     1    |                 $350 |           $350 | [https://www.victronics.cl/reguladores/reguladorvoltl7805cv5v-15ato220/](https://www.victronics.cl/reguladores/reguladorvoltl7805cv5v-15ato220/)                                             |
| Condensador electrolítico | 10 µF          |     3    |                 $330 |           $990 | [https://www.victronics.cl/condensadores/condensadorelectrolitico10uf50v/](https://www.victronics.cl/condensadores/condensadorelectrolitico10uf50v/)                                         |
| Condensador cerámico      | 100 nF         |     2    |                 $100 |           $200 | [https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/](https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/)                                     |
| Condensador electrolítico | 100 µF         |     1    |                 $380 |           $380 | [https://www.victronics.cl/condensadores/cond-electrolitico-100uf-25v20105oc-6x12-p2-5mm-10u/](https://www.victronics.cl/condensadores/cond-electrolitico-100uf-25v20105oc-6x12-p2-5mm-10u/) |
| Diodo                     | 1N4148         |     1    |                 $100 |           $100 | [https://www.mechatronicstore.cl/diodo-rectificador-de-alta-frecuencia-1n4148-do35/](https://www.mechatronicstore.cl/diodo-rectificador-de-alta-frecuencia-1n4148-do35/)                     |
| Diodo                     | 1N4007         |     1    |                 $200 |           $200 | [https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/](https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/)                                             |
| Potenciómetro             | 100 kΩ         |     4    |                 $495 |         $1.980 | [https://altronics.cl/potenciometro-lineal-100k-b100k](https://altronics.cl/potenciometro-lineal-100k-b100k)                                                                                 |
| Resistencia               | 1 kΩ           |     6    |                 $100 |           $600 | [https://www.mechatronicstore.cl/resistencia/](https://www.mechatronicstore.cl/resistencia/)                                                                                                 |
| LED                       | 5 mm           |     2    |                 $300 |           $600 | [https://www.mechatronicstore.cl/led-intermitente-5mm/](https://www.mechatronicstore.cl/led-intermitente-5mm/)                                                                               |

---

# Grupo 6 – Lub-dub (Percutor)

| Componente                | Valor / Modelo | Cantidad | Valor Unitario (CLP) | Subtotal (CLP) | Link                                                                                                                                                                                                       |
| ------------------------- | -------------- | :------: | -------------------: | -------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Chip                      | CD40106        |     1    |               $1.200 |         $1.200 | [https://electronicareal.cl/producto/integrado-digital-cd-40106/](https://electronicareal.cl/producto/integrado-digital-cd-40106/)                                                                         |
| Chip                      | CD4069         |     1    |               $1.100 |         $1.100 | [https://www.cabezacuadrada.cl/product/cd4069/](https://www.cabezacuadrada.cl/product/cd4069/)                                                                                                             |
| Regulador                 | L7805          |     1    |                 $490 |           $490 | [https://www.mechatronicstore.cl/regulador-limitador-de-voltaje-5v-dc/](https://www.mechatronicstore.cl/regulador-limitador-de-voltaje-5v-dc/)                                                             |
| Condensador electrolítico | 10 µF          |     2    |                 $330 |           $660 | [https://www.victronics.cl/condensadores/condensadorelectrolitico10uf50v/](https://www.victronics.cl/condensadores/condensadorelectrolitico10uf50v/)                                                       |
| Condensador cerámico      | 100 nF         |     4    |                 $100 |           $400 | [https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/](https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/)                                                   |
| Condensador cerámico      | 10 nF          |     1    |                 $100 |           $100 | [https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/](https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/)                                                   |
| Condensador electrolítico | 100 µF         |     1    |                 $380 |           $380 | [https://www.victronics.cl/condensadores/cond-electrolitico-100uf-25v20105oc-6x12-p2-5mm-10u/](https://www.victronics.cl/condensadores/cond-electrolitico-100uf-25v20105oc-6x12-p2-5mm-10u/)               |
| Condensador               | 0.22 µF        |     1    |                 $100 |           $100 | [https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/](https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/) |
| Diodo                     | 1N4007         |     1    |                 $200 |           $200 | [https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/](https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/)                                                           |
| Potenciómetro             | 100 kΩ         |     4    |                 $495 |         $1.980 | [https://altronics.cl/potenciometro-lineal-100k-b100k](https://altronics.cl/potenciometro-lineal-100k-b100k)                                                                                               |
| Resistencia               | 1 kΩ           |     1    |                 $100 |           $100 | [https://www.mechatronicstore.cl/resistencia/](https://www.mechatronicstore.cl/resistencia/)                                                                                                               |
| Resistencia               | 100 kΩ         |     2    |                 $100 |           $200 | [https://www.mechatronicstore.cl/resistencias-electricas-1-2-w-1-unidad/](https://www.mechatronicstore.cl/resistencias-electricas-1-2-w-1-unidad/)                                                         |
| LED                       | 5 mm           |     2    |                 $300 |           $600 | [https://www.mechatronicstore.cl/led-intermitente-5mm/](https://www.mechatronicstore.cl/led-intermitente-5mm/)                                                                                             |
| LED                       | 3 mm / 5 mm    |     1    |                 $100 |           $100 | [https://www.mechatronicstore.cl/led-3mm-5mm/](https://www.mechatronicstore.cl/led-3mm-5mm/)                                                                                                               |

---

Tiempo total de soldadura**

---

---

# Carcasa del filtro

## Concepto

La propuesta no corresponde simplemente a una carcasa de acrílico. Se plantea como una estructura cuya función es proteger, organizar, revelar y comunicar el funcionamiento interno del instrumento.

En lugar de ocultar la electrónica, la estructura la exhibe como parte esencial de la identidad visual del objeto.

---

## Decisiones materiales y formales

La estructura está conformada por dos placas de acrílico cortadas mediante láser siguiendo exactamente el contorno de la PCB, respetando la silueta inspirada en un tocadiscos presente en el diseño original de la placa.

Una pieza funciona como base y la otra como panel superior. Ambas permanecen separadas mediante pernos M3 de aproximadamente 15 a 20 mm de altura.

Esta solución genera un volumen liviano donde la placa permanece suspendida entre ambas piezas, permitiendo observar completamente el circuito desde la parte superior y desde los laterales.

La transparencia del acrílico transforma al circuito en el principal protagonista visual del instrumento.

---

# Inspiración y referentes

Uno de los principales referentes fue **Bleep Labs**, fabricante de sintetizadores experimentales cuya filosofía consiste en comprender la electrónica como parte del lenguaje visual del instrumento.

Más que reproducir la apariencia de sus productos, se tomó como referencia la idea de que el circuito deje de ser un componente oculto y pase a convertirse en un elemento visible que comunica el funcionamiento del instrumento y fortalece la relación entre el usuario, la electrónica y el sonido.

---

# Composición

La composición de la carcasa también toma como referencia las ideas desarrolladas por **Yoko Ono** sobre la participación activa del usuario frente al objeto.

En sus obras e instrucciones artísticas, el valor no reside únicamente en el objeto físico, sino en la experiencia que genera durante su utilización.

Siguiendo esta lógica, el sintetizador no busca esconder su funcionamiento detrás de una caja cerrada. Al contrario, expone el circuito para invitar al usuario a comprender cómo se produce el sonido y cómo cada componente participa en dicho proceso.

La carcasa deja de ser un simple contenedor y se transforma en un elemento de comunicación entre la electrónica y quien interpreta el instrumento.

---

# Partitura experimental

## ONDAS INVISIBLES

**Instrumento:** sintetizador conectado al filtro pasivo de dos controles (RV1 y RV2).

**Duración:** 5 a 10 minutos.

1. Comienza con una única nota sostenida.
2. Gira RV1 lentamente desde el mínimo hasta el máximo durante un minuto completo.
3. Escucha únicamente los cambios de color del sonido. No cambies la nota.
4. Cuando percibas una frecuencia que te recuerde un lugar, mantén esa posición durante diez segundos.
5. Cambia a otra nota. Puede ser más aguda o más grave. No debe seguir ninguna escala.
6. Mueve RV2 muy lentamente hasta que el sonido parezca respirar.
7. Introduce silencios. Los silencios deben durar más de lo que resulte cómodo.
8. Repite una nota tres veces. Cada repetición debe ser más suave que la anterior.
9. Lleva ambos controles al extremo opuesto.
10. Toca una última nota.
11. Espera a que desaparezca completamente.
12. No hagas nada durante treinta segundos.

**Fin.**

---

# Operación de la partitura

La partitura fue diseñada para facilitar la interacción de personas sin experiencia previa con sintetizadores modulares. En lugar de exigir conocimientos musicales o técnicos, propone acciones sencillas que permiten descubrir progresivamente el comportamiento del filtro mediante la escucha.

Cada instrucción invita al intérprete a prestar atención a pequeñas variaciones del sonido, promoviendo una experiencia basada en la exploración más que en la ejecución correcta.

---

# Proceso de creación

La partitura surge de la intención de transformar la primera interacción con el sintetizador en una experiencia abierta y accesible.

Al mismo tiempo, incorpora momentos de incomodidad deliberada —como silencios prolongados o la ausencia de referencias tonales tradicionales— para invitar al intérprete a abandonar expectativas convencionales y construir una interpretación propia.

De esta forma, el usuario deja de reproducir una pieza musical y comienza a descubrir nuevos paisajes sonoros mediante la experimentación.

---

# Referentes

La estructura de instrucciones se inspira en las **Instruction Pieces** de **Yoko Ono**, donde la obra se activa únicamente cuando el participante ejecuta una serie de acciones propuestas por la autora.

Asimismo, la exploración libre del sonido toma referencias de la música experimental y de la práctica de improvisación característica de los sintetizadores modulares.

---

# Simbología

La partitura reemplaza la notación musical tradicional por acciones e instrucciones.

Cada movimiento de los controles representa una exploración del espacio sonoro; los silencios funcionan como parte activa de la composición; y la ausencia de una melodía predeterminada convierte cada interpretación en una experiencia única e irrepetible.

El resultado final depende completamente de las decisiones tomadas por quien interactúa con el instrumento, haciendo que cada ejecución construya un nuevo recorrido dentro del universo modular propuesto.

PAUTA: / imaenes + funcionamiento detallado .

INCOMPLETO, subido por si acaso

## integrantes

| Nombre | Cuenta de GitHub |
| --- | --- |
| Luisa Toro | @30-Luisaatoro9 |
| Antonia Améstica | @04-antoniaamc |
| Sebastián Guevara | @14-sebastianguevaralarotta |
| Catalina Jeria | @15-catalinajeria |
| Catalina Balboa | @05-Catabalboa |

## criterios de diseño del sistema

inspiración para construir, desde donde partieron

contexto desde Chile, desde nuestra disponibilidad material

nombre de sistema/instrumento construido por medio de módulos

## 2. Placas Utilizadas 

Durante el proceso de ensamble y pruebas en el taller, el proyecto decantó en dos grupos de circuitos: los que lograron integrarse exitosamente para formar el instrumento final, y los que, pese a haber sido soldados, debieron ser descartados del montaje por fallas o inestabilidad.

### Placas en funcionamiento (Sistema Final)

| Módulo | Origen / Grupo | Función Principal |
| --- | --- | --- |
| **Reloj (RELO)** | Cátedra / Profesores | Generador de pulsos de sincronía temporizados. |
| **Secuenciador CD4017** | Primer Circuito | Control de pasos rítmicos distribuidos (Ver Nota Final). |
| **Lub-dub** | Grupo 06 | **Oscilador** (Fuente principal de señal de audio activa). |
| **Filtro Paso Bajo Activo** | Grupo 05 | Filtro Analógico VCF soldado sobre cobre desnudo. |

### Placas soldadas pero no utilizadas (Descartadas)

| Módulo | Origen / Grupo | Estado / Observación |
| --- | --- | --- |
| **Secuenciador** | Grupo 02 | Descartado por inestabilidad en la cadena general. |
| **Comando Estelar** | Grupo 03 | Soldado, pero no integrado al flujo definitivo. |
| **Chirigüe Mecanizado** | Grupo 04 | Oscilador original descartado por fallas en placa. |
| **PARLA** | LID | Módulo de salida descartado. |

**Flujo general del sistema:**

## 3. Funcionamiento de las placas

### Placa 1: RELO 

Este módulo funciona como el reloj del sistema, es el encargado de dictar el "tiempo" o la velocidad de todo el sintetizador. Sin él, el sistema no tendría una referencia para avanzar y, por lo tanto, no habría ritmo. Su función es generar constantemente una señal eléctrica llamada "onda cuadrada" (un pulso que sube y baja de voltaje a un ritmo constante), que sale hacia el secuenciador para marcarle el paso a cada uno de sus movimientos. Esta placa fue diseñada por nuestros profesores de cátedra.

* **Señal de Salida:** Emite una onda cuadrada que es el pulso maestro del sintetizador.
* **Recepción y Envío:** Actúa como la fuente emisora que alimenta directamente al Secuenciador CD4017, sincronizando todos los procesos temporales del instrumento.

### Placa 2: Secuenciador

El secuenciador toma el pulso rítmico que viene del RELO y, con cada pulso, activa un marcador. Apenas llega al cuarto paso, vuelve a empezar inmediatamente sin pausas. Así, transformamos un simple pulso eléctrico en un bucle rítmico continuo, indicándole a la máquina exactamente en qué momento debe actuar.

Para entender este módulo de forma sencilla, imaginen un contador de cuatro tiempos. El secuenciador no genera ningún sonido por sí mismo, su trabajo es ir activando luces y marcando ritmos uno tras otro siguiendo el "tic-tac" del metrónomo. 

Originalmente, nuestro plan era utilizar la PCB diseñada por el **Grupo 06 (Contador Binario)** para cumplir con esta función. Sin embargo, tras ensamblar la placa, el circuito no funcionó. Frente a este imprevisto, tomamos la decisión técnica de descartarla y construir una solución alternativa desde cero. Para ello, decidimos utilizar el esquemático original entregado por nuestro profesor de cátedra y **soldar los componentes directamente a mano sobre una placa de contacto (PCB genérica perforada) que teníamos a libre disposición en el taller. Estructurando el circuito en torno al integrado **CD4017** (un contador de década).

> * **Diseño Original:** Documentación técnica y esquemático base provisto por la Cátedra del Taller de Máquinas Electrónicas.

### Placa 3: Oscilador

### Placa 4: Filtro


## 4. Proceso de armado de cada placa, aprendizajes y complicaciones

Explicar primer modulo

#### Detalles del Funcionamiento Técnico

Al integrar el secuenciador CD4017 en nuestra placa, logramos transformar los pulsos del módulo reloj (555) en un ciclo lógico estructurado. Para asegurar el éxito de esta etapa, mapeamos las salidas y configuramos el reinicio del chip, obteniendo los siguientes resultados:

> * **Diseño Original:** Documentación técnica y esquemático base provisto por la Cátedra del Taller de Máquinas Eelectrónicas.

### Filtro Paso Bajo Activo — Grupo 05

El circuito que realizamos corresponde a un **filtro pasabajos activo**. Su función es dejar pasar principalmente las frecuencias bajas, que corresponden a los graves, mientras que reduce las frecuencias altas o agudos. Este tipo de circuito se utiliza en equipos de audio cuando se quiere obtener un sonido más grave, por ejemplo en un subwoofer.

Se llama filtro **activo** porque utiliza un componente electrónico activo, que en este caso es el integrado **JRC4558**, el cual necesita alimentación para poder funcionar. En nuestro montaje decidimos utilizar una alimentación de **5 V**, obtenida desde una salida USB de una batería recargable. Aunque el esquema original suele alimentarse con un voltaje mayor, durante las pruebas comprobamos que con 5 V el circuito funcionó correctamente para la aplicación que necesitábamos.

#### Recorrido de la señal
La señal de audio entra por el terminal llamado **Audio Input**. Esa señal puede venir desde un teléfono, un computador o cualquier dispositivo que entregue audio. Antes de llegar al integrado, la señal pasa por una combinación de resistencias, capacitores y el potenciómetro de frecuencia. Todos estos componentes trabajan juntos para determinar qué frecuencias van a pasar y cuáles se van a atenuar.

Después de ser procesada por el integrado, la señal pasa por el potenciómetro de volumen y finalmente sale por **Audio Output**, lista para conectarse a un amplificador o a un parlante.

#### Alimentación
El circuito necesita alimentación porque el JRC4558 no puede funcionar por sí solo. En nuestro caso decidimos utilizar una fuente de **5 V** desde un adaptador de corriente AC/DC. El terminal positivo entrega la energía al integrado y el terminal G corresponde a la tierra o negativo común del circuito. Todos los componentes utilizan esa referencia para funcionar correctamente.

#### Componentes en Detalle

| Componente | Función / Descripción |
| --- | --- |
| **Integrado JRC4558** | El componente más importante del circuito es el **JRC4558**, que es un amplificador operacional doble. Aunque internamente tiene dos amplificadores operacionales, en este circuito solamente se utiliza uno. Su función es recibir la señal de audio y trabajar junto con las resistencias y los capacitores para realizar el filtrado. Además ayuda a mantener una señal estable y evita que el filtro pierda demasiado nivel de salida, algo que normalmente ocurre en los filtros pasivos. |
| **Resistencias** | Cumplen varias funciones dentro del circuito. Primero, controlan la cantidad de corriente que circula por algunas partes del circuito, protegiendo al integrado. También ayudan a establecer el punto de funcionamiento del amplificador operacional para que trabaje correctamente. Además, junto con los capacitores forman la red RC, que es la encargada de definir la frecuencia de corte del filtro. |
| **Capacitores** | Son fundamentales porque reaccionan de forma distinta dependiendo de la frecuencia de la señal. En este circuito aparecen dos capacitores cerámicos. El primero está marcado como **472**, que corresponde a **4,7 nanofaradios**. El segundo está marcado como **222**, que corresponde a **2,2 nanofaradios**. Estos capacitores, al trabajar junto con las resistencias, hacen que las frecuencias altas se atenúen mientras las bajas puedan seguir pasando. Por eso el resultado es un sonido con mayor presencia de graves. |
| **Potenciómetro de frecuencia** | El primer potenciómetro está marcado como **Frequency** y tiene un valor de **100K**. Su función es modificar la frecuencia de corte del filtro. Cuando giramos la perilla, cambia el valor de resistencia dentro de la red RC. Eso hace que el filtro deje pasar una mayor o menor cantidad de frecuencias. Si aumentamos la resistencia, el filtro elimina más agudos y el sonido queda más grave. Si disminuimos la resistencia, pasan más frecuencias y el sonido conserva más medios y agudos. |
| **Potenciómetro de volumen** | El segundo potenciómetro se llama **Level**. Su función es mucho más simple: solamente controla el volumen de salida. No modifica el filtrado del sonido. Lo único que hace es aumentar o disminuir el nivel de la señal que ya fue procesada. |

#### ¿Cómo funciona todo junto?
Cuando entra la señal de audio, las resistencias y los capacitores comienzan a separar las frecuencias. El integrado procesa esa señal utilizando la red de realimentación formada por esos mismos componentes. Después, el usuario puede ajustar la frecuencia de corte con el potenciómetro **Frequency** y regular el volumen final con el potenciómetro **Level**. Finalmente, la señal sale filtrada por la salida de audio.

#### ¿Por qué se llama filtro pasabajos?
Se llama pasabajos porque permite el paso de las frecuencias bajas y reduce las frecuencias altas. La frecuencia donde comienza esa reducción se conoce como **frecuencia de corte**, y depende de los valores de las resistencias y los capacitores del circuito.

#### Conclusión
En resumen, este circuito recibe una señal de audio, elimina parte de las frecuencias altas mediante una red formada por resistencias y capacitores, el integrado JRC4558 procesa esa señal para obtener un filtrado más estable y el usuario puede ajustar tanto la frecuencia de corte como el volumen de salida mediante los dos potenciómetros. El resultado es una señal donde predominan los sonidos graves.

## carcasa

## 5. Arquitectura Estructural de las Carcasas

La carcasa de nuestro instrumento trasciende la idea de ser un simple contenedor protector. Se concibe como un manifiesto formal y material cuya meta es resguardar, estructurar, revelar y comunicar de manera clara la trama electrónica que ocurre en su interior. En perfecta sincronía con nuestra metáfora de la Tierra y el Cielo (el meteorito y el telescopio), decidimos que el sistema final no habitara en una sola caja ciega, sino en **dos carcasas físicas diferenciadas** que dialogan entre sí a través del contraste de sus materiales y procesos de fabricación.

### Carcasa 1: Geoda 

Esta unidad funciona como el "núcleo rítmico" y sonoro del sistema. Contiene dos placas que operan de forma conjunta:
* El módulo **Secuenciador** 
* El módulo **Oscilador/Percutor (Lub-Dub)**.

**Un meteorito llegó desde el espacio.** ¿Por qué tiene cables? ¿Las luces significan algo? ¿Qué nos están tratando de decir? ¿Es solo ruido o hay algo más?...

Los científicos intentan capturar este sonido y necesitan descifrarlo. **¿Seremos capaces? ¿Será que aún no estamos listos?**...

Primero necesitamos entender su forma. En la Tierra existen unas rocas llamadas **geodas**. Estas son formaciones geológicas cuyo interior está parcial o totalmente cristalizado.

Los cristales de este meteorito son muy parecidos a los de una geoda. **¿Será que la luz en su interior y sus cristales están tratando de salir por los orificios para no pasar desapercibidos?**

**Su interior:**

En su interior hay unas placas que están emitiendo señales. En uno de sus lados se encuentran estas luces y, en el otro, está el **¿corazón?** Tiene la forma de un corazón humano, aunque no sabemos de dónde proviene este meteorito.

Lo que sí sabemos es que, **al conectarlo, comienza a emitir señales**. Se escuchan ruidos intensos, como un corazón acelerado, o sonidos más débiles, como un corazón que se está apagando. Su pulso puede ser fuerte o suave y la señal puede volverse lenta o muy rápida, **como una taquicardia**.

### Construcción

Para representar la caída del meteorito, el caos y su conexión con la Tierra, esta carcasa fue **construida completamente a mano**, alejándonos por completo de la fabricación digital. Su base se conforma por una estructura alámbrica recubierta con papel aluminio para generar el soporte estructural. Sobre esto, se modeló el volumen con cerámica en frío para lograr la textura rocosa, finalizando con un trabajo de pintura. 

FOTOS PROCESO

El detalle más íntimo de esta pieza se encuentra en su interior: cristales adheridos a mano que simulan el corazón cristalizado de una geoda real. Las luces LED de los circuitos actúan como indicadores visuales del "latido" del sistema, brillando y refractándose a través de estos cristales internos para asomarse hacia el exterior, invitando al observador a mirar dentro de la roca.

### Carcasa 2: Filtro

Esta segunda carcasa está dedicada exclusivamente al módulo del **Filtro Paso Bajo (VCF) del Grupo 05**. A diferencia de la rusticidad orgánica de la Geoda, esta unidad representa la precisión, el "cielo" y la observación estructurada.

Su arquitectura se compone de placas de acrílico transparente cortadas mediante tecnología láser. El vector de corte sigue fielmente el contorno perimetral de la PCB, respetando la icónica silueta inspirada en las líneas de un tocadiscos o un lente de observación, presente desde nuestras primeras etapas de diseño. La placa inferior actúa como base del chasis y la superior como panel de control e interfaz. Ambas caras se mantienen firmemente unidas y distanciadas mediante pernos M3 y espaciadores metálicos con una altura de entre 15 y 20 mm.

Esta solución de diseño da vida a un volumen liviano y suspendido. Al dejar los laterales abiertos y aprovechar la transparencia absoluta del acrílico, la **placa de cobre desnudo** se convierte en la protagonista indiscutida. El usuario puede escudriñar las soldaduras manuales y los componentes desde cualquier ángulo, transformando la ingeniería cruda en un paisaje visualmente contemplable.

### Influencias y referentes artísticos

El diseño conceptual de estos contenedores se apoya fuertemente en dos corrientes vanguardistas:

1. **Bleep Labs:** Firma icónica en la manufactura de sintetizadores experimentales. Su filosofía operativa plantea que la electrónica debe hablar el mismo idioma que la interfaz visual. El circuito no debe ser un secreto técnico confinado a una caja ciega; debe ser un elemento vivo que explica de forma transparente el origen del flujo eléctrico y sonoro, estrechando el vínculo entre el músico, la máquina y la onda sonora resultante.
2. **Yoko Ono (Composición Activa):** La disposición de los controles y la apertura de las carcasas dialogan con las teorías de participación artística planteadas por Yoko Ono. En sus postulados teóricos, el valor del arte no descansa en la rigidez del objeto estático, sino en las dinámicas humanas y las experiencias que se desencadenan cuando el espectador interactúa con él. Bajo este enfoque, nuestro sintetizador modular renuncia a la caja cerrada tradicional para invitar activamente al usuario a un viaje de descubrimiento perceptivo.

## composición

partitura e interpretación

detallar operación de la partitura, como se creó, cuales fueron los referentes (citando), cual es la simbología

## bibliografía
