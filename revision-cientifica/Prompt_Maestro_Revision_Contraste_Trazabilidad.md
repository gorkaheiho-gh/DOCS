# Prompt maestro: revisión, contraste y trazabilidad de estudios científicos

Prompt reutilizable para analizar uno o varios artículos, estudios o informes y organizar sus afirmaciones, evidencias, limitaciones y conclusiones de forma trazable.

El proceso distingue cuatro niveles:

**Lo que dice el estudio → lo que muestran sus datos → lo que encontramos al contrastarlo → lo que finalmente podemos afirmar.**

## Cómo utilizarlo

1. Adjunta el artículo, estudio o conjunto de documentos que quieras analizar.
2. Copia el prompt completo que aparece a continuación.
3. Facilita acceso a las fuentes externas necesarias para el contraste. Si no están disponibles, el análisis debe dejar explícito qué no ha podido verificarse.

## Prompt completo

```text
PROMPT MAESTRO
REVISIÓN, CONTRASTE Y TRAZABILIDAD DE UN ARTÍCULO O ESTUDIO CIENTÍFICO

Quiero que analices el artículo, estudio, informe o conjunto de documentos
que te facilito utilizando un proceso científico trazable.

NO quiero únicamente un resumen.

Quiero transformar el documento en un conjunto de afirmaciones,
evidencias, limitaciones, contrastes y conclusiones que permitan saber:

- qué afirma realmente el estudio;
- qué resultados presenta;
- qué parte es interpretación de los autores;
- qué evidencia respalda cada afirmación;
- qué evidencia externa la apoya, matiza o contradice;
- qué grado de incertidumbre existe;
- qué podemos afirmar razonablemente después del análisis;
- y cómo puede otra persona reconstruir esa conclusión.

==================================================
0. PRINCIPIOS GENERALES
==================================================

Trabaja con estas reglas durante todo el análisis:

1. EL ARTÍCULO ES UNA FUENTE, NO LA VERDAD.

Que algo aparezca publicado no significa automáticamente que sea correcto.

Distingue siempre:

LO QUE DICE EL ESTUDIO

de

LO QUE CONCLUIMOS DESPUÉS DE ANALIZARLO.

2. NO CORRIJAS SILENCIOSAMENTE EL DOCUMENTO.

Si detectas un posible error, simplificación o contradicción:

- conserva primero la afirmación original;
- identifica su procedencia;
- después añade el contraste;
- finalmente emite un veredicto separado.

3. CONSERVA TRAZABILIDAD.

Toda afirmación importante debe poder volver a:

documento
→ página
→ sección
→ párrafo
→ tabla
→ figura
→ resultado concreto.

4. NO INVENTES CERTEZA.

NOT_VERIFIED no significa INCORRECT.

INSUFFICIENT_EVIDENCE no significa CONTRADICTED.

Si la evidencia no permite concluir algo:
declararlo explícitamente.

5. NO CONFUNDAS:

asociación
con causalidad;

significación estadística
con relevancia clínica;

resultado del estudio
con interpretación;

interpretación
con recomendación;

evidencia científica
con permiso para reutilizar contenido.

==================================================
1. IDENTIFICAR EL ESTUDIO
==================================================

Antes de interpretar resultados, extrae:

- título;
- autores;
- año;
- revista/institución;
- DOI o identificador;
- tipo de estudio;
- objetivo principal;
- población;
- ámbito;
- tamaño muestral;
- periodo de estudio;
- intervención o exposición;
- comparador;
- outcomes principales;
- outcomes secundarios;
- financiación;
- conflictos de interés declarados.

Si falta alguno:
indicarlo.

No inferir lo que el documento no indique.

==================================================
2. DESCOMPONER EL DOCUMENTO
==================================================

Separa conceptualmente:

BACKGROUND
→ conocimiento previo utilizado por los autores.

METHODS
→ cómo se realizó el estudio.

RESULTS
→ qué observaron realmente.

INTERPRETATION
→ cómo interpretan los autores los resultados.

LIMITATIONS
→ limitaciones reconocidas.

RECOMMENDATIONS
→ recomendaciones o implicaciones propuestas.

EXTERNAL CLAIMS
→ afirmaciones que dependen de otros estudios o datos externos.

No mezclar estas capas.

==================================================
3. EXTRAER LOS CLAIMS IMPORTANTES
==================================================

No conviertas cada frase en un claim.

Extrae únicamente afirmaciones con valor científico o decisional.

Prioriza:

- resultado principal;
- resultados secundarios relevantes;
- asociaciones;
- efectos;
- cifras;
- prevalencias;
- riesgos;
- odds ratios;
- hazard ratios;
- diferencias entre grupos;
- causalidad;
- afirmaciones de superioridad;
- generalizaciones;
- recomendaciones;
- afirmaciones sobre seguridad;
- afirmaciones sobre eficacia;
- afirmaciones dependientes del tiempo;
- afirmaciones que parezcan especialmente fuertes;
- afirmaciones que contradigan conocimiento previo.

Para cada claim crear una ficha.

==================================================
4. FICHA DE CLAIM
==================================================

Para cada claim registrar:

CLAIM_ID

CLAIM_ORIGINAL
→ texto fiel a lo que sostiene el estudio.

CLAIM_TYPE
por ejemplo:
- resultado;
- asociación;
- causalidad;
- generalización;
- seguridad;
- eficacia;
- prevalencia;
- recomendación;
- background;
- temporal;
- institucional.

SOURCE_LOCATION
→ página;
→ sección;
→ párrafo;
→ tabla/figura cuando corresponda.

POPULATION

INTERVENTION_OR_EXPOSURE

COMPARATOR

OUTCOME

TIMEFRAME

RESULTADO_CUANTITATIVO
cuando exista:
- n;
- efecto;
- diferencia;
- RR;
- OR;
- HR;
- beta;
- media;
- mediana;
- IC95%;
- p;
- NNT/NNH;
- riesgo absoluto;
- riesgo relativo.

No inventar métricas que no estén publicadas.

==================================================
5. RESULTADO VS INTERPRETACIÓN
==================================================

Para cada claim preguntar:

¿Es un dato directamente observado?

¿Es una estimación estadística?

¿Es una interpretación de los autores?

¿Es una recomendación?

¿Es una extrapolación?

Ejemplo:

RESULTADO:
HR 0,72; IC95% 0,61–0,85.

INTERPRETACIÓN:
“La intervención parece tener efecto protector.”

RECOMENDACIÓN:
“La intervención debería incorporarse a práctica clínica.”

No tratar los tres niveles como equivalentes.

==================================================
6. EVALUACIÓN METODOLÓGICA
==================================================

Analiza la metodología sin reducirla a una puntuación única.

Revisar, cuando sea aplicable:

DISEÑO
- RCT;
- cohorte;
- casos-controles;
- transversal;
- diagnóstico;
- predicción;
- revisión sistemática;
- meta-análisis;
- cualitativo;
- otro.

POBLACIÓN
- criterios de inclusión;
- exclusión;
- representatividad;
- contexto asistencial;
- edad;
- sexo;
- comorbilidad;
- tamaño.

EXPOSICIÓN / INTERVENCIÓN
- definición;
- medición;
- consistencia.

COMPARADOR
- adecuado o no;
- comparable.

OUTCOMES
- primarios/secundarios;
- definición;
- medición;
- outcome surrogate vs clínico.

SESGOS
- selección;
- información;
- medición;
- supervivencia;
- publicación;
- confusión.

ESTADÍSTICA
- ajuste;
- confusores;
- tamaño muestral;
- potencia;
- intervalos de confianza;
- multiplicidad;
- análisis post hoc;
- missing data;
- imputación;
- sensibilidad.

PREDICCIÓN, si aplica:
- train/test;
- validación interna;
- externa;
- calibración;
- discriminación;
- overfitting;
- leakage.

REPRODUCIBILIDAD
- datos;
- código;
- protocolo;
- preregistro.

FINANCIACIÓN
- financiación;
- conflictos declarados.

No convertir estas dimensiones automáticamente en:
“estudio bueno/malo”.

Describir fortalezas y limitaciones concretas.

==================================================
7. DETECTAR CLAIMS QUE NECESITAN CONTRASTE EXTERNO
==================================================

No investigar externamente cada frase.

Priorizar para contraste:

- afirmaciones fuertes;
- cifras externas;
- causalidad;
- recomendaciones clínicas;
- seguridad;
- eficacia;
- resultados sorprendentes;
- generalizaciones;
- afirmaciones que los datos internos no justifican por sí solos;
- referencias a “la evidencia existente”;
- claims dependientes del tiempo;
- legislación;
- guías;
- medicamentos;
- vacunas;
- criterios clínicos;
- prevalencias actuales;
- datos institucionales;
- posibles contradicciones.

==================================================
8. CONVERTIR CADA CONTRASTE EN UNA PREGUNTA PRECISA
==================================================

No buscar por tema general.

NO:

“fragilidad mortalidad”.

SÍ:

“¿La fragilidad medida mediante X predice mortalidad a 12 meses
en personas mayores institucionalizadas?”

La búsqueda debe mantener:

CLAIM
→ pregunta
→ búsqueda
→ fuentes encontradas
→ evidencia.

==================================================
9. SOURCE GATE
==================================================

Antes de utilizar una fuente externa registrar:

SOURCE_ID

obra concreta

autores / institución

año

URL / DOI

versión

tipo de publicación

población

licencia o términos de uso cuando importe la reutilización

USAGE_DECISION:

- consultable;
- citable;
- reutilizable;
- restringida;
- no determinada.

No utilizar:

“lo dice PubMed”

“lo dice Google”

“lo dice una web oficial”

como evidencia.

Identificar siempre la obra concreta.

==================================================
10. JERARQUÍA DE FUENTES
==================================================

Seleccionar fuentes según la pregunta.

Cuando sea pertinente valorar:

- revisiones sistemáticas;
- meta-análisis;
- guías clínicas;
- organismos públicos;
- consensos;
- estudios primarios;
- cohortes externas;
- RCT;
- estudios de validación.

Pero no asumir automáticamente que una categoría superior
responde mejor a la pregunta.

Una revisión puede ser excelente
y no incluir la población concreta del claim.

==================================================
11. COMPARABILIDAD
==================================================

Antes de decir que otro estudio “confirma” o “contradice”:

comparar:

- población;
- contexto;
- intervención/exposición;
- comparador;
- outcome;
- definición;
- duración;
- diseño;
- ajuste;
- fecha.

Si no son comparables:
indicarlo.

No usar resultados de otra población
como demostración directa.

==================================================
12. CLASIFICAR LA EVIDENCIA
==================================================

Para cada fuente externa y claim usar:

SUPPORTS
→ apoya directamente la afirmación.

PARTIALLY_SUPPORTS
→ apoya parte del claim o una versión más limitada.

CONTRADICTS
→ aporta evidencia incompatible.

INSUFFICIENT
→ relacionada pero no suficiente para decidir.

NO_EVIDENCE
→ no aporta evidencia útil al claim.

Añadir siempre:

RATIONALE
→ explicación breve de por qué recibe ese estado.

==================================================
13. VEREDICTO DEL CLAIM
==================================================

Después de reunir la evidencia,
emitir un veredicto SEPARADO:

VERIFIED

CORRECT_BUT_SIMPLIFIED

AMBIGUOUS

INCORRECT

NOT_VERIFIED

Definiciones:

VERIFIED
→ evidencia suficiente y compatible con el claim.

CORRECT_BUT_SIMPLIFIED
→ el núcleo es correcto, pero omite matices razonables.

AMBIGUOUS
→ existen interpretaciones, poblaciones o evidencias incompatibles
que impiden una conclusión fuerte.

INCORRECT
→ evidencia suficiente contradice el claim.

NOT_VERIFIED
→ no hemos conseguido evidencia suficiente para decidir.

No usar NOT_VERIFIED como sinónimo de falso.

==================================================
14. EXPLICAR EL VEREDICTO
==================================================

Para cada claim devolver:

VERDICT_REASON

Ejemplo:

“Dos cohortes apoyan la asociación, pero utilizan poblaciones
y definiciones de outcome diferentes. No es posible sostener
el porcentaje exacto del claim original.”

No devolver únicamente una etiqueta.

==================================================
15. CAUSALIDAD
==================================================

Marcar específicamente cualquier salto:

asociación
→ causalidad.

Preguntar:

¿el diseño permite inferencia causal?

¿hay confusión residual?

¿hay temporalidad?

¿existe intervención o sólo observación?

Si el artículo dice:

“X causa Y”

pero sólo presenta asociación observacional:

señalarlo.

==================================================
16. SIGNIFICACIÓN VS RELEVANCIA
==================================================

No interpretar automáticamente:

p < 0,05
→ importante.

Extraer y discutir cuando sea posible:

- tamaño del efecto;
- IC;
- riesgo absoluto;
- riesgo relativo;
- NNT/NNH;
- relevancia clínica;
- incertidumbre.

Separar:

STATISTICAL_SIGNIFICANCE

de

CLINICAL_RELEVANCE.

==================================================
17. GENERALIZACIÓN
==================================================

Registrar:

STUDIED_POPULATION

TARGET_POPULATION
cuando exista una extrapolación.

Evaluar:

¿la conclusión se refiere sólo a la muestra?

¿los autores la extienden a otros grupos?

¿la evidencia externa permite esa extensión?

No asumir que un resultado de hospital
representa residencias,
atención primaria
o población general.

==================================================
18. TEMPORALIDAD
==================================================

Para claims que puedan cambiar con el tiempo registrar:

VALID_AT

CURRENTNESS

Especialmente:

- legislación;
- vacunas;
- guías;
- medicamentos;
- prevalencias;
- estructuras sanitarias;
- protocolos;
- recomendaciones.

No utilizar evidencia actual para demostrar
una afirmación histórica,
ni evidencia histórica como si fuera actual.

==================================================
19. DESACUERDOS
==================================================

Si estudios razonables discrepan:

NO elegir automáticamente uno.

Representar:

CLAIM
├─ SOURCE A → SUPPORTS
├─ SOURCE B → SUPPORTS
├─ SOURCE C → CONTRADICTS
└─ SOURCE D → PARTIALLY_SUPPORTS

Buscar posibles causas:

- población;
- tamaño;
- outcome;
- intervención;
- diseño;
- duración;
- definición;
- sesgo;
- fecha.

El desacuerdo puede ser el resultado.

==================================================
20. EVITAR JUEZ Y PARTE
==================================================

Separar conceptualmente:

EXTRACTOR
→ identifica claims.

RETRIEVER
→ busca evidencia.

VERIFIER
→ clasifica evidencia.

REVIEWER
→ emite veredicto.

Cuando sea posible:

el verificador no debe recibir
una conclusión predeterminada que deba confirmar.

No buscar sólo evidencia confirmatoria.

Buscar también:

“evidence against”
“contradictory findings”
“failed replication”
“no association”
según corresponda.

==================================================
21. LÍMITE DE BÚSQUEDA
==================================================

No convertir cada claim en una investigación infinita.

Para cada claim:

- buscar suficientes fuentes para valorar el estado;
- priorizar calidad y comparabilidad;
- detenerse cuando nuevas búsquedas no cambien razonablemente
  la conclusión.

Si no se puede resolver:

NOT_VERIFIED
o
AMBIGUOUS.

Registrar:

SEARCH_EXHAUSTED = true

cuando corresponda.

==================================================
22. PUBLICATION READINESS
==================================================

Separar la conclusión científica de la capacidad de reutilizarla.

Para cada claim revisado:

SCIENTIFIC_STATUS

y

PUBLICATION_STATUS:

READY

HOLD

RESTRICTED

UNKNOWN

Un claim puede estar:

VERIFIED
+
HOLD

si científicamente está suficientemente apoyado
pero no tenemos condiciones claras para reutilizar
determinada fuente o corrección.

==================================================
23. PUBLICATION HOLD
==================================================

Cuando algo no esté listo para publicación:

NO inventar una fuente.

NO volver silenciosamente a una versión anterior.

NO esconder la incertidumbre.

Marcar:

PUBLICATION_HOLD

con:

- motivo;
- fuente problemática;
- qué falta para resolverlo.

==================================================
24. RASTRO AUDITABLE
==================================================

Para cada claim conservar:

CLAIM
↓
SOURCE LOCATION
↓
SEARCH QUERY
↓
EXTERNAL SOURCES
↓
EVIDENCE CLASSIFICATION
↓
VERDICT
↓
RATIONALE
↓
PUBLICATION STATUS
↓
DATE
↓
VERSION.

Otra persona debe poder reconstruir
por qué se llegó a la conclusión.

==================================================
25. NO USAR UN SCORE ÚNICO
==================================================

NO crear por defecto:

“calidad científica: 8/10”

“fiabilidad: 82%”

“evidencia: 4 estrellas”.

Mantener separadas dimensiones como:

- diseño;
- sesgo;
- precisión;
- comparabilidad;
- consistencia;
- actualidad;
- aplicabilidad;
- reproducibilidad.

Un único score puede ocultar compensaciones importantes.

==================================================
26. SALIDA FINAL
==================================================

Quiero el resultado en seis bloques.

=====================
A. RESUMEN DEL ESTUDIO
=====================

Máximo 10-15 líneas.

Explica:

- qué pregunta intenta responder;
- cómo lo hace;
- qué encontró;
- cuál es su conclusión principal.

Sin añadir todavía el contraste externo.

=====================
B. MAPA DE CLAIMS
=====================

Tabla con:

CLAIM_ID

CLAIM

TIPO

PROCEDENCIA

RESULTADO DEL ESTUDIO

NECESITA CONTRASTE:
sí/no

=====================
C. REVISIÓN METODOLÓGICA
=====================

Describir por dimensiones:

- diseño;
- población;
- medición;
- comparador;
- outcomes;
- análisis;
- sesgos;
- incertidumbre;
- generalización;
- reproducibilidad;
- financiación/conflictos.

Separar:

FORTALEZAS

LIMITACIONES

No puntuación agregada.

=====================
D. CONTRASTE CLAIM POR CLAIM
=====================

Para cada claim relevante:

CLAIM_ID

CLAIM ORIGINAL

PREGUNTA DE VERIFICACIÓN

FUENTES EXTERNAS

Para cada fuente:
- referencia;
- población;
- resultado;
- SUPPORTS / PARTIALLY_SUPPORTS /
  CONTRADICTS / INSUFFICIENT / NO_EVIDENCE;
- razón.

Después:

VERDICT:
VERIFIED /
CORRECT_BUT_SIMPLIFIED /
AMBIGUOUS /
INCORRECT /
NOT_VERIFIED.

VERDICT_REASON.

=====================
E. QUÉ PODEMOS AFIRMAR
=====================

Transforma los resultados anteriores en una síntesis prudente:

PODEMOS AFIRMAR

PODEMOS AFIRMAR CON MATICES

NO PODEMOS AFIRMAR TODAVÍA

EVIDENCIA CONTRADICTORIA

No introducir nuevos claims.

=====================
F. AUDIT TRAIL
=====================

Para cada claim:

claim
→ procedencia original
→ fuentes externas
→ evidencia
→ veredicto
→ publication status
→ fecha de revisión.

==================================================
27. CONCLUSIÓN GENERAL
==================================================

Finaliza respondiendo:

1. ¿Qué aporta realmente este estudio?

2. ¿Qué resultados parecen suficientemente sólidos?

3. ¿Qué afirmaciones deberían formularse con mayor prudencia?

4. ¿Qué resultados no se han podido verificar?

5. ¿Dónde existe evidencia contradictoria?

6. ¿Qué limitaciones condicionan la aplicabilidad?

7. ¿Qué cuestiones merecerían nuevos estudios?

8. ¿Qué claims están listos para reutilizarse
   y cuáles deberían quedar en HOLD?

==================================================
28. REGLA FINAL
==================================================

NO quiero que me digas simplemente:

“el estudio es fiable”

o

“el estudio no es fiable”.

Quiero poder reconstruir:

QUÉ AFIRMA
+
DE DÓNDE SALE
+
QUÉ EVIDENCIA LO APOYA
+
QUÉ EVIDENCIA LO MATIZA
+
QUÉ INCERTIDUMBRE EXISTE
+
QUÉ PODEMOS CONCLUIR.

Si alguna información no está en el documento:
indicarlo.

Si alguna afirmación no puede verificarse:
indicarlo.

Si las fuentes discrepan:
conservar el desacuerdo.

Si no hay evidencia suficiente:
no rellenar el hueco con conocimiento general.

El objetivo no es producir una respuesta contundente.

El objetivo es producir
CONOCIMIENTO CIENTÍFICO TRAZABLE Y AUDITABLE.
```

## Qué aporta este enfoque

Este prompt no pide a la IA que decida si un estudio es bueno o malo. Le obliga a descomponer lo que afirma, localizar de dónde sale, separar resultados de interpretación, buscar evidencia comparable, conservar las contradicciones y dejar visible aquello que no ha podido demostrar.

## Uso con varios estudios

Cada estudio aporta sus afirmaciones (claims), que pueden integrarse en un mapa común de evidencias, conclusiones, contradicciones e incertidumbre:

```text
ESTUDIO A ─→ claims ─┐
ESTUDIO B ─→ claims ─┤
ESTUDIO C ─→ claims ─┼→ EVIDENCE GRAPH
ESTUDIO D ─→ claims ─┤         ↓
ESTUDIO E ─→ claims ─┘    conclusiones
                              +
                         contradicciones
                              +
                          incertidumbre
```

El objetivo es compartir tanto las conclusiones como el procedimiento que permite reconstruir el camino hasta ellas.
