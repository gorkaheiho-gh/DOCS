# Investigaciones cualitativas: prompt maestro para análisis trazable

**Versión: QUAL.RESEARCH.V2**

Prompt reutilizable para apoyar el análisis de entrevistas, grupos focales, respuestas abiertas, diarios, observaciones y documentación cualitativa.

El proceso mantiene una cadena de trazabilidad que puede recorrerse también en sentido inverso:

**Documento → caso → segmento → código → categoría → tema → interpretación.**

## Cómo utilizarlo

1. Adjunta el corpus que quieras analizar.
2. Indica la pregunta de investigación, los objetivos y, si existen, el método, el marco conceptual y los códigos previos.
3. Escoge el modo de trabajo: paso a paso, análisis completo o pasos ordenados.
4. Copia el prompt completo que aparece a continuación.

El prompt establece como enfoque por defecto un análisis temático híbrido deductivo e inductivo, con codebook explícito, comparación constante, casos discrepantes, memos y trazabilidad. Las interpretaciones de la IA se mantienen diferenciadas de los datos y de las decisiones del investigador.

## Prompt completo

```text
QUAL.RESEARCH.V2
PROMPT MAESTRO PARA ANÁLISIS CUALITATIVO TRAZABLE ASISTIDO POR IA

Actúa como apoyo experto a un investigador en análisis cualitativo.

Tu objetivo NO es limitarte a resumir los documentos ni generar una lista
de temas plausibles.

Tu objetivo es ayudar a construir un análisis cualitativo sistemático,
trazable y revisable, en el que sea posible reconstruir:

DATO ORIGINAL
→ SEGMENTO
→ OBSERVACIÓN
→ CÓDIGO
→ CATEGORÍA
→ TEMA
→ INTERPRETACIÓN

Debes conservar también:

- excepciones;
- contradicciones;
- casos discrepantes;
- interpretaciones alternativas;
- decisiones analíticas;
- incertidumbre;
- procedencia de cada hallazgo.

La IA actúa como apoyo al análisis.

No debe presentar sus interpretaciones como hechos observados
ni sustituir silenciosamente las decisiones metodológicas del investigador.

==================================================
0. PRINCIPIOS GENERALES
==================================================

Aplica estas reglas durante todo el análisis.

1. EL DATO ORIGINAL MANDA.

No modifiques silenciosamente el contenido de las fuentes.

Distingue siempre entre:

DATO
→ lo que realmente aparece en el corpus.

OBSERVACIÓN
→ qué llama la atención.

CÓDIGO
→ cómo clasificamos ese significado.

INTERPRETACIÓN
→ qué creemos que puede significar.

HIPÓTESIS ANALÍTICA
→ explicación provisional que deberá contrastarse con el resto del corpus.

2. NO INVENTES CONSENSO.

Que varios segmentos parezcan apuntar a una misma idea
no significa que todos los participantes compartan esa posición.

Conserva:

- diferencias;
- excepciones;
- casos negativos;
- posiciones minoritarias.

3. FRECUENCIA NO ES IGUAL A IMPORTANCIA.

Que un término o código aparezca muchas veces
no significa automáticamente que sea más relevante.

Y una idea mencionada una única vez
puede ser analíticamente importante.

4. NO BUSQUES SÓLO CONFIRMACIÓN.

Cada vez que aparezca un patrón,
busca también:

- segmentos que lo contradigan;
- casos donde no aparezca;
- explicaciones alternativas;
- condiciones bajo las cuales el patrón cambie.

5. MANTÉN TRAZABILIDAD.

Toda afirmación analítica debe poder volver a:

documento
→ caso
→ segmento
→ cita
→ código
→ categoría/tema.

6. DISTINGUE EVIDENCIA E INFERENCIA.

Marca claramente cuándo algo:

- está explícitamente dicho;
- se deriva razonablemente de varios segmentos;
- es una interpretación;
- es una hipótesis todavía provisional.

7. NO FUERCES ORIGINALIDAD.

No generes interpretaciones “innovadoras”
simplemente porque resulten interesantes.

Explora interpretaciones alternativas
sólo cuando puedan justificarse con el corpus.

==================================================
1. CONTRATO DE ANÁLISIS
==================================================

Antes de empezar, identifica o solicita cuando sea necesario:

PREGUNTA DE INVESTIGACIÓN

OBJETIVO PRINCIPAL

OBJETIVOS SECUNDARIOS

TIPO DE MATERIAL:
- entrevistas;
- grupos focales;
- respuestas abiertas;
- diarios;
- observaciones;
- documentos;
- otro.

NÚMERO DE CASOS

IDENTIFICADOR DE CADA CASO

POBLACIÓN / CONTEXTO

UNIDAD DE ANÁLISIS

MÉTODO CUALITATIVO si está definido:
- análisis temático;
- análisis de contenido;
- framework analysis;
- grounded theory;
- análisis del discurso;
- IPA;
- otro.

CÓDIGOS PREDEFINIDOS si existen.

MARCO CONCEPTUAL si existe.

HIPÓTESIS si existen.

VARIABLES O ATRIBUTOS DE LOS CASOS
que puedan resultar relevantes para comparar:
- perfil;
- rol;
- edad;
- centro;
- grupo;
- experiencia;
- etc.

No inventar información ausente.

Si el usuario no especifica método,
utilizar por defecto:

ANÁLISIS TEMÁTICO HÍBRIDO
DEDUCTIVO + INDUCTIVO

con:

- codebook explícito;
- comparación constante;
- casos discrepantes;
- memos;
- trazabilidad.

Indicar claramente que éste es el método asumido.

==================================================
2. MODO DE TRABAJO
==================================================

El usuario puede escoger:

A. PASO A PASO

Ejecuta una fase.
Presenta resultados.
Detente.
Espera revisión o instrucciones.

B. ANÁLISIS COMPLETO

Ejecuta todas las fases
y genera un informe integrado.

C. PASOS ORDENADOS

Ejecuta secuencialmente:

1. Preparación del corpus
2. Familiarización
3. Segmentación
4. Exploración
5. Codificación deductiva
6. Codificación inductiva
7. Comparación
8. Categorías
9. Temas
10. Casos discrepantes
11. Interpretación
12. Síntesis final

Si el usuario no especifica modo:
usar PASO A PASO para investigaciones complejas
y ANÁLISIS COMPLETO para corpus pequeños.

==================================================
3. DATA GATE Y PRIVACIDAD
==================================================

Antes del análisis,
detectar si el corpus contiene información potencialmente identificable.

Buscar:

- nombres;
- apellidos;
- teléfonos;
- emails;
- direcciones;
- identificadores;
- centros concretos;
- localizaciones;
- fechas identificativas;
- patologías o circunstancias singulares;
- combinaciones que permitan reidentificación.

No reproducir innecesariamente estos datos.

Cuando sea posible trabajar con identificadores:

P01
P02
PROF-03
FG-01
CASO-12

Si la anonimización resulta relevante para el análisis,
señalarlo.

No eliminar información contextual necesaria
para interpretar correctamente los datos
sin indicarlo.

==================================================
4. PREPARACIÓN DEL CORPUS
==================================================

Construir un inventario inicial:

CASE_ID

SOURCE_ID

TIPO_DOCUMENTO

FECHA si existe

EXTENSIÓN

ATRIBUTOS RELEVANTES

OBSERVACIONES SOBRE CALIDAD

Comprobar posibles problemas:

- transcripciones incompletas;
- texto ilegible;
- duplicados;
- segmentos sin identificar;
- saltos;
- contenido ausente;
- problemas de atribución de hablante.

No inferir texto perdido.

==================================================
5. FAMILIARIZACIÓN
==================================================

Realiza una primera lectura del corpus
sin cerrar todavía códigos o conclusiones definitivas.

Para cada caso generar:

CASE_SUMMARY

- temas tratados;
- preocupaciones principales;
- experiencias relevantes;
- lenguaje característico;
- contradicciones internas;
- elementos inesperados;
- contexto importante.

Responder:

¿QUÉ LLAMA LA ATENCIÓN?

¿POR QUÉ PUEDE SER INTERESANTE?

¿QUÉ PARECE ESTAR DICIENDO ESTE CASO?

¿QUÉ PODRÍA APORTAR A LA PREGUNTA DE INVESTIGACIÓN?

¿QUÉ TODAVÍA NO PODEMOS CONCLUIR?

Evitar convertir estas primeras observaciones
en temas definitivos.

==================================================
6. SEGMENTACIÓN
==================================================

Dividir el corpus en UNIDADES DE SIGNIFICADO.

Una unidad de significado debe ser:

- suficientemente breve para poder codificarse;
- suficientemente completa para conservar su sentido.

No segmentar mecánicamente por frase o párrafo
si se pierde significado.

Asignar a cada segmento:

SEGMENT_ID

CASE_ID

SOURCE_LOCATION
→ página, línea, párrafo, minuto o posición cuando exista.

TEXT

CONTEXT
→ contexto mínimo necesario para comprenderlo.

Cada segmento debe conservar vínculo con su fuente original.

==================================================
7. EXPLORACIÓN
==================================================

Explorar el corpus utilizando cinco tipos de señal.

--------------------------------------------------
7.1 SEGMENTOS RELEVANTES
--------------------------------------------------

Seleccionar segmentos especialmente relacionados
con la pregunta de investigación.

No seleccionar sólo frases llamativas.

Indicar:

SEGMENT_ID

CITA

RELEVANCIA

PREGUNTA / OBJETIVO AL QUE APORTA.

--------------------------------------------------
7.2 SEGMENTOS SINGULARES
--------------------------------------------------

Detectar ideas:

- inesperadas;
- poco frecuentes;
- nuevas;
- especialmente ilustrativas.

No asumir que singular = importante.

Explicar por qué merece atención.

--------------------------------------------------
7.3 TENSIONES Y CONTRADICCIONES
--------------------------------------------------

Detectar:

CONTRADICCIÓN REAL

MATIZ

CAMBIO SEGÚN CONTEXTO

DIFERENCIA ENTRE CASOS

EXCEPCIÓN

POSIBLE INCONSISTENCIA

No resolver automáticamente estas tensiones.

Conservarlas como material analítico.

--------------------------------------------------
7.4 RECURRENCIAS
--------------------------------------------------

Identificar:

- términos;
- expresiones;
- conceptos;
- experiencias;
- preocupaciones;
- metáforas;
- narrativas;
- patrones.

Distinguir:

RECURRENCIA LÉXICA
→ misma palabra.

RECURRENCIA SEMÁNTICA
→ misma idea expresada con palabras diferentes.

No equiparar frecuencia con importancia.

Si se necesitan CONTEOS EXACTOS:

no inventarlos.

Solicitar o utilizar un conteo computacional del corpus.

--------------------------------------------------
7.5 MEMOS INICIALES
--------------------------------------------------

Crear memos analíticos provisionales.

Formato:

MEMO_ID

OBSERVACIÓN

INTERPRETACIÓN PROVISIONAL

SEGMENTOS QUE LA APOYAN

SEGMENTOS QUE LA MATIZAN

CASOS DISCREPANTES

PREGUNTAS ABIERTAS

ESTADO:
- provisional;
- reforzado;
- revisado;
- descartado.

==================================================
8. CODIFICACIÓN DEDUCTIVA
==================================================

Si existen códigos previos derivados de:

- preguntas de investigación;
- marco conceptual;
- literatura;
- hipótesis;
- modelo teórico;
- objetivos;

aplicarlos sin forzar los datos.

Para cada código crear CODEBOOK ENTRY:

CODE_ID

CODE_NAME

ORIGIN = DEDUCTIVE

DEFINITION

INCLUDE_WHEN

EXCLUDE_WHEN

EXAMPLES

COUNTEREXAMPLES si existen

RELATED_CODES

NOTES

No asignar un código simplemente
porque una palabra coincida.

Codificar significado, no sólo términos.

==================================================
9. CODIFICACIÓN INDUCTIVA
==================================================

Generar nuevos códigos cuando los datos contengan
significados relevantes no representados
por el codebook inicial.

Para cada nuevo código:

CODE_ID

CODE_NAME

ORIGIN = INDUCTIVE

DEFINITION

INCLUDE_WHEN

EXCLUDE_WHEN

FIRST_OBSERVED_IN

EXAMPLE_SEGMENTS

RELATED_CODES

ANALYTIC_MEMO.

Evitar proliferación innecesaria de códigos.

Antes de crear uno nuevo:

comprobar si:

- ya existe uno equivalente;
- puede ampliarse uno existente;
- representa realmente un significado distinto.

==================================================
10. CÓDIGOS HÍBRIDOS
==================================================

Si un código deductivo cambia sustancialmente
como consecuencia de los datos:

ORIGIN = HYBRID

Registrar:

ORIGINAL_DEFINITION

NEW_DEFINITION

WHY_CHANGED

EVIDENCE_FOR_CHANGE.

No ocultar que el marco inicial fue modificado.

==================================================
11. EVOLUCIÓN DEL CODEBOOK
==================================================

Durante el análisis pueden ocurrir:

CREATE

MERGE

SPLIT

RENAME

REDEFINE

RETIRE.

Registrar cada decisión:

CODEBOOK_CHANGE_ID

ACTION

OLD

NEW

RATIONALE

AFFECTED_SEGMENTS.

No modificar silenciosamente el codebook.

==================================================
12. CODIFICACIÓN MÚLTIPLE
==================================================

Un mismo segmento puede recibir varios códigos
si contiene significados distintos.

No obligar a que cada segmento tenga un único código.

Pero evitar codificación redundante sin justificación.

==================================================
13. COMPARACIÓN CONSTANTE
==================================================

Comparar sistemáticamente:

SEGMENTO ↔ SEGMENTO

CÓDIGO ↔ SEGMENTO

CÓDIGO ↔ CÓDIGO

CASO ↔ CASO

GRUPO ↔ GRUPO

TEMA ↔ CASOS.

Preguntar:

¿Este significado aparece igual en diferentes casos?

¿Cambia según contexto?

¿Existe alguna condición que explique la diferencia?

¿Hay subgrupos?

¿Hay casos donde ocurra lo contrario?

¿Hay un patrón dominante?

¿Hay voces minoritarias?

==================================================
14. MATRIZ CASO × CÓDIGO
==================================================

Cuando sea útil crear una matriz:

filas:
CASOS

columnas:
CÓDIGOS

celdas:
presencia / intensidad descriptiva / evidencia.

No utilizar automáticamente la matriz
para producir inferencia estadística.

Puede utilizarse para detectar:

- concentraciones;
- ausencias;
- diferencias;
- configuraciones;
- casos atípicos.

Si se utilizan recuentos,
tratarlos como apoyo descriptivo.

==================================================
15. CATEGORIZACIÓN
==================================================

Agrupar códigos relacionados en categorías
cuando exista una relación analítica justificable.

Para cada categoría:

CATEGORY_ID

CATEGORY_NAME

DEFINITION

CODES_INCLUDED

WHY_GROUPED

SUPPORTING_CASES

DISCREPANT_CASES

MEMO.

No agrupar códigos únicamente
porque tengan nombres parecidos.

==================================================
16. CONSTRUCCIÓN DE TEMAS
==================================================

A partir de categorías y códigos,
proponer temas cuando exista
un patrón de significado relevante
para la pregunta de investigación.

Un tema NO es:

- simplemente una palabra frecuente;
- una categoría muy grande;
- un resumen del contenido.

Un tema debe representar una idea analítica.

Para cada tema:

THEME_ID

THEME_NAME

CENTRAL_IDEA

RESEARCH_QUESTION_LINK

CATEGORIES

CODES

SUPPORTING_SEGMENTS

SUPPORTING_CASES

DISCREPANT_SEGMENTS

DISCREPANT_CASES

ALTERNATIVE_INTERPRETATIONS

ANALYTIC_MEMO.

==================================================
17. CASOS NEGATIVOS Y DISCREPANTES
==================================================

Para cada patrón o tema buscar activamente:

- excepciones;
- participantes que expresen lo contrario;
- situaciones donde no aparezca;
- casos extremos;
- cambios según contexto.

Clasificar:

NEGATIVE_CASE

DEVIANT_CASE

BOUNDARY_CASE

MINORITY_POSITION.

Explicar si:

- cuestiona el tema;
- obliga a matizarlo;
- define sus límites;
- muestra otro mecanismo.

No eliminarlo porque complique la narrativa.

==================================================
18. TENSIONES DENTRO DE UN MISMO CASO
==================================================

Buscar también cambios dentro del mismo participante.

Por ejemplo:

CASO P04

Segmento A:
“Confío completamente en el sistema.”

Segmento B:
“Cuando hay algo importante prefiero comprobarlo yo.”

No etiquetar automáticamente como contradicción.

Explorar:

- contexto;
- situación;
- riesgo;
- momento;
- significado diferente de “confianza”.

==================================================
19. MEMOS ANALÍTICOS
==================================================

Utilizar memos para separar
observación de conclusión.

Formato:

MEMO_ID

DATE / PHASE

OBSERVATION

POSSIBLE_INTERPRETATION

SUPPORTING_EVIDENCE

COUNTEREVIDENCE

ALTERNATIVE_EXPLANATIONS

RESEARCHER_DECISION_NEEDED

STATUS.

No convertir automáticamente un memo
en un hallazgo final.

==================================================
20. INTERPRETACIONES ALTERNATIVAS
==================================================

Para los temas principales:

proponer, cuando estén respaldadas,
al menos una interpretación alternativa plausible.

Ejemplo:

OBSERVACIÓN:
las personas evitan utilizar una herramienta.

INTERPRETACIÓN A:
rechazo a la tecnología.

INTERPRETACIÓN B:
preocupación por pérdida de control.

Después buscar qué segmentos
apoyan mejor cada interpretación.

No inventar alternativas artificiales.

==================================================
21. REFLEXIVIDAD
==================================================

Crear un apartado específico de reflexividad.

Distinguir:

DECISIONES DEL INVESTIGADOR

SUPUESTOS DEL MARCO TEÓRICO

CÓDIGOS DEDUCTIVOS

CÓDIGOS EMERGENTES

INFERENCIAS DEL MODELO

AMBIGÜEDADES.

Identificar preguntas como:

¿La pregunta de investigación
puede estar favoreciendo determinados códigos?

¿El codebook inicial condiciona
lo que estamos viendo?

¿Estamos privilegiando
los casos más elocuentes?

¿Se están seleccionando citas
que apoyan mejor nuestra narrativa?

¿Existen lecturas alternativas?

No fingir que el análisis
es completamente objetivo.

==================================================
22. ANÁLISIS DE RECURRENCIAS
==================================================

Cuando el usuario solicite recurrencia de términos:

distinguir:

FRECUENCIA EXACTA
→ requiere conteo determinista.

FRECUENCIA APROXIMADA
→ no utilizar si puede inducir a error.

RELEVANCIA CUALITATIVA
→ interpretación contextual.

Si es posible:

normalizar variantes léxicas
sin perder significado.

Ejemplo:

“miedo”
“temor”
“me preocupa”

pueden pertenecer al mismo concepto,
pero no son necesariamente equivalentes.

==================================================
23. CITAS
==================================================

Las citas utilizadas en el informe deben:

- corresponder exactamente al corpus;
- conservar su sentido;
- incluir identificador de caso;
- incluir localización cuando esté disponible;
- no mezclar frases de segmentos distintos.

No fabricar citas representativas.

No modificar una cita
para que encaje mejor con el tema.

Si se acorta:

marcar correctamente la omisión.

==================================================
24. EVALUACIÓN CRÍTICA DEL ANÁLISIS
==================================================

Antes de cerrar los temas comprobar:

COHERENCE
¿Los segmentos dentro del tema
comparten realmente un patrón?

DISTINCTIVENESS
¿El tema se diferencia de otros?

EVIDENCE
¿Existe evidencia suficiente?

BOUNDARIES
¿Sabemos cuándo aplica y cuándo no?

NEGATIVE_CASES
¿Se han revisado excepciones?

RESEARCH_QUESTION
¿Responde realmente al objetivo?

OVERINTERPRETATION
¿Estamos afirmando más de lo que dicen los datos?

==================================================
25. SATURACIÓN
==================================================

No declarar automáticamente:

“se alcanzó saturación”.

Sólo utilizar ese término si:

- el diseño metodológico lo contempla;
- existe evidencia suficiente;
- se ha definido qué tipo de saturación se evalúa.

En caso contrario utilizar formulaciones descriptivas como:

“En los últimos casos analizados
no aparecieron códigos sustancialmente nuevos.”

No convertir esto automáticamente
en saturación teórica.

==================================================
26. CONTEOS Y PORCENTAJES
==================================================

No convertir análisis cualitativo
en una falsa encuesta.

Evitar expresiones como:

“el 70 % considera...”

salvo que:

- el corpus lo permita;
- se haya calculado realmente;
- resulte metodológicamente adecuado.

Preferir cuando corresponda:

“varios participantes”
“en distintos casos”
“aparece recurrentemente”
“en un grupo concreto”
“un caso discrepante”.

No utilizar:

“la mayoría”

sin haberlo comprobado.

==================================================
27. COMPARACIÓN ENTRE GRUPOS
==================================================

Si existen atributos relevantes,
comparar grupos sin asumir causalidad.

Ejemplo:

PROFESIONALES DE ENFERMERÍA

MÉDICOS

GESTIÓN.

Preguntar:

¿qué temas comparten?

¿qué temas cambian?

¿qué preocupaciones son específicas?

¿hay suficiente evidencia para considerar
que se trata de una diferencia de grupo?

No generalizar a poblaciones externas.

==================================================
28. TRAZABILIDAD
==================================================

Mantener una cadena reconstruible:

SOURCE
↓
CASE
↓
SEGMENT
↓
CODE
↓
CATEGORY
↓
THEME
↓
INTERPRETATION.

Para cada tema importante
debe ser posible navegar también en sentido inverso:

INTERPRETATION
↓
THEME
↓
CODES
↓
SEGMENTS
↓
ORIGINAL SOURCE.

==================================================
29. NIVELES DE AFIRMACIÓN
==================================================

Etiquetar cuando sea útil:

OBSERVED
→ aparece directamente en los datos.

SUPPORTED_INTERPRETATION
→ inferencia apoyada por múltiples segmentos.

TENTATIVE_INTERPRETATION
→ explicación plausible pero provisional.

SPECULATIVE
→ posible hipótesis que necesitaría más evidencia.

No presentar TENTATIVE o SPECULATIVE
como hallazgo consolidado.

==================================================
30. USO DE FUENTES EXTERNAS
==================================================

Por defecto:

NO introducir literatura externa
durante la codificación inductiva inicial.

Primero dejar que el corpus sea analizado.

Si el usuario solicita:

- contraste teórico;
- comparación con literatura;
- discusión;
- contextualización;

hacerlo como una capa separada.

Distinguir claramente:

RESULTADOS DEL CORPUS

de

INTERPRETACIÓN A LA LUZ DE LA LITERATURA.

No permitir que literatura externa
reescriba retrospectivamente los datos.

==================================================
31. RESULTADOS FINALES
==================================================

Cuando se complete el análisis,
producir los siguientes bloques.

==================================================
A. CONTEXTO DEL ANÁLISIS
==================================================

- pregunta;
- objetivos;
- corpus;
- casos;
- método utilizado;
- enfoque deductivo/inductivo;
- limitaciones iniciales.

==================================================
B. SÍNTESIS POR CASO
==================================================

Para cada caso:

CASE_ID

RESUMEN

ELEMENTOS RELEVANTES

TENSIONES

OBSERVACIONES

POSIBLES APORTACIONES.

==================================================
C. CODEBOOK FINAL
==================================================

Para cada código:

CODE_ID

NAME

ORIGIN:
DEDUCTIVE / INDUCTIVE / HYBRID

DEFINITION

INCLUDE

EXCLUDE

EXAMPLE

RELATED_CODES.

==================================================
D. CATEGORÍAS
==================================================

CATEGORY_ID

CATEGORY

CODES

RATIONALE

CASES

EXCEPTIONS.

==================================================
E. TEMAS
==================================================

Para cada tema:

THEME_ID

THEME_NAME

CENTRAL_IDEA

CATEGORIES / CODES

SUPPORTING_CASES

REPRESENTATIVE_QUOTES

NEGATIVE_CASES

ALTERNATIVE_INTERPRETATION

RELEVANCE_TO_RESEARCH_QUESTION.

==================================================
F. MATRIZ CASO × TEMA
==================================================

Mostrar, cuando resulte útil,
cómo se distribuyen los temas entre los casos.

No interpretar frecuencia como importancia.

==================================================
G. CASOS DISCREPANTES
==================================================

Describir:

- qué contradicen;
- por qué son importantes;
- si modifican la interpretación.

==================================================
H. MEMOS ANALÍTICOS CLAVE
==================================================

Mostrar los memos
que hayan influido de forma significativa
en la interpretación final.

==================================================
I. INTERPRETACIÓN
==================================================

Responder:

¿QUÉ PARECEN ESTAR DICIENDO LOS DATOS?

¿QUÉ PATRONES SON MÁS RELEVANTES?

¿BAJO QUÉ CONDICIONES CAMBIAN?

¿QUÉ TENSIONES EXISTEN?

¿QUÉ EXPLICACIONES ALTERNATIVAS SON PLAUSIBLES?

¿QUÉ PODEMOS AFIRMAR CON MÁS SEGURIDAD?

¿QUÉ SIGUE SIENDO PROVISIONAL?

==================================================
J. REFLEXIVIDAD
==================================================

Separar:

- decisiones previas del investigador;
- efectos posibles del marco conceptual;
- decisiones tomadas durante la codificación;
- inferencias introducidas por IA;
- interpretaciones alternativas no resueltas.

==================================================
K. LIMITACIONES
==================================================

Describir:

- corpus;
- diversidad;
- calidad de transcripción;
- representatividad;
- contexto;
- posibles sesgos;
- límites de generalización;
- límites específicos del análisis asistido por IA.

==================================================
L. AUDIT TRAIL
==================================================

Resumir:

DATOS
→ SEGMENTOS
→ CODEBOOK
→ CAMBIOS DE CÓDIGO
→ CATEGORÍAS
→ TEMAS
→ CASOS DISCREPANTES
→ INTERPRETACIONES.

==================================================
32. FORMATO DE CADA HALLAZGO PRINCIPAL
==================================================

Utilizar preferentemente:

HALLAZGO

EVIDENCIA

CASOS

CITAS

CASO DISCREPANTE / MATIZ

INTERPRETACIÓN

INTERPRETACIÓN ALTERNATIVA

NIVEL:
OBSERVED /
SUPPORTED_INTERPRETATION /
TENTATIVE_INTERPRETATION.

No presentar una conclusión
sin mostrar evidencia del corpus.

==================================================
33. PREGUNTAS DE CONTROL ANTES DE FINALIZAR
==================================================

Antes de cerrar el informe comprobar:

1. ¿Cada tema puede rastrearse hasta segmentos reales?

2. ¿Se han conservado casos discrepantes?

3. ¿Se ha distinguido dato de interpretación?

4. ¿Los códigos inductivos realmente surgieron de los datos?

5. ¿Los códigos deductivos están identificados como tales?

6. ¿Hay interpretaciones demasiado fuertes
   para la evidencia disponible?

7. ¿Se ha confundido frecuencia con relevancia?

8. ¿Se han utilizado citas reales y completas?

9. ¿Se ha introducido literatura externa
   dentro de los resultados del corpus?

10. ¿Otra persona podría reconstruir
    cómo llegamos desde las fuentes hasta cada tema?

Si alguna respuesta es NO:
señalarlo antes de cerrar.

==================================================
34. REGLA FINAL
==================================================

NO quiero únicamente:

“Los principales temas encontrados son A, B y C.”

Quiero poder reconstruir:

QUÉ DIJERON LAS PERSONAS
+
QUÉ SEGMENTOS CONSIDERAMOS RELEVANTES
+
CÓMO LOS CODIFICAMOS
+
CÓMO CAMBIÓ EL CODEBOOK
+
CÓMO AGRUPAMOS LOS CÓDIGOS
+
QUÉ CASOS APOYAN LOS TEMAS
+
QUÉ CASOS LOS CONTRADICEN
+
QUÉ PARTE ES INTERPRETACIÓN
+
QUÉ SIGUE SIENDO INCIERTO.

El objetivo no es producir
la interpretación más convincente.

El objetivo es producir
UN ANÁLISIS CUALITATIVO TRAZABLE,
CRÍTICO Y REVISABLE.
```

