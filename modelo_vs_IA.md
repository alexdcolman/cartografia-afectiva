# Tecnologías del afecto: interpretabilidad, conflicto y crítica en la era de los modelos generativos

En los últimos años, los grandes modelos de lenguaje (LLMs) han alcanzado una notable capacidad para generar texto coherente, identificar patrones afectivos básicos y participar en tareas complejas de procesamiento del lenguaje natural. Estos desarrollos consolidaron su integración en múltiples áreas, desde la asistencia conversacional hasta el análisis automatizado de sentimientos.

No obstante, su aplicación al estudio discursivo de las emociones plantea desafíos significativos. Entre ellos, destacan las dificultades para captar estructuras de sentido más allá de correlaciones estadísticas, la opacidad de sus mecanismos inferenciales y la posibilidad de replicar sesgos presentes en los datos de entrenamiento. Estos problemas no son meramente técnicos: ponen en juego modos específicos de construir conocimiento, definir categorías y organizar la interpretación.

Este documento argumenta una estrategia complementaria, basada en la construcción de modelos de codificación emocional informados por tradiciones críticas del análisis del discurso, la semiótica, la retórica y la teoría de la argumentación. Lejos de oponer saber experto y capacidad computacional, se explora una articulación posible entre ambos, con el objetivo de guiar los procedimientos automáticos sin renunciar a la complejidad del sentido.

En esta óptica, el análisis se orienta a problematizar los supuestos que subyacen a los modelos estadísticos aplicados al lenguaje –en especial los basados en arquitecturas de LLMs– y a contrastarlos con enfoques que priorizan la interpretación situada y la historicidad de los afectos. Más que una denuncia o un rechazo, se busca habilitar un espacio crítico donde las herramientas algorítmicas puedan ser repensadas desde sus condiciones culturales, epistemológicas y políticas de producción.

## I. Entre eficiencia y sentido: tensiones en el paradigma computacional

**1. La "lección amarga" y sus implicancias**

En [“The Bitter Lesson”](http://www.incompleteideas.net/IncIdeas/BitterLesson.html), Rich Sutton (2019) –referente del aprendizaje por refuerzo– resume lo que considera la enseñanza central de más de siete décadas de investigación en inteligencia artificial: los métodos generales que aprovechan la capacidad creciente del cómputo y el aprendizaje automático tienden a superar, a largo plazo, aquellos basados en conocimiento experto o estructuras humanas.

Su argumento parte de una constatación empírica: si bien los enfoques que incorporan intuiciones humanas o teorías cognitivas pueden ofrecer ventajas iniciales, su escalabilidad y capacidad de mejora suelen estar acotadas. En cambio, los métodos estadísticos generalistas, por más “opacos” o técnicamente rudimentarios que parezcan, logran avances sostenidos al apoyarse en el crecimiento exponencial del procesamiento de datos. Sutton ilustra esta dinámica con casos como el ajedrez computacional, el reconocimiento del habla o el procesamiento del lenguaje natural, donde sistemas inicialmente guiados por reglas humanas fueron progresivamente desplazados por modelos de búsqueda masiva o aprendizaje automático.

Este diagnóstico se inscribe en una concepción pragmática y operativa del conocimiento, fuertemente orientada por la eficiencia algorítmica. En este marco, lo relevante no es tanto si un sistema imita la cognición humana, sino si resuelve con eficacia una tarea a partir de correlaciones y patrones estadísticos. El conocimiento, así entendido, se valida por su capacidad performativa más que por su anclaje en marcos teóricos.

En el fondo, esta concepción presupone una cierta forma de universalismo computacional: una confianza en que los patrones que emergen del aprendizaje automático pueden producir formas válidas de saber, incluso cuando escapan a las categorías conceptuales o a las mediaciones interpretativas tradicionales. La “lección amarga” consistiría, entonces, en aceptar que nuestras estructuras de sentido no siempre optimizan el rendimiento, y que, en ciertos contextos, pueden incluso interferir en él.

**2. La mutación del lugar del saber**

Aceptar esta perspectiva no implica simplemente un giro metodológico: supone repensar el estatuto del saber y el lugar de la interpretación en los procesos de modelización. La cuestión no es solo técnica, sino epistémica.

En efecto, los modelos estadísticos de aprendizaje profundo producen decisiones a partir de múltiples capas de correlaciones cuya trazabilidad es limitada. Esto conlleva riesgos evidentes: desde la pérdida de inteligibilidad en los procesos de decisión, hasta la naturalización de categorías o sesgos que permanecen ocultos en las capas internas del modelo. A nivel social, puede favorecer formas de automatización normativa difíciles de cuestionar; a nivel epistémico, puede contribuir a desplazar o deslegitimar saberes situados, interpretativos o críticos.

No se trata aquí de oponer lo “humano” a lo “artificial” como términos esencializados, sino de señalar que ciertos modos de producción de conocimiento –reflexivos, históricos, contextualizados– pueden verse marginados en contextos donde prima una lógica de rendimiento estadístico. Esta transformación afecta particularmente aquellos campos donde la interpretación es una dimensión constitutiva, como ocurre en el análisis emocional y discursivo.

Desde esta perspectiva, el desafío no es rechazar la computación estadística, sino pensar cómo reintroducir en ella formas de inteligibilidad que no se reduzcan a la correlación. Modelar lo emocional exige reconocer su inscripción simbólica, su dependencia de contextos enunciativos y su carga axiológica. Esas dimensiones no desaparecen en el dato: pero sí pueden quedar silenciadas si el dato se absolutiza como fuente autosuficiente de conocimiento.

## II. Codificar la emoción desde la interpretación: un enfoque alternativo

**1. Modelización interpretativa y conocimiento experto**

El modelo desarrollado en este repositorio se sitúa en diálogo crítico con los enfoques de clasificación afectiva basados exclusivamente en aprendizaje automático. En lugar de delegar íntegramente la detección de lo emocional a correlaciones estadísticas, propone una estrategia combinada: construir una gramática computable de la emocionalidad discursiva, informada por marcos teóricos y conocimiento experto.

Este enfoque retoma tradiciones semióticas y pragmáticas que entienden la emoción como una forma históricamente situada de significación. A partir de teorías como la semiótica de las pasiones (Greimas, Fabbri), la tópica emocional (Plantin) o las retóricas del *páthos*, se diseñó un sistema de codificación de más de noventa variables. Estas buscan capturar modos de presencia, modulaciones, mediaciones y configuraciones afectivas en los textos.

Lejos de ser simples etiquetas, estas variables son operadores que permiten representar fenómenos complejos –como el conflicto afectivo, la legitimación valorativa o la oscilación modal– de manera computacionalmente procesable, sin perder por ello su espesor hermenéutico.

En ese sentido, el modelo no se plantea como alternativa excluyente a los enfoques basados en LLM o aprendizaje profundo, sino como un dispositivo complementario, orientado a reinscribir preguntas interpretativas en el análisis computacional del lenguaje. Su objetivo no es competir en escala, sino explorar otro tipo de inteligibilidad: una que integre la semántica con la estadística y la técnica con la reflexión crítica.

**2. Cartografiar la emoción como forma de saber**

La emoción no es un residuo subjetivo ni un ruido frente a la objetividad del dato. Tiene espesor cognitivo, valor epistémico y fuerza organizadora. Configura jerarquías valorativas, orienta la interpretación y contribuye a la inteligibilidad social de los conflictos.

Desde esta perspectiva, las pasiones en el discurso no son meros añadidos expresivos. Son estructuras significantes, formas codificadas de intervenir en el mundo, con efectos pragmáticos, ideológicos y políticos.

El modelo propuesto parte de esta premisa. La emocionalidad no se reduce a sentimientos discretos, listas de palabras o coordenadas binarias de polaridad. Es una dimensión relacional, modulada por marcos de sentido, estrategias retóricas y posiciones enunciativas. Por eso, las 92 variables construidas no buscan simplemente detectar afectos, sino cartografiar su inscripción discursiva. Permiten identificar, por ejemplo:

-	*Mapas emocionales*, que visualizan la distribución de categorías afectivas según criterios modales, experienciales o evaluativos.

-	*Perfiles emocionales*, que vinculan tipos de experienciadores con dominios afectivos específicos.

-	*Series temporales*, que trazan la evolución de la afectividad a lo largo de textos o corpus, identificando momentos de ruptura o reconfiguración.

-	*Campos de emoción*, que reconstruyen el espacio relacional en el que distintos experienciadores se posicionan frente a determinadas fuentes de emoción, o en torno a los tipos de emoción que una misma fuente activa en diferentes sujetos.

-	*Simulacros emocionales*, cuyo análisis computacional permite detectar estructuras semánticas que organizan la escenificación de la emoción.

Este tipo de formalización permite articular lo cualitativo y lo computacional sin disolver la densidad interpretativa del análisis. Lejos de proponer una alternativa tecnofóbica, el enfoque plantea una posibilidad metodológica distinta: aquella que inscribe la computación en un horizonte de sentido.

## III. Condiciones epocales: saber, experiencia y producción de sentido

**1. Las condiciones de posibilidad del pensamiento**

En su análisis sobre la historicidad del pensamiento político moderno, Elías Palti (2003, 2007) sostiene que los conceptos fundamentales que organizan dicho pensamiento –como “sujeto”, “Estado” o “historia”– no deben entenderse como nociones universales o doctrinarias, sino como formas históricamente situadas de organizar la experiencia política. En diálogo con tradiciones como la historia conceptual y la genealogía foucaultiana, Palti propone estudiar las condiciones de posibilidad que permiten que ciertas categorías emerjan, circulen y adquieran sentido en contextos específicos. Estas condiciones no se limitan a lo explícitamente ideológico, sino que configuran regímenes de visibilidad y formas de inteligibilidad que determinan qué puede pensarse y decirse políticamente en un momento dado.

Desde esta perspectiva, la expansión contemporánea de la inteligencia artificial no puede pensarse únicamente como un avance técnico. Su despliegue también señala una transformación más amplia en el régimen de saber: un corrimiento hacia dispositivos que privilegian la correlación, la previsión y la eficiencia algorítmica como criterios de validación epistémica. Lo que está en juego no es sólo qué tecnologías utilizamos, sino qué entendemos por conocimiento, por evidencia y por objetividad en este nuevo paisaje epistémico.

Por ello, los debates actuales en torno a la IA –incluidos los análisis afectivos computacionales– exceden las decisiones metodológicas o las opciones de modelado. En el fondo, remiten a disputas más amplias sobre las formas contemporáneas de producción de verdad: sobre qué saberes se legitiman, qué procedimientos se consideran válidos y qué actores están autorizados a producir conocimiento en la esfera pública.

**2. Tensiones persistentes: estructura, experiencia y la cuestión del afecto**

Este escenario reactualiza una tensión presente desde hace tiempo en las ciencias humanas: la que contrapone formas estructurales de explicación y comprensiones centradas en la experiencia.

En la actualidad, esa tensión asume nuevas formas:

-	La lógica algorítmica, orientada a detectar patrones en grandes volúmenes de datos, frente a la experiencia situada, encarnada en prácticas y trayectorias singulares.

-	El hallazgo estadístico como correlación frente a la interpretación contextualizada como reconstrucción de sentidos.

-	La emoción concebida como ruido que contamina el dato frente a su consideración como estructura significativa que orienta valores, evaluaciones y posiciones.

Estas tensiones no son nuevas, pero cobran actualidad frente a la masificación de modelos automáticos y la creciente automatización de procesos analíticos. En este contexto, toda propuesta de modelización afectiva –sea técnica o interpretativa– implica un posicionamiento sobre cómo se articula el conocimiento con la vivencia y el dato con el sentido. No hay neutralidad en las formas en que codificamos el afecto.

**3. Más allá de las oposiciones: modelos operativos y sensibilidad al contexto**

Buena parte del pensamiento crítico contemporáneo ha problematizado la dicotomía entre estructura y experiencia, cuestionando sus presupuestos dualistas. Sin embargo, esa operación, aunque productiva intelectual y (quizás) políticamente, ha dejado abiertas ciertas preguntas operativas: ¿cómo construir modelos analíticos que no sólo sean técnicamente eficaces, sino también sensibles a la complejidad de lo vivencial? ¿Cómo generar herramientas capaces de formalizar sin empobrecer?

Este trabajo busca retomar esas preguntas sin resolverlas de forma definitiva. No se trata de proponer una síntesis superadora ni de postular una tecnología “del sentido” como solución acabada. Más modestamente, se propone explorar formas de articulación entre distintas lógicas de análisis –computacional e interpretativa– que permitan abordar el fenómeno afectivo en su doble dimensión: como patrón estructurable y como experiencia situada.

## IV. Hacia una inteligencia hermenéutica: explorar lo híbrido

En lugar de plantear una oposición entre enfoques técnicos e interpretativos, esta propuesta se inscribe en una lógica de complementariedad crítica. Su hipótesis de trabajo parte de la idea de que la combinación de modelos estadísticos y categorías teóricas puede enriquecer tanto la exploración de los datos como la construcción de sentido.

Los marcos expertos –derivados de la semiótica, la teoría del discurso o la pragmática– ofrecen herramientas para introducir criterios conceptuales, explicitar decisiones analíticas y mantener una trazabilidad teórica clara. Por su parte, las técnicas computacionales –desde LLMs hasta análisis multivariado– permiten trabajar con grandes volúmenes de información, detectar regularidades no evidentes y poner en tensión hipótesis previas.

La articulación entre ambos registros se organiza aquí en torno a tres principios:

-	*Situación del conocimiento:* toda operación analítica está situada, históricamente mediada y teóricamente condicionada.

-	*Reflexividad epistémica:* los modelos –tanto computacionales como teóricos– contienen opacidades que deben ser reconocidas y puestas en discusión.

-	*Hibridación estratégica:* no como conciliación armónica, sino como modo de activar tensiones productivas entre modos de saber distintos.

Desde este enfoque, el modelo desarrollado no busca sustituir ni replicar las capacidades de los LLMs. Su objetivo es otro: intervenir críticamente en sus resultados, enriquecer sus producciones con interpretaciones conceptuales y abrir espacio para formas de lectura donde lo afectivo no sea sólo una etiqueta, sino una clave estructurante de la significación.

Esta integración habilita, por ejemplo:

-	La clasificación supervisada basada en categorías semánticas densas, construidas teóricamente.

-	El uso de técnicas no supervisadas guiadas por variables conceptuales, evitando agrupamientos vacíos de sentido.

-	Visualizaciones que muestren el afecto no sólo como intensidad o frecuencia, sino como forma de orientación ética y política.

Antes que una solución final, esta inteligencia hermenéutica se plantea como una estrategia de lectura crítica: una forma de pensar y modelar el sentido que reconozca la heterogeneidad del dato, la historicidad de las emociones y la dimensión conflictiva del lenguaje.

## V. Cuestiones epistemológicas y políticas

El análisis computacional de las emociones no puede abordarse únicamente como un problema técnico. Involucra una serie de decisiones epistemológicas y políticas que inciden en los modos en que se producen, circulan e interpretan los afectos en las sociedades contemporáneas.

Una primera cuestión remite a la definición misma de “emoción”: ¿se la concibe como una respuesta fisiológica, una experiencia subjetiva, una forma de conocimiento, un acto semiótico? Cada respuesta conlleva un recorte: define qué se observa, qué dimensiones se consideran relevantes y qué aspectos del lenguaje se tornan legibles para el análisis automatizado. No se trata, por tanto, de una cuestión neutral ni secundaria, sino de una operación que condiciona los resultados desde el inicio.

Una segunda cuestión se vincula con la construcción de las categorías analíticas. Los repertorios emocionales que nutren los modelos no son transparentes ni universales: responden a matrices culturales, históricamente situadas, que definen qué emociones son reconocidas, cómo se las nombra y qué valor se les asigna. Todo modelo –sea construido a partir de corpus etiquetados, expertos o estadísticas– inscribe, de forma más o menos explícita, una determinada concepción del sujeto, del conflicto y del valor.

Finalmente, debe considerarse el uso de estas tecnologías en espacios sensibles como la comunicación política, la cultura o los medios. Automatizar la lectura emocional en estos ámbitos no es un procedimiento inocuo: puede implicar la cristalización de ciertos esquemas interpretativos, la normalización de jerarquías valorativas y la reproducción (o disputa) de clivajes simbólicos. La apariencia de objetividad matemática no elimina el carácter situado de toda interpretación.

Frente a estos desafíos, el enfoque adoptado en este proyecto no plantea una oposición entre modelos “sesgados” y “neutrales”, sino que apunta a *visibilizar las condiciones de producción de los modelos*, los supuestos que los sustentan y las formas en que habilitan o restringen determinadas lecturas. Tanto el aprendizaje automático como las estrategias de codificación experta operan con marcos conceptuales, sesgos y límites. Pero difieren en el grado de explicitación, trazabilidad y deliberabilidad que ofrecen.

En ese sentido, la codificación experta permite situar el análisis dentro de un marco teórico definido, explicitar las decisiones metodológicas y someterlas a discusión crítica. No se trata de idealizar este enfoque, sino de reconocer que su apertura a la revisión constituye una condición necesaria para una lectura reflexiva de los afectos en el discurso.

## VI. La dificultad de lo singular

Uno de los desafíos persistentes en el análisis computacional de las emociones radica en su limitada capacidad para dar cuenta de lo singular: aquellas manifestaciones afectivas que no se ajustan fácilmente a patrones recurrentes, que emergen en el espesor del lenguaje como acontecimientos situados y contextualmente modulados.

El tono, la ironía, la performatividad, los silencios, las marcas de interdiscursividad, entre otras formas de modulación, inciden de manera decisiva en la construcción afectiva de un enunciado. Una misma palabra puede adquirir valores emocionales opuestos según el gesto enunciativo que la soporte, el horizonte pragmático en el que se inscriba o la memoria discursiva que convoque.

En este marco, la singularidad es una propiedad constitutiva del lenguaje como práctica social situada. Por eso, la detección de fenómenos como la ironía, la ambivalencia o los desplazamientos de sentido exigen aproximaciones que reconozcan la densidad retórica, semántica y pragmática del discurso.

Desde esta perspectiva, los modelos expertos –anclados en categorías teóricas, decisiones analíticas explícitas y una lectura situada del corpus– ofrecen una ventaja cualitativa frente a aproximaciones puramente correlacionales, al permitir identificar y describir con mayor precisión fenómenos como:

-	La ambigüedad emocional, cuando coexisten registros afectivos contradictorios dentro de un mismo enunciado.

-	La evolución temporal de climas emocionales, que permite rastrear transformaciones en la orientación valorativa a lo largo del discurso.

-	Las tensiones o los desajustes modulativos, donde se superponen o chocan distintos indicadores afectivos en una misma unidad textual.

Los enfoques basados en codificación experta –aunque no exentos de sesgos ni arbitrariedades– permiten explicitar las decisiones analíticas, anclar el análisis en categorías teóricas y atender a la densidad semántica del corpus. En ese sentido, no necesariamente se oponen a las estrategias automatizadas, sino que pueden complementar y tensionar sus resultados, abriendo espacio para la interpretación crítica de aquello que los modelos estadísticos tienden a simplificar.

## VII. Conclusión

El modelo propuesto no busca competir con la inteligencia artificial en términos de eficiencia ni reemplazar la interpretación humana con procedimientos algorítmicos. Más bien, parte de la premisa de que *la colaboración crítica entre enfoques automatizados y lecturas situadas* puede enriquecer la comprensión de los afectos en el discurso.

Frente a una tendencia generalizada a automatizar la interpretación emocional, este enfoque se sitúa en un espacio intermedio: reconoce la potencia de la escala y la velocidad que ofrecen los métodos computacionales, pero también señala sus límites al enfrentar fenómenos semánticamente densos, contextualmente modulados o retóricamente complejos.

Lejos de oponer taxativamente modelos expertos y modelos estadísticos, se propone una articulación cuidadosa: una estrategia que combine la capacidad de detección masiva con la lectura analítica situada. Esta articulación no borra las tensiones entre ambas lógicas –la del patrón y la de la excepción, la estadística y la hermenéutica–, pero las vuelve productivas como campo de experimentación y crítica.

En última instancia, el objetivo no es “humanizar” la IA en un sentido superficial, ni atribuirle capacidades interpretativas plenas, sino explorar cómo puede integrarse en procesos de análisis que no renuncien al juicio, a la reflexividad o al conflicto de interpretaciones. Si algo puede aportar este modelo, es precisamente eso: un modo de habitar críticamente la interfaz entre cálculo y sentido, entre lo que se repite y lo que, por definición, resiste toda repetición.

## Referencias

Palti, E. (2003). El “retorno del sujeto”: subjetividad, historia y contingencia en el pensamiento moderno. *Prismas. Revista de historia intelectual*, (7), 27-50.

Palti, E. (2007). *El tiempo de la política: El siglo XIX reconsiderado*. Buenos Aires: Siglo XXI Editores.

Sutton, R. (2019). The bitter lesson. *Incomplete Ideas (blog), 13*(1), 38.
