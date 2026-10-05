# Problem Brief

## Decisión del problema

### Problema elegido

> **Anticipos de obra sin garantía.** Quien contrata una remodelación tiene que soltar plata antes de ver la obra, sin garantía de que el maestro la termine, y el maestro trabaja semanas sin garantía de que le paguen el saldo.

**Lo propuso:** Emanuel Benavides ([ver su propuesta](EmanuelBenavides.md)).

### Por qué elegimos este

Es el único de los cuatro problemas que cumple los **tres criterios de la Sesión 1**, y además fue el que mejor salió en nuestro análisis.

| Criterio de la Sesión 1 | Anticipos de obra | Gastos de terreno | Liquidar activos | Activos a distancia |
|---|:-:|:-:|:-:|:-:|
| 🤝 Partes que no confían entre sí comparten un registro | ✅ | ✅ | ✅ | ✅ |
| 🔒 Histórico inalterable | ✅ | ✅ | ➖ | ✅ |
| ✂️ Eliminar un intermediario que concentra la confianza | ✅ | ➖ | ✅ | ➖ |

Lo que inclinó la balanza:

- **Cumple los tres criterios.** La familia y el maestro casi nunca se conocen de antes. El único intermediario que podría dar confianza, la fiducia, no está al alcance de una obra pequeña. Y cuando hay pelea, nadie puede probar qué se acordó, qué se hizo y qué se pagó.
- **El dolor es fuerte y muy humano.** De un lado están los ahorros de una familia; del otro, semanas de trabajo de un maestro y su cuadrilla.
- **Lo podemos validar ya.** Familias que remodelan y maestros de obra están en nuestro círculo cercano, y conocemos el sector por nuestra investigación sobre transformación digital en la construcción.
- **Es una pieza de algo más grande.** Este problema es un micro componente de [Octoul](https://octoul.lat), nuestro proyecto de BIM y blockchain para verificar el avance de las obras, en el que ya hicimos validación y tenemos tracción en el sector. Resolverlo en una remodelación pequeña nos permite probar con familias y maestros lo que después escala a obras más grandes.

Calificamos los cuatro problemas con siete criterios ponderados (de 1 a 5):

```mermaid
%%{init: {"theme": "base", "themeVariables": {"fontFamily": "Inter, Helvetica, Arial, sans-serif", "xyChart": {"plotColorPalette": "#FDDA24", "backgroundColor": "#F6F7F8", "titleColor": "#0F0F0F", "xAxisLabelColor": "#0F0F0F", "yAxisLabelColor": "#0F0F0F", "xAxisLineColor": "#0F0F0F", "yAxisLineColor": "#0F0F0F"}}}}%%
xychart-beta horizontal
    title "Puntaje ponderado (1 a 5)"
    x-axis ["Anticipos de obra", "Gastos de terreno", "Liquidar activos", "Activos a distancia"]
    y-axis "Puntaje" 0 --> 5
    bar [4.25, 3.95, 3.20, 3.15]
```

<details>
<summary><b>Ver los criterios, los pesos y las notas</b></summary>

| Criterio | Peso | Anticipos de obra | Gastos de terreno | Liquidar activos | Activos a distancia |
|---|:-:|:-:|:-:|:-:|:-:|
| Pertinencia según los criterios de la Sesión 1 | 20 % | **5** | 3 | 4 | 4 |
| Acceso a usuarios para validar esta semana | 15 % | 4 | **5** | 2 | 2 |
| Qué tan fuerte es el dolor para quien lo sufre | 15 % | **5** | 4 | 3 | 4 |
| Se puede construir y demostrar en cuatro semanas | 15 % | **5** | 4 | 2 | 3 |
| Encaje con las prioridades de Stellar en 2026 | 15 % | 3 | 4 | **5** | 4 |
| Diferencia frente a lo que ya existe en Stellar | 10 % | 2 | **3** | **3** | 2 |
| Conocimiento y red del equipo en el sector | 10 % | **5** | **5** | 3 | 2 |
| **Puntaje ponderado** | | **4,25** | 3,95 | 3,20 | 3,15 |

Con un segundo escenario, que le da más peso a Stellar y a la diferenciación, el orden se mantiene: Anticipos de obra 3,95 · Gastos de terreno 3,85 · Liquidar activos 3,50 · Activos a distancia 3,20.

</details>

Y los ubicamos según cuánto interés generan y qué tan difícil sería abordarlos en cinco semanas:

```mermaid
%%{init: {"theme": "base", "themeVariables": {"fontFamily": "Inter, Helvetica, Arial, sans-serif", "quadrant1Fill": "#B7ACE8", "quadrant2Fill": "#FDDA24", "quadrant3Fill": "#F6F7F8", "quadrant4Fill": "#D6D2C4", "quadrant1TextFill": "#0F0F0F", "quadrant2TextFill": "#0F0F0F", "quadrant3TextFill": "#0F0F0F", "quadrant4TextFill": "#0F0F0F", "quadrantPointFill": "#0F0F0F", "quadrantPointTextFill": "#0F0F0F", "quadrantXAxisTextFill": "#8C8C8C", "quadrantYAxisTextFill": "#8C8C8C", "quadrantTitleFill": "#0F0F0F", "quadrantInternalBorderStrokeFill": "#0F0F0F", "quadrantExternalBorderStrokeFill": "#8C8C8C"}}}%%
quadrantChart
    x-axis "Baja dificultad" --> "Alta dificultad"
    y-axis "Bajo interés" --> "Alto interés"
    quadrant-1 Grandes apuestas
    quadrant-2 Apuestas seguras
    quadrant-3 Relleno
    quadrant-4 Descartar
    Obra: [0.30, 0.70]
    Terreno: [0.40, 0.70]
    Activos: [0.70, 0.80]
    Liquidar: [0.90, 0.80]
```

Anticipos de obra cae en **apuestas seguras**: genera interés y es abordable en el tiempo del bootcamp.

> ⚠️ **Lo que tenemos que vigilar:** es el problema con menos diferencia frente a lo que ya existe (2 de 5), porque en Stellar ya hay proyectos alrededor de pagos condicionados. Por eso nuestro foco estará en quien sufre el problema: familias y maestros de obra que no saben, ni tienen por qué saber, de tecnología. Ahí nos ayuda lo que ya aprendimos del sector con Octoul.

### Propuestas descartadas

| Problema | Lo propuso | Puntaje | Por qué lo descartamos |
|---|---|:-:|---|
| Gastos de terreno que no se pueden demostrar | Jairo | 3,95 | Quedó muy cerca y es el que tiene mejor acceso a usuarios. Lo descartamos porque su pertinencia es la más débil: buena parte del problema se podría resolver con un software tradicional. **Queda como plan B.** |
| Liquidar activos sin exponer la operación | Emanuel | 3,20 | Es el que más le interesa a Stellar, pero el más difícil: llegar a los fondos para validar toma tiempo, la compraventa de estos activos todavía es baja y depende de que los emisores lo permitan. |
| Activos difíciles de comprobar a distancia | Jairo | 3,15 | Tiene urgencia real por la norma europea contra la deforestación (EUDR), pero no tenemos acceso a ganaderos y el reto de la última milla no se resuelve en cinco semanas. |

### Cómo tomamos la decisión

Elegimos **por consenso**, apoyados en dos métodos de selección (el **análisis de decisiones multicriterio** y la **matriz de interés vs. dificultad**), en nuestra **experiencia construyendo en la red de Stellar** y en que el problema es un **micro componente de Octoul**, un proyecto más grande con validación y tracción en el sector.

```mermaid
%%{init: {"theme": "base", "themeVariables": {"fontFamily": "Inter, Helvetica, Arial, sans-serif", "primaryColor": "#F6F7F8", "primaryBorderColor": "#0F0F0F", "primaryTextColor": "#0F0F0F", "lineColor": "#8C8C8C"}}}%%
flowchart LR
    A["Cuatro problemas<br/>dos por integrante"] --> B["Siete criterios<br/>con su peso"]
    B --> C["Nota de 1 a 5<br/>por criterio"]
    C --> D["Segundo escenario<br/>para probar el resultado"]
    D --> E["Matriz de interés<br/>vs. dificultad"]
    E --> F["Consenso: métodos, experiencia<br/>en Stellar y encaje con Octoul"]
    classDef win fill:#FDDA24,stroke:#0F0F0F,color:#0F0F0F
    class F win
```

1. **Cada uno propuso dos problemas** por separado, en su propuesta individual.
2. **Acordamos siete criterios con su peso**, a partir de lo que exige este Problem Brief y de lo que necesitamos para llegar al Demo Day.
3. **Calificamos cada problema de 1 a 5** en cada criterio y calculamos el puntaje ponderado.
4. **Probamos un segundo escenario**, con más peso para Stellar y la diferenciación, para ver si el ganador cambiaba. No cambió.
5. **Ubicamos los cuatro en la matriz** de interés vs. dificultad.
6. **Revisamos el resultado juntos** y, sumando nuestra experiencia en la red de Stellar y el encaje con Octoul, elegimos por consenso Anticipos de obra, con Gastos de terreno como plan B.

---

## Problem Brief

### Encabezado

**BB101 · Anticipos de obra sin garantía**

> En las obras de construcción, desde un edificio hasta la remodelación de una casa, la plata se entrega antes de poder verificar el trabajo hecho, y cuando algo falla nadie puede probar qué se acordó, qué se hizo y qué se pagó.

### Equipo y roles

| Integrante | GitHub | Rol |
|---|---|---|
| Emanuel Benavides León | [@EmanuXBe](https://github.com/EmanuXBe) | Producto y desarrollo: descubrimiento del problema, diseño de la experiencia y construcción técnica |
| Jairo Enrique Amaya Celis | [@jairoamayac](https://github.com/jairoamayac) | Usuarios y negocio: entrevistas, validación con familias y maestros, y modelo de negocio |

- **Responsable de las entregas:** Emanuel Benavides.
- **Coordinación interna:** grupo de WhatsApp del equipo para el día a día y el canal de Discord del bootcamp para las entregas.

### Problema y evidencia

> **En la construcción, la plata sale antes de que alguien pueda verificar el trabajo.** Anticipos, actas de avance y pagos por etapas se mueven sin un registro común de qué se acordó, qué se hizo y qué se pagó, desde un contrato público hasta la remodelación de una casa.

**En cifras:**

| | Cifra | Fuente |
|:-:|---|---|
| 🌎 | La construcción mueve **USD 16,45 billones** al año en el mundo (billones = millones de millones) y **USD 1,14 billones** en Latinoamérica | Estudios de mercado, 2025 |
| 💸 | Entre el **10 % y el 30 %** del valor de un contrato de infraestructura se pierde por mala gestión y corrupción | CoST |
| ⏳ | En EE. UU., los pagos lentos le costaron a la construcción **USD 299.000 millones** en 2025 | Rabbet, 2025 |
| ⚖️ | Una disputa de construcción promedio ya vale **más de USD 60 millones** | Arcadis, 2024 |
| 🇨🇴 | En Colombia hay **1.970 obras públicas inconclusas o críticas** que comprometen **USD 16.400 millones** | Contraloría |

**Frecuencia y alcance.** Pasa en cada obra que arranca con un anticipo. En 2025, la obra pública colombiana firmó **9.806 contratos por USD 5.500 millones**, y **4.456 (USD 250 millones) no tenían que proteger el anticipo** con fiducia. En una remodelación el patrón es idéntico: una familia perdió **USD 6.850** con un maestro que nunca terminó (Séptimo Día).

**Por qué le importa a Stellar:**

- 💵 **Flujo de fondos.** Cada obra es una cadena de pagos recurrente (anticipo, hitos y saldo) entre partes que no confían entre sí.
- 🔌 **Integraciones.** La plata entra y sale en pesos por anchors que ya operan en Colombia (MoneyGram, Bitso) y se apoya en piezas del Integration Track del SCF, como Trustless Work.
- 🧰 **Herramienta para otros desarrolladores.** Comprobar el avance de un trabajo físico es una pieza que no existe en la red; marketplaces, plataformas inmobiliarias y de financiación por hitos podrían reutilizarla.

### Usuario y actores

**Quién sufre el problema.** Son dos, y cada uno carga con el riesgo del otro:

| Usuario | Qué necesita resolver | Cómo lo resuelve hoy | Qué le cuesta |
|---|---|---|---|
| 🏠 **La familia** que remodela | Pagar solo por el trabajo que de verdad se hizo y tener cómo probarlo | Confía en la recomendación, da el anticipo y paga por etapas "según vaya viendo" | La plata del anticipo si el maestro se va, meses de retraso, arriendo extra y años de pleito si decide demandar |
| 🧱 **El maestro de obra** | Tener plata para empezar (materiales y jornales) y la certeza de que le pagarán el saldo | Pide un anticipo y cobra por etapas a medida que avanza | Semanas de trabajo, los jornales de su gente y los materiales si la familia no paga o le pone peros a todo |

**Los demás actores del flujo:**

| Actor | Papel |
|---|---|
| 👷 Cuadrilla de ayudantes | Trabaja en la obra y cobra el jornal al maestro, no a la familia |
| 🔩 Ferretería o depósito | Vende los materiales, con plata del anticipo o directamente a la familia |
| 🏦 Banco o billetera digital | Mueve la plata entre la familia y el maestro; no sabe nada de la obra |
| 🏢 Administración del conjunto | Autoriza la obra, los horarios y el ingreso de materiales cuando es propiedad horizontal |
| 🏛️ Curaduría urbana | Expide la licencia cuando la obra toca la estructura, la fachada o amplía el inmueble |
| 🛡️ Aseguradora | Vende pólizas de cumplimiento, que casi nadie compra para una obra pequeña |
| ⚖️ SIC, Fiscalía o juez | Reciben la queja, la denuncia o la demanda cuando todo falla |

### Flujo actual de valor

Así se mueven hoy la plata (💵), la información y el trabajo en una remodelación típica:

```mermaid
%%{init: {"theme": "base", "themeVariables": {"fontFamily": "Inter, Helvetica, Arial, sans-serif", "primaryColor": "#F6F7F8", "primaryBorderColor": "#0F0F0F", "primaryTextColor": "#0F0F0F", "lineColor": "#8C8C8C", "edgeLabelBackground": "#F6F7F8"}}}%%
flowchart TD
    A["1 · Voz a voz<br/>la familia consigue un maestro"] --> B["2 · Cotización<br/>a ojo, por WhatsApp"]
    B --> C{"¿La obra toca estructura,<br/>fachada o amplía?"}
    C -->|"Sí"| L["3 · Licencia de construcción<br/>en la curaduría"]
    C -->|"No: pisos, enchapes,<br/>pintura o redes"| P["3 · Permiso de la administración<br/>si es un conjunto"]
    L --> D["4 · Anticipo 💵<br/>transferencia o efectivo al maestro"]
    P --> D
    D --> E["5 · Materiales 💵<br/>el maestro compra en la ferretería"]
    E --> F["6 · Obra por etapas 💵<br/>pagos parciales y jornales"]
    F --> G["7 · Entrega y saldo 💵"]
    G -.->|"si hay conflicto"| H["8 · Queja, denuncia<br/>o demanda"]
    classDef money fill:#FDDA24,stroke:#0F0F0F,color:#0F0F0F
    classDef norma fill:#B7ACE8,stroke:#0F0F0F,color:#0F0F0F
    classDef conflict fill:#D6D2C4,stroke:#0F0F0F,color:#0F0F0F
    class D,E,F,G money
    class L,P norma
    class H conflict
```

1. **Voz a voz.** La familia consigue un maestro por recomendación de un vecino o un familiar.
2. **Cotización.** El maestro visita, calcula a ojo y manda el precio por WhatsApp. No suele haber contrato escrito.
3. **Permisos (obligación normativa).** Si la obra modifica la estructura, la fachada o amplía el inmueble, necesita **licencia de construcción** en una curaduría (Decreto 1077 de 2015). Si son reparaciones locativas como pisos, enchapes, pintura o redes, no necesita licencia (Ley 810 de 2003, art. 8), pero en un conjunto sí hace falta el permiso de la administración.
4. **Anticipo.** La familia transfiere o entrega en efectivo una parte grande del valor, antes de ver cualquier avance.
5. **Materiales.** El maestro compra en la ferretería con esa plata, mezclada con la de su mano de obra.
6. **Obra por etapas.** La familia hace pagos parciales "según vaya viendo" y el maestro les paga los jornales a sus ayudantes.
7. **Entrega y saldo.** La familia revisa y paga lo que falta, o lo retiene si no está conforme.
8. **Conflicto.** Si algo sale mal, la salida es una queja ante la SIC, una denuncia por estafa o una demanda.

### Fricciones identificadas

| # | Fricción | Paso | Qué la causa | A quién afecta |
|:-:|---|:-:|---|---|
| F1 | **El anticipo viaja sin respaldo** | 4 | Se paga antes de ver avance, y la única garantía formal (póliza o fiducia) es cara para una obra pequeña | 🏠 Familia |
| F2 | **Nadie sabe cuánto va de verdad** | 6 | No hay una forma acordada de medir el avance; quedan fotos sueltas en el chat | 🏠🧱 Ambos |
| F3 | **La plata de materiales se mezcla** | 5 | El anticipo cubre material y mano de obra sin separar, y no hay soportes | 🏠 Familia |
| F4 | **El saldo se retiene o se regatea** | 7 | No hay un registro común de lo acordado; la familia le puede poner peros a todo | 🧱 Maestro y cuadrilla |
| F5 | **La pelea no tiene pruebas y dura años** | 8 | Los acuerdos fueron de palabra o por chat, y la justicia es lenta y costosa | 🏠🧱 Ambos |

F1 y F2 están en el origen de las demás: como la plata se mueve sin que el avance esté verificado, el saldo termina en discusión (F4) y la disputa no tiene pruebas (F5).

### Oportunidad e hipótesis

**La oportunidad que priorizamos:** amarrar el pago al avance verificado, es decir, F1 y F2 juntas.

**Por qué esta y no otra:** es la raíz del problema. Si cada peso se moviera solo cuando las dos partes reconocen que la obra avanzó, el anticipo dejaría de ser un salto al vacío, el saldo no tendría por qué regatearse y, en una pelea, habría con qué demostrar lo que pasó. Además es la que más pesa para los dos usuarios a la vez: la familia arriesga su plata y el maestro su trabajo en el mismo punto.

**Nuestra hipótesis inicial.** Creemos que un registro compartido podría cambiar la experiencia de esta forma:

| Para | Hoy | Lo que cambiaría |
|---|---|---|
| 🏠 La familia | Entrega el anticipo y cruza los dedos | Sabría que su plata solo avanza cuando la obra avanza, y tendría la historia completa de lo acordado y lo pagado |
| 🧱 El maestro | Empieza sin saber si la plata del saldo existe | Sabría desde el primer día que la plata de la obra está ahí y que le llegará a medida que entregue |
| ⚖️ Ambos, si hay pelea | Es un chat contra otro | Habría un registro que ninguno de los dos pudo cambiar después |

Es una intuición, todavía no una certeza: la vamos a poner a prueba en las entrevistas de esta semana.

### Tamaño del mercado

> La remodelación de una familia es nuestro laboratorio: tiene el mismo patrón (anticipo, avance por etapas y pago contra lo hecho) a una escala que podemos validar en cinco semanas. **El mercado es la contratación de obra**: todo proyecto de construcción en el que la plata se entrega antes de poder verificar el trabajo.

```mermaid
%%{init: {"theme": "base", "themeVariables": {"fontFamily": "Inter, Helvetica, Arial, sans-serif", "primaryColor": "#F6F7F8", "primaryBorderColor": "#0F0F0F", "primaryTextColor": "#0F0F0F", "lineColor": "#8C8C8C"}}}%%
flowchart TD
    TAM["TAM · USD 1,14 billones al año<br/>construcción en Latinoamérica"] --> SAM["SAM · USD 5.500 millones al año<br/>9.806 contratos de obra pública en Colombia"]
    SAM --> ENT["Segmento de entrada · USD 514 millones al año<br/>8.158 contratos de obra pública pequeña"]
    ENT --> SOM["SOM · USD 25,7 millones al año<br/>408 contratos en tres años"]
    classDef tam fill:#D6D2C4,stroke:#0F0F0F,color:#0F0F0F
    classDef sam fill:#B7ACE8,stroke:#0F0F0F,color:#0F0F0F
    classDef som fill:#FDDA24,stroke:#0F0F0F,color:#0F0F0F
    class TAM tam
    class SAM,ENT sam
    class SOM som
```

| Nivel | Qué incluye | Tamaño | Por qué cuenta |
|---|---|---|---|
| 🌎 **TAM** | Toda la construcción en Latinoamérica: edificaciones, vías, obras civiles y remodelaciones | **USD 1,14 billones** al año | En toda obra el pago va por delante de la verificación. Solo Colombia aporta **USD 19.100 millones** de valor agregado, el 4,2 % de su PIB |
| 🏛️ **SAM** | La obra pública contratada en Colombia a través de SECOP II | **USD 5.500 millones** en **9.806 contratos** firmados en 2025 | La ley ya exige trazabilidad (fiducia para el anticipo, interventoría y actas de avance), y aun así falla |
| 🧱 **Segmento de entrada** | Contratos de obra pública de hasta 1.000 salarios mínimos (unos USD 348.000) | **USD 514 millones** en **8.158 contratos**, el 83 % de los contratos de obra | Obras pequeñas, sobre todo municipales, donde una fiducia es desproporcionada o la ley ni siquiera la exige |
| 🎯 **SOM** | El 5 % del segmento de entrada en tres años | **USD 25,7 millones** al año en unos **408 contratos** | Es el valor de obra que pasaría por la red: cada anticipo, hito y pago quedaría verificable |

**El tamaño del dolor.** La Contraloría tiene identificadas **1.970 obras públicas inconclusas o críticas por USD 16.400 millones** (entre septiembre de 2022 y julio de 2026). De ellas, 1.029 por **USD 13.250 millones** siguen con problemas de ejecución y 134 por **USD 153 millones** ya se consideran irrecuperables. Si al gasto anual en obra pública le aplicamos el rango de pérdida de CoST (10 % a 30 %), entre **USD 550 y 1.650 millones** al año se irían solo en Colombia.

**Por qué entramos por la obra pequeña.** La Ley 1474 de 2011 (art. 91) obliga a manejar el anticipo de los contratos de obra con una fiducia, **salvo en los de menor y mínima cuantía**. En 2025 esos contratos exentos fueron **4.456 por USD 250 millones**. Ahí el anticipo viaja sin respaldo, igual que en la remodelación de una familia, y un registro compartido y barato compite con una fiducia que cuesta más de lo que vale controlar una obra chica.

**De la obra pequeña a Octoul.** Lo que probemos con anticipos e hitos en obras pequeñas es la base para verificar el avance de proyectos más grandes, donde la fiducia ya existe pero no ve la obra: controla en qué se gasta el anticipo, no si el trabajo se hizo.

> ⚠️ **El SOM es una hipótesis.** El 5 % es una meta del equipo, no un dato: la vamos a contrastar con el modelo de negocio de la semana 2.

<details>
<summary><b>Cómo calculamos estas cifras</b></summary>

- **Tasa de cambio.** Convertimos todas las cifras en pesos con la **TRM promedio de 2025: COP 4.088 por dólar** (Portafolio), porque los datos de base son de 2025. Es un criterio conservador: con la TRM del 5 de octubre de 2026 (COP 3.273) las cifras en dólares serían cerca de un 25 % más altas.
- **TAM.** Tamaño del mercado de construcción en Latinoamérica en 2025, según Expert Market Research. Como referencia, el valor agregado de la construcción en Colombia en 2025 fue de COP 77,9 billones (DANE, cifra preliminar, vía El Colombiano), unos USD 19.100 millones.
- **SAM y segmento de entrada.** Base abierta *SECOP II, Contratos Electrónicos* (datos.gov.co), consultada el 5 de octubre de 2026: contratos con tipo "Obra" y fecha de firma en 2025. SAM: COP 22,5 billones. Segmento de entrada: COP 2,1 billones.
  - Excluimos 32 contratos etiquetados como "Selección abreviada de menor cuantía sin manifestación de interés" por COP 669.500 millones (USD 164 millones), porque sus valores superan el tope legal de esa modalidad.
  - Obra pequeña: hasta 1.000 salarios mínimos de 2025, es decir, COP 1.423.500.000, el tope de menor cuantía para las entidades más grandes.
  - Contratos exentos de fiducia: 2.697 de menor cuantía por COP 932.806 millones (USD 228 millones) y 1.759 de mínima cuantía por COP 87.153 millones (USD 21 millones), filtrados con sus topes legales.
  - Los contratos que todavía se registran en SECOP I quedan por fuera, así que estas cifras son un piso.
- **SOM.** 5 % de los 8.158 contratos de obra pequeña y de sus USD 514 millones.
- **Pérdida estimada.** Rango de CoST (10 % a 30 %) aplicado a los USD 5.500 millones de obra pública de 2025. Es una estimación de orden de magnitud, no una medición.

</details>

### Criterio de pertinencia

**¿Por qué no basta una base de datos o una app tradicional?** Porque la pregunta clave es **quién la controla**.

- Si el registro lo lleva **el maestro** o **la familia**, la otra parte no tiene por qué creerle.
- Si lo lleva **una plataforma**, que además guarda la plata, aparece un nuevo intermediario que concentra la confianza y cobra por ello. Eso ya existe (la fiducia y la póliza de cumplimiento), y por caro no llega a las obras pequeñas.
- Integrar los sistemas existentes tampoco resuelve nada: hoy no hay sistemas que integrar, solo chats, transferencias y papeles.

El caso cumple los **tres criterios de la Sesión 1**:

| Criterio | Cómo aplica |
|---|---|
| 🤝 Partes que no confían entre sí comparten un registro | La familia y el maestro casi nunca se conocen de antes y cada uno asume el riesgo de que el otro incumpla |
| 🔒 Histórico inalterable | Lo acordado, lo aprobado y lo pagado tiene que quedar fijo, porque es la prueba si hay disputa |
| ✂️ Eliminar un intermediario que concentra la confianza | Hoy el único tercero que da garantías (fiducia o aseguradora) es inaccesible para una remodelación |

Siguiendo la regla de la Sesión 1, **en la red solo iría lo que varias partes necesitan verificar**: los montos, los hitos acordados, las aprobaciones y la huella de la evidencia. Las fotos, los nombres, las cédulas y las conversaciones se quedan en una base de datos tradicional.

### Supuestos y riesgos

**Supuestos que tendrían que ser ciertos:**

| # | Supuesto | Qué lo invalidaría |
|:-:|---|---|
| S1 | **El problema es frecuente**, no solo un puñado de casos de televisión | Que en las entrevistas la mayoría de familias y maestros cuente que sus obras terminaron bien solo con la confianza |
| S2 | **La familia y el maestro aceptarían comprometer la plata desde el inicio** y moverla por etapas | Que el maestro necesite libre todo el anticipo para materiales y no acepte trabajar de otra forma |
| S3 | **Las peleas son por avance y pago, no solo por calidad** | Que la mayoría de conflictos sean sobre si algo quedó "bien hecho", algo subjetivo que un registro de avance no resuelve |

**Riesgos:**

- **Adopción.** Familias y maestros no saben, ni tienen por qué saber, de tecnología. Si la experiencia no es tan simple como mandar un WhatsApp, no la van a usar.
- **Competencia.** En Stellar ya existen proyectos alrededor de pagos condicionados. Nuestra diferencia tiene que estar en el usuario: la familia y el maestro de obra colombianos.
- **Regulación.** Guardar plata de terceros puede tener implicaciones legales en Colombia. Lo vamos a revisar antes de diseñar.

<details>
<summary><b>Fuentes</b></summary>

- Reportaje de Séptimo Día (Caracol Televisión) sobre remodelaciones pagadas y sin terminar, con cifras de la Superintendencia de Industria y Comercio (quejas entre enero de 2022 y mayo de 2026) y recomendaciones de expertos.
- DANE, Gran Encuesta Integrada de Hogares, informalidad laboral a junio de 2026, vía [Portafolio](https://www.portafolio.co/economia/mientras-que-el-desempleo-en-colombia-baja-de-los-dos-digitos-la-informalidad-no-cede-del-491084).
- Reparaciones locativas y licencias de construcción, Decreto 1077 de 2015 y Ley 810 de 2003, art. 8, según [concepto de la Curaduría Urbana 3 de Bogotá](https://curaduria3bogota.com/wp-content/uploads/2024/12/CONCEPTO-R23-3-0240.pdf).
- DANE, Producto Interno Bruto 2025, aporte de la construcción, vía [El Colombiano](https://www.elcolombiano.com/negocios/pib-colombia-2025-valor-pesos-datos-dane-EG33602701), y variación del sector en el [boletín técnico del IV trimestre de 2025](https://www.dane.gov.co/files/operaciones/PIB/bol-PIB-IVtrim2025.pdf).
- Mercado global de construcción 2025 (USD 16,45 billones), [ResearchAndMarkets vía Business Wire](https://www.businesswire.com/news/home/20251002308109/en/Construction-Industry-Report-2025-Global-Market-to-Reach-%2420.44-Trillion-in-2029-from-%2415.78-Trillion-in-2024---Long-term-Forecast-to-2034---ResearchAndMarkets.com), y mercado de construcción en Latinoamérica 2025, [Expert Market Research](https://www.expertmarketresearch.com/es/reports/latin-america-construction-market).
- Pérdida del 10 % al 30 % del valor de los contratos de infraestructura, [Banco Mundial sobre CoST](https://www.worldbank.org/en/news/feature/2012/11/08/construction-sector-transparency-program-goes-global).
- Costo de los pagos lentos en la construcción de EE. UU., [Rabbet, 2025 Construction Payments Report](https://rabbet.com/reports/construction-payments-2025).
- Valor promedio de las disputas de construcción, Arcadis, vía [Pinsent Masons](https://www.pinsentmasons.com/out-law/news/arcadis-global-construction-value-disputes).
- TRM promedio de 2025, [Portafolio](https://www.portafolio.co/economia/finanzas/precio-del-dolar-en-colombia-cerro-el-2025-en-3-757-marcado-por-la-revalorizacion-del-peso-local-485476).
- Trustless Work en el Integration Track del SCF, [Trustless Work](https://www.trustlesswork.com/escrow-times/news-scf-integration-track).
- Agencia Nacional de Contratación Pública (Colombia Compra Eficiente), [SECOP II, Contratos Electrónicos](https://www.datos.gov.co/Estad-sticas-Nacionales/SECOP-II-Contratos-Electr-nicos/jbjy-vk9h), contratos de obra firmados en 2025, consultado el 5 de octubre de 2026.
- Ley 1474 de 2011, art. 91, sobre el manejo de anticipos con fiducia, en la [síntesis normativa de Colombia Compra Eficiente](https://sintesis.colombiacompra.gov.co/norma/LEY%201474%20DE%202011/258).
- Contraloría General de la República, obras inconclusas y críticas entre septiembre de 2022 y julio de 2026, vía [Infobae](https://www.infobae.com/colombia/2026/07/12/colombia-acumula-1970-elefantes-blancos-por-67-billones-estas-son-las-obras-que-dejo-inconclusas-el-gobierno-petro/).

</details>