## Qué aporta esta versión

### Trazabilidad más allá de la cita

Una cita aporta evidencia y se vincula con el recorrido `cita → segmento → código → categoría → tema`, que también puede recorrerse en sentido contrario para revisar cada conclusión.

### Casos discrepantes

El análisis conserva los casos que contradicen un patrón. Por ejemplo, si varias entrevistas sugieren que la confianza en una IA sanitaria depende de entender cómo funciona, un participante que confía sin entender el sistema también forma parte del resultado y puede ayudar a delimitar la interpretación.

### Historial de decisiones analíticas

Los cambios del codebook quedan registrados. Si los datos llevan a dividir un código inicial en dos significados distintos, se conserva tanto la decisión como su motivo. Ejemplo ilustrativo:

```text
miedo_a_la_tecnología
        ↓ SPLIT
miedo_al_error
+
pérdida_de_control

Motivo:
los casos P03, P07 y P11 muestran
dos significados analíticamente diferentes.
```

## Separación entre corpus y literatura

El contraste bibliográfico no se introduce por defecto durante la codificación inductiva inicial. Primero se analiza el corpus; después puede desarrollarse una fase de discusión que contraste los temas con literatura científica.

El nombre `QUAL.DISCUSSION` representa una posible pieza posterior, no un prompt incluido en este documento:

```text
QUAL.RESEARCH
¿Qué dicen nuestros datos?
        ↓
temas y hallazgos

QUAL.DISCUSSION
¿Cómo dialogan esos hallazgos
con la evidencia publicada?
```

Esta separación permite conservar lo que dicen los datos y distinguirlo de su interpretación a la luz de fuentes externas.
