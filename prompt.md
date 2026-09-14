# Tariff News Prompt

Search for all factual news published between September 8 and September 14,
2026, regarding tariff-related actions taken by the United States government.
Include all industries and all types of actions: new tariffs, increases,
suspensions, official threats, or proposals.  Also include any retaliatory
measures announced or implemented by other countries in response to U.S.
tariffs.  Focus strictly on factual information — exclude any editorial
commentary or opinion.  Provide a structured summary in English, preferably with
tables listing the country, type of action, affected goods, and date of the
announcement.  Include official actions and news form reputable sources.  Cover
official government announcements and actions, and reports from reputable news
outlets about potential or unofficial tariff developments.  I want the search to
include both U.S.  government actions and responses by foreign governments
(retaliatory tariffs, etc.).  Include actions or proposals even if they are not
yet finalized (e.g., draft proposals or threats).  I like the sources linked in
the summary.  Focus only on tariffs directly involving the United States.
Include links to official government sites and top-tier news outlets.

# General News Prompt

Busca en la web noticias publicadas entre el 8 de septiembre y el 14 de
septiembre de 2026, inclusive, para elaborar un resumen semanal dirigido a
economistas y responsables de política económica de un banco central.

Criterio central de selección

Prioriza noticias que aporten información capaz de modificar el diagnóstico
macroeconómico, las perspectivas de inflación y crecimiento, el balance de
riesgos, la orientación de política económica o las condiciones financieras
internacionales.

Selecciona por la importancia del mecanismo económico y sus consecuencias.  Una
noticia debe ayudar a entender qué cambió y por qué ese cambio importa para las
decisiones de política.

Temas prioritarios

Inflación y expectativas: persistencia, difusión entre sectores, inflación
subyacente, salarios, fijación de precios, anclaje de expectativas y efectos de
segunda ronda.  Política monetaria: decisiones, comunicación y cambios en la
posición de los bancos centrales.  Prioriza noticias que expliquen sus dilemas,
los datos que podrían modificar una decisión y la trayectoria esperada de tasas.
Condiciones financieras internacionales: movimientos significativos en
rendimientos, primas de riesgo, crédito, liquidez, tipos de cambio y flujos de
capital.  Transmisión monetaria, fiscal y comercial: noticias que identifiquen
mecanismos concretos mediante los cuales las políticas afectan la inflación, la
actividad, la inversión, el consumo o el comercio.  Choques de oferta: cambios
relevantes en alimentos, energía, transporte, materias primas y cadenas de
suministro, especialmente cuando puedan generar efectos persistentes.  Actividad
económica y empleo: indicadores o acontecimientos que cambien de forma material
la evaluación del ciclo económico.  No selecciones variaciones ordinarias sin
consecuencias claras.  Deuda y sostenibilidad fiscal: cambios que alteren el
riesgo soberano, las condiciones de financiamiento o el margen de acción de la
política económica.  Riesgos geopolíticos e institucionales: inclúyelos cuando
tengan un canal económico identificable y consecuencias para precios, comercio,
mercados o decisiones de política.

Cobertura geográfica

Prioriza Estados Unidos, la eurozona y los mercados globales.  Incluye otras
economías cuando sus acontecimientos tengan implicaciones internacionales o sean
relevantes para Guatemala mediante el comercio, los precios de materias primas,
las remesas, los flujos financieros o las expectativas.

Criterios de exclusión

Excluye:

Noticias que solo informen una variación ordinaria de un indicador.  Revisiones
rutinarias de previsiones sin un cambio relevante en el diagnóstico.
Acontecimientos estrictamente locales sin mecanismos de transmisión
internacional.  Anuncios administrativos o financieros sin efectos
macroeconómicos claros.  Colocaciones de deuda rutinarias.  Noticias repetitivas
o que no añadan información frente a acontecimientos ya seleccionados.

Fuentes admitidas y verificación

Utiliza exclusivamente noticias y análisis informativos de medios con reputación
internacional reconocida, como Reuters, Associated Press, Bloomberg, Financial
Times, The Wall Street Journal, The New York Times, CNN y BBC; o publicaciones
oficiales de bancos centrales, organismos internacionales y autoridades
estadísticas, como el BCE, la Reserva Federal, el FMI, el Banco Mundial, el BPI
y Eurostat.

Enlaza directamente al artículo o documento en el sitio de la entidad que lo
publicó.  Excluye agregadores, blogs personales, portales de inversión sin
responsabilidad editorial reconocida y publicaciones sin autoría o procedencia
verificable.

Verifica la fecha de publicación y la fecha del acontecimiento.  Para
indicadores, identifica el período de referencia.  Distingue entre hechos
observados, anuncios, previsiones, opiniones y expectativas de mercado.  No
presentes expectativas de tasas como decisiones adoptadas ni amenazas
comerciales como medidas implementadas.

Redacta titulares fieles al contenido comprobado.  Si una noticia proporcionada
como referencia no puede verificarse, indícalo y no le atribuyas una fuente por
semejanza temática.  Separa las conclusiones de la fuente de tu interpretación
sobre su relevancia económica

Formato de entrega

Presenta los resultados en español en una tabla con las siguientes columnas:

Fecha País o ámbito Noticia y hechos principales Relevancia para la política
económica Fuente y enlace

Ordena las noticias cronológicamente.  Explica de forma concreta el mecanismo
económico y evita descripciones genéricas.  No fijes previamente un número de
noticias: incluye únicamente las que satisfagan los criterios.

## Summary Prompt

Realiza un resumen de la información contenida en la siguiente noticia o
conjunto de noticias:

[ENLACE O ENLACES]

Si se proporcionan varias fuentes, utiliza la publicación más reciente como
fuente principal.  Emplea las anteriores para aportar contexto, verificar
antecedentes y precisar la interpretación, sin permitir que desplacen la idea
central de la noticia más reciente.

Formato de salida:

1. Escribe un título informativo que exprese con precisión la idea central.
2. Redacta exactamente tres bullets.  Cada bullet, incluida la fecha cuando
   corresponda, debe tener un máximo de 300 caracteres.
3. Coloca al final todos los enlaces como texto visible, uno por línea y sin
   hipervínculos embebidos.
4. Presenta todo el resultado dentro de un bloque de texto para facilitar su
   copia.

Contenido de los bullets:

• Bullet 1: Comienza con la fecha de publicación de la noticia más reciente,
seguida de un punto.  Resume el hecho o expectativa principal e identifica al
agente involucrado.

• Bullet 2: Incluye los detalles más relevantes: cifras, fechas, tasas,
variaciones, lugares, disposiciones legales, indicadores o condiciones
económicas.

• Bullet 3: Expone únicamente el análisis, las previsiones, los riesgos o las
consecuencias señalados por los agentes o por las noticias consultadas.  No
agregues interpretaciones propias.

Reglas de redacción:

- Utiliza un lenguaje formal, conciso y apropiado para economistas y
  responsables de política económica.
- Los tres bullets deben desarrollar una misma idea central y guardar coherencia
  entre sí.
- Distingue claramente entre hechos confirmados, decisiones anunciadas,
  propuestas, expectativas y pronósticos.
- Conserva el carácter de expectativa cuando un acontecimiento todavía no ha
  ocurrido.  No redactes una medida esperada como un hecho consumado.
- Indica quién sostiene una expectativa o previsión.  Utiliza formulaciones como
  "los mercados financieros anticipan", "los operadores descuentan" o "los
  responsables del banco central prevén", según lo indicado en la noticia.
- Cuando la fuente específica sea anónima o no esté identificada, evita
  expresiones como "fuentes conocedoras" o "personas informadas".  Formula la
  idea como una expectativa del mercado o del agente colectivo pertinente,
  únicamente cuando la noticia permita esa atribución.
- No menciones en los bullets al medio que publica la noticia, como Reuters, The
  Wall Street Journal o Bloomberg.  El interés debe centrarse en los agentes y
  hechos involucrados.
- Evita referencias vagas como "los economistas", "los expertos" o "la deuda
  mejoró".  Precisa el grupo, la variable, el ámbito geográfico y el sentido del
  cambio.
- Evita nombres de analistas individuales y de instituciones privadas, salvo que
  sean indispensables para respaldar una previsión o cifra relevante.  En ese
  caso, identifica brevemente qué tipo de entidad es, por ejemplo: "la
  consultora energética Energy Aspects".
- Puedes mencionar autoridades, funcionarios o instituciones públicas cuando
  sean protagonistas esenciales, como gobernadores de bancos centrales, la
  Reserva Federal, el BCE, el BIS o el FMI.
- Mantén en presente los efectos que continúan vigentes: "endurecen", "añaden",
  "elevan" o "restringen".  Utiliza el pasado solo para hechos ya concluidos.
- Evita afirmaciones imprecisas, contradicciones, repeticiones, explicaciones
  innecesarias y conclusiones que no estén contenidas en las fuentes.
- No incluyas comentarios, aclaraciones ni texto fuera del bloque solicitado.