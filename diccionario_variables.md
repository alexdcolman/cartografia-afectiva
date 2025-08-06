# Diccionario de variables

Este documento presenta el conjunto completo de variables utilizadas en la base anotada del proyecto, incluyendo su clasificación, códigos, valores posibles, definiciones, fundamentos teóricos y notas metodológicas de codificación.

## Formato de presentación

Cada variable se presenta con los siguientes campos:

- **Nombre de la variable**
- **Tipo de variable** (Identificación, Emoción, etc.)
- **Valores posibles**
- **Definición operativa**
- **Fundamento teórico**
- **Notas metodológicas**
- **Bibliografía**

---

## Variables de identificación

### `ID` — Código de identificación 
- **Tipo de variable**: Identificación
- **Valores posibles**: [Número entero]
- **Definición operativa**: Código numérico único asignado a cada observación en la base.
- **Fundamento teórico**: —
- **Notas metodológicas**: —
- **Bibliografía**: —

---

### `COD_REC` — Código de recorte
- **Tipo de variable**: Identificación
- **Valores posibles**: [Texto]
- **Definición operativa**: Código alfanumérico que identifica cada recorte dentro de la base.
- **Fundamento teórico**: —
- **Notas metodológicas**: Tomados de la base de datos de mi investigación doctoral (Colman, 2024).
- **Bibliografía**: —

---

### `RECORTE` — Cita de recorte
- **Tipo de variable**: Identificación
- **Valores posibles**: [Texto]
- **Definición operativa**: Cita textual que constituye el recorte objeto de análisis. A diferencia del “fragmento textual”, el recorte tiene densidad metodológica, ya que remite a la selección de una parte de un texto según criterios analíticos específicos.
- **Fundamento teórico**: Según Fontanille y Zilberberg (2020), el recorte es una operación de segmentación que crea una unidad semiótica con entidad propia, inscrita en una red de relaciones significantes.
- **Notas metodológicas**: Los recortes normalmente respetan los límites de la frase, pero en algunos casos se consideran conglomerados de frases (por ejemplo, párrafos completos) cuando resulta pertinente para el análisis.
- **Bibliografía**: Fontanille y Zilberberg, 2020.

---

### `POSICION` — Posición en el texto (englobante)
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Inicio
    2: Desarrollo
    3: Cierre
    4: Otro
- **Definición operativa**: Segmentación posicional del recorte dentro de la estructura textual general del artículo.
- **Fundamento teórico**: Deriva de la segmentación clásica del texto en partes funcionales, adoptada en narratología.
- **Notas metodológicas**: Según la posición del recorte en la estructura textual de cada artículo (ver base de datos de mi investigación doctoral; Colman, 2024).
- **Bibliografía**: Adam, 1992.

---

### `TIPO_SEC` — Tipo de secuencia englobante del recorte
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Narrativa
    2: Descriptiva
    3: Explicativa
    4: Argumentativa
    5: Dialogal
- **Definición operativa**: Tipo de secuencia englobante del recorte, según las formas prototípicas de organización textual.
- **Fundamento teórico**: Según Adam (1992), existe un número limitado de tipos de secuencia que guían la organización jerárquica de las macroproposiciones textuales. Estas formas permiten reconocer combinaciones típicas de enunciados con una unidad compositiva reconocible.
- **Notas metodológicas**: Clasificación automática mediante LLM y revisada manualmente.
- **Bibliografía**: Adam, 1992; Calsamiglia Blancafort y Tusón Valls, 2007; Charaudeau y Maingueneau, 2005.

---

### `VALENCIA_DISC` — Valencia del discurso
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Positivo
    2: Negativo
    3: Ambivalente
- **Definición operativa**: Evaluación general del tono valorativo-emocional del discurso del recorte.
- **Fundamento teórico**: Se apoya en la Appraisal Theory (Martin y White, 2005) y en los estudios de análisis crítico del discurso (Van Dijk, 1998), que analizan cómo los textos expresan juicios, afectos y actitudes evaluativas.
- **Notas metodológicas**: Clasificación automática mediante LLM y revisada.
- **Bibliografía**: Martin y White, 2005; Van Dijk, 1998.

---

### `TIPO_DISC` — Tipo de discurso
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Científico-académico
    2: Político
    3: Burocrático
    4: Otro
- **Definición operativa**: Clasificación del tipo de discurso según el sector de producción verbal y los modos de estructuración dominantes.
- **Fundamento teórico**: Basado en la distinción entre tipos y géneros discursivos de Charaudeau y Maingueneau (2005).
- **Notas metodológicas**: Clasificación realizada según los tipos de discurso más relevantes en el corpus de mi tesis doctoral (Colman, 2024).
- **Bibliografía**: Calsamiglia Blancafort y Tusón Valls, 2007; Charaudeau y Maingueneau, 2005.

---

### `GEN_DISC` — Género discursivo de inscripción del recorte
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Artículo de investigación
    2: Comunicado/panfleto/volante/etc.
    3: Informe de inteligencia/Memorando/etc.
    4: Entrevista
    5: Otro
- **Definición operativa**: Clasificación del género discursivo de inscripción del recorte.
- **Fundamento teórico**: Se consideran distintos enfoques sobre el género discursivo (Charaudeau, Adam, Bajtín, Heidemann). También se incorpora la noción de “genericidad” como proceso dinámico de producción y reconocimiento.
- **Notas metodológicas**: Clasificación según los géneros dominantes en el corpus de mi tesis doctoral. En caso de hibridez, se consideró el predominio del género en función de la emoción predominante.
- **Bibliografía**: Bajtín, 1997; Calsamiglia Blancafort y Tusón Valls, 2007; Charaudeau y Maingueneau, 2005; Adam y Heidemann, 2004.

---

### `TEMA` — Tema principal del recorte
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Academia, Cultura e Intelectuales (incluye: Censura)
    2: Agricultura y Asentamientos (incluye: Agricultura y Horticultura, Asentamientos y Colonias)
    3: Archivos
    4: Ciencia y Salud (incluye: Ciencia, Hospitales)
    5: Conflictos y Fuerzas Armadas (incluye: Conflictos Bélicos, Militares Veteranos)
    6: Derechos Humanos, Exilio y Memoria (incluye: Derechos Humanos, Exiliados, Memoria e Historia Reciente)
    7: Derechas y Antisemitismo (incluye: Derechas y Anticomunismo, Judíos y Antisemitismo)
    8: Economía y Mundo del Trabajo (incluye: Empresarios, Trabajadores)
    9: Estado y Política Institucional (incluye: Democracia, Estado y Burocracias Estatales, Legalidad)
    10: Dictadura y Fuerzas Represivas (incluye: Dictadura, Fuerzas Represivas y Servicios de Inteligencia, Represión y Violencia)
    11: Género
    12: Iglesia y Cristianismo
    13: Izquierda y Militancia (incluye: Izquierda, Lucha Armada, Organizaciones Políticas y Militancia)
    14: Juventud, Estudiantes y Universidad
    15: Movimientos Sociales y Organizaciones Civiles (incluye: Movimientos Sociales, Organizaciones Civiles, Culturales y Deportivas, Entidades Autárquicas y No Gubernamentales)
    16: Peronismo y Reformismo.
- **Definición operativa**: Categoría temática principal del recorte.
- **Fundamento teórico**: Se considera la noción amplia de “tema” de Bajtín (1997), como orientación temática y objeto de enunciación.
- **Notas metodológicas**: Se reclasificaron los temas registrados en mi tesis doctoral (Colman, 2024). En caso de ambivalencia temática, se priorizó la dominancia.
- **Bibliografía**: Bajtín, 1997.

---

### `ESTILO_ME` — Estilo del recorte (marco enunciativo)
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Académico personal
    2: Académico impersonal
    3: Sin especificar
- **Definición operativa**: Estilo enunciativo dominante del recorte, considerando el marco enunciativo.
- **Fundamento teórico**: Se retoma la noción de “estilo” en Bajtín (1997), reformulada según convenciones discursivas que articulan modo de enunciación, registro y pertenencia institucional.
- **Notas metodológicas**: Clasificación automática mediante LLM y revisada.
- **Bibliografía: Bajtín, 1997.

---

### `ESTILO_C` — Estilo del recorte (incrustado/citado)
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Académico
    2: Coloquial/Testimonial
    3: Político/Ideológico
    4: Administrativo/Burocrático
    5: Narrativo/Cultural
    6: No corresponde
- **Definición operativa**: Estilo del fragmento incrustado o citado dentro del recorte.
- **Fundamento teórico**: Permite diferenciar el estilo dominante del marco enunciativo y el estilo de la citación.
- **Notas metodológicas**: Clasificación automática mediante LLM y revisada.
- **Bibliografía**: Bajtín, 1997.

---

### `ESTILO_REL` — Tipo de relación entre marco e incrustación
- **Tipo de variable**: Identificación
- **Valores posibles**:
    1: Cita directa
    2: Cita indirecta
    3: Cita mixta o encubierta
    4: Evocación de categorías (comillas, cursivas)
    5: No corresponde
- **Definición operativa**: Tipo de relación entre el marco enunciativo y el fragmento incrustado o citado.
- **Fundamento teórico**: Se apoya en la teoría de la heterogeneidad enunciativa, en particular la tipología de las voces citadas propuesta por Authier-Revuz (1984) y Reyes (2002).
- **Notas metodológicas**: Clasificación automática mediante LLM y revisada.
- **Bibliografía**: Authier-Revuz, 1984; Reyes, 2002.

---

## Emoción

### EMOCION — Categoría de emoción
- **Tipo de variable**: Emoción
- **Valores posibles**: [Texto libre]
- **Definición operativa**: Categoría cultural asignada a la emoción predominante presente en el recorte discursivo.
- **Fundamento teórico**: La emoción se concibe como una categoría cultural, en línea con una tradición semiótica y sociodiscursiva que enfatiza su carácter construido y situado.
- **Notas metodológicas**: Clasificación artesanal basada en lectura e interpretación del recorte.
- **Bibliografía**: Parret, 1995b; Plantin, 2014.

---

### DURACION — Duración
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Instantánea  
  2: Durable  
  3: Permanente
- **Definición operativa**: Duración temporal del estado emocional en el discurso, basada en la distinción entre emoción, pasión y sentimiento.
- **Fundamento teórico**:  
  Considerando la dimensión de duración e intensidad, Fontanille distingue entre emoción (instantánea), pasión (durable) y sentimiento (permanente):  
  “[d]e la emoción al sentimiento, conforme la extensión temporal aumenta y se regulariza, la intensidad disminuye” (Fontanille, 2001: 181).  
  La clasificación temporal de la emoción en permanente, durable e instantánea constituye una herramienta clave para analizar las modalidades de inscripción de lo afectivo en los discursos.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Fontanille, 2001; ver nota metodológica sobre la variable.

---

### DOM_EM — Dominio de emoción
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Alegría  
  2: Tristeza  
  3: Ira  
  4: Miedo  
  5: Sorpresa  
  6: Asco
- **Definición operativa**: Clasificación general de la emoción predominante según un conjunto limitado de dominios afectivos básicos.
- **Fundamento teórico**: Dominios de emociones básicas.
- **Notas metodológicas**: Clasificación automática (forzada), realizada por ChatGPT y revisada.
- **Bibliografía**: Habría que revisar clasificaciones de emociones desde distintos campos.

---

### DOM_EM_SEC — Dominio de emoción secundario
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Amor / Confianza / Empatía  
  2: Celos / Sospecha / Desconfianza  
  3: Culpa / Vergüenza  
  4: Decepción  
  5: Esperanza  
  6: Melancolía / Tristeza socializada  
  7: Orgullo / Placer / Satisfacción personal  
  8: Reacción frente al otro (juicio social, respuesta afectiva)  
  9: Ansiedad / Preocupación contextual  
  10: Sorpresa  
  11: Afectación profunda / conmoción emocional
- **Definición operativa**: Subclasificación de matices emocionales presentes en el discurso, complementaria al dominio básico.
- **Fundamento teórico**: Dominios de emociones secundarias.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Habría que revisar clasificaciones de emociones desde distintos campos.

---

### DOMINANCIA — Dominancia de la emoción
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Corporal  
  2: Cognoscitiva  
  3: Mixta
- **Definición operativa**: Dominancia corporal y/o cognoscitiva de la emoción.
- **Fundamento teórico**: Se considera si la emoción se manifiesta principalmente a través de respuestas corporales (viscerales, somáticas) o bien mediante juicios, valoraciones o inferencias.
- **Notas metodológicas**: Clasificación artesanal auxiliada por IA.
- **Bibliografía**: Habría que revisar clasificaciones de emociones desde distintos campos.

---

### FORIA — Foria
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Eufórico  
  2: Disfórico  
  3: Afórico  
  4: Ambifórico
- **Definición operativa**: Carácter fórico de la emoción, es decir, la orientación evaluativa positiva, negativa, neutra o ambigua.
- **Fundamento teórico**: Teoría de la foria como rasgo estructurante del pathos.
- **Notas metodológicas**: Clasificación artesanal auxiliada por IA.
- **Bibliografía**: Greimas y Fontanille, 1994 (revisar definición ahí).

---

### INTENSIDAD — Intensidad de la emoción
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Alta  
  2: Baja  
  3: Neutra / Ambivalente
- **Definición operativa**: Nivel de energía o activación afectiva que presenta la emoción.
- **Fundamento teórico**: Se retoman distinciones tradicionales entre emociones intensas, moderadas y débiles.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Habría que revisar clasificaciones de emociones desde distintos campos.

---

### MODO_EXIST — Modo de existencia semiótica de la emoción
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Realizado  
  2: Potencial  
  3: Actual  
  4: Virtual
- **Definición operativa**:  
  - Virtual: emoción como posibilidad o competencia.  
  - Actual: emoción insinuada o convocada sin realización plena.  
  - Potencial: emoción disponible, activable, proyectada.  
  - Realizado: emoción explícitamente expresada o actuada.
- **Fundamento teórico**: Teoría tensional de los modos de existencia semiótica.
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: Fontanille y Zilberberg, 2016.

---

### F_TEMP — Factor temporal
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Pasado  
  2: Presente  
  3: Futuro
- **Definición operativa**: Temporalidad predominante de la emoción según el anclaje discursivo.
- **Fundamento teórico**: Algunas emociones se orientan hacia el pasado (culpa, nostalgia), otras al futuro (esperanza, ansiedad).
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Fabbri, 2000.

---

### TIPO_TEMP — Tipo temporal
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Proyectivo  
  2: Realizado  
  3: Bloqueado  
  4: Amenazante  
  5: Indefinido  
  6: Súbito  
  7: Cerrado  
  8: Persistente
- **Definición operativa**: Tipo de orientación temporal que estructura la emoción.
- **Fundamento teórico**:  
  - Proyectivo: hacia un objetivo futuro.  
  - Realizado: ya acontecido.  
  - Bloqueado: impedido.  
  - Amenazante: anticipa peligro.  
  - Indefinido: abierto o incierto.  
  - Súbito: irrumpe sin transición.  
  - Cerrado: sin horizonte de cambio.  
  - Persistente: se mantiene en el tiempo.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: ---

---

### F_ASP — Factor aspectual
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Iniciático  
  2: Sostenido  
  3: Culminado  
  4: Interrumpido  
  5: Recurrente  
  6: Clausurado  
  7: Expansivo  
  8: Bloqueado  
  9: Disparado
- **Definición operativa**: Modalidad aspectual del desarrollo de la emoción, según duración, ritmo, despliegue.
- **Fundamento teórico**:  
  - Iniciático: se activa.  
  - Sostenido: se mantiene.  
  - Culminado: se completa.  
  - Interrumpido: se corta.  
  - Recurrente: vuelve.  
  - Clausurado: se cierra.  
  - Expansivo: crece.  
  - Bloqueado: no avanza.  
  - Disparado: estalla.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Fabbri, 2000.

---

### F_MOD — Factor modal
- **Tipo de variable**: Emoción
- **Valores posibles**: [Texto libre]
- **Definición operativa**: Combinación modal relevante para la emoción (querer, poder, saber, deber).
- **Fundamento teórico**: Las emociones se vinculan a modos de posibilidad, necesidad, voluntad y conocimiento.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Fabbri, 2000; Parret, 1995b.

---

### TIPO_F_MOD — Tipo de factor modal
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Potencia afirmativa  
  2: Frustración / impedimento  
  3: Suspensión epistémica  
  4: Disonancia interna  
  5: Desactivación / retiro  
  6: Colisión inevitable  
  7: Realización plena  
  8: Juicio ético / axiológico
- **Definición operativa**: Tipificación del esquema modal predominante que estructura la emoción.
- **Fundamento teórico**: Se consideran configuraciones modales del sujeto frente a su acción, identidad, saber o deseo.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: ---

---

### VEL_ACT — Velocidad de activación de la emoción
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Rápida  
  2: Media  
  3: Lenta
- **Definición operativa**: Rapidez con que la emoción se activa frente a un estímulo o contexto.
- **Fundamento teórico**:  
  - Rápida: emociones súbitas.  
  - Media: requieren procesamiento.  
  - Lenta: se construyen progresivamente.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Habría que revisar autores que utilizan esta variable.

---

### VEL_DIS — Velocidad de disolución de la emoción
- **Tipo de variable**: Emoción
- **Valores posibles**:  
  1: Rápida  
  2: Media  
  3: Lenta
- **Definición operativa**: Tiempo que tarda la emoción en disolverse o dejar de estar activa.
- **Fundamento teórico**:  
  - Rápida: emoción volátil o pasajera.  
  - Media: resolución moderada.  
  - Lenta: se prolonga, persiste o se transforma en estado.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Habría que revisar autores que utilizan esta variable.

---

### F_EST — Factor estésico
- **Tipo de variable**: Emoción
- **Valores posibles**:  
    1: Tónica  
    2: Disfórica  
    3: Eufórica  
    4: Neutra / Apática  
    5: Ambivalente
- **Definición operativa**: Clasifica el tono estésico general de la emoción, es decir, su cualidad sensorial o afectiva de base, tal como se manifiesta en el cuerpo o en su representación discursiva.
- **Fundamento teórico**: Componente estésico de la pasión. Las emociones se corporizan y modulan en distintas formas de intensidad, tono y afectación. Fabbri propone caracterizaciones estésicas (como coloraciones afectivas) que permiten analizar cómo las pasiones afectan el cuerpo y el discurso.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: González Pérez, 2010. [Revisar puntos en común con FORIA]

---

### INSCR_TEMP_E — Inscripción temporal del experienciador
- **Tipo de variable**: Emoción
- **Valores posibles**:  
    1: Presente enunciativo  
    2: Presente contemporáneo  
    3: Pasado de la investigación  
    4: Pasado histórico  
    5: Pasado contemporáneo  
    6: Futuro proyectado
- **Definición operativa**: Codifica el tiempo en el que se inscribe el experienciador de la emoción (el sujeto afectado), según su relación con el momento de la enunciación o del relato.
- **Fundamento teórico**: Las temporalidades del discurso permiten situar las emociones en relación con actores sociales, momentos narrativos e instancias de producción del sentido.
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: ---

---

### INSCR_TEMP_F — Inscripción temporal de la fuente
- **Tipo de variable**: Emoción
- **Valores posibles**:  
    1: Pasado  
    2: Presente  
    3: Futuro
- **Definición operativa**: Determina el anclaje temporal del evento, situación o elemento que desencadena la emoción, en tanto “fuente emocional” construida discursivamente.
- **Fundamento teórico**: Las emociones pueden orientarse hacia hechos pretéritos, situaciones actuales o anticipaciones futuras, lo que incide en su modulación afectiva.
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: ---

---

### ASPECT — Aspectualización de la emoción en el recorte
- **Tipo de variable**: Emoción
- **Valores posibles**:  
    1: Inicio  
    2: Persistencia  
    3: Resolución  
    4: Repetición  
    5: Interrupción / Frustración  
    6: Sin aspecto explícito / ambiguo / no codificable
- **Definición operativa**: Refleja el modo en que la emoción es presentada en su despliegue temporal dentro del recorte discursivo: si se inicia, se mantiene, se repite, se resuelve, se frustra, o no tiene una marcación aspectual clara.
- **Fundamento teórico**: Inspirada en categorías aspectuales lingüísticas y semióticas, así como en la propuesta de Fabbri sobre la existencia cultural de las pasiones.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: ---

---

### TIMICO_FASICO — ¿La emoción es tímica o fásica?
- **Tipo de variable**: Emoción
- **Valores posibles**:  
    0: Fásica  
    1: Tímica
- **Definición operativa**: Distingue si la emoción corresponde a una tonalidad afectiva de base (estado compositivo, tímico) o a una irrupción perturbadora (evento fásico).
- **Fundamento teórico**: Plantin diferencia entre estados afectivos de base (tímicos), que estructuran el horizonte emocional del sujeto, y emociones puntuales o disruptivas (fásicas), que marcan un desequilibrio en ese estado.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.
- **Bibliografía**: Plantin, 2014.

---

### EFECT_PAT — ¿Se trata de un efecto patémico?
- **Tipo de variable**: Emoción
- **Valores posibles**:  
    1: Sí  
    0: No
- **Definición operativa**: Indica si el recorte discursivo construye un efecto de patemización, orientado a generar una reacción emocional en el destinatario.
- **Fundamento teórico**: La patemización es un recurso argumentativo-emocional que busca inducir afectos en el interlocutor o auditorio mediante marcas léxicas, sintácticas o retóricas cargadas emocionalmente.
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: Amossy, 2000; Plantin, 2014.

---

### PRES_TE — Presencia o ausencia de término de emoción
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Indica si hay o no un término de emoción presente en el recorte discursivo.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal
- **Bibliografía**: Plantin, 2014

---

### TIPO_TE — Tipo de término de emoción
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Sustantivo; 2: Adjetivo; 3: Verbo psicológico; 4: No corresponde
- **Definición operativa**: Clasifica gramaticalmente los términos de emoción según su forma léxica predominante.
- **Fundamento teórico**: Plantin caracteriza los términos de emoción con relación a verbos o sustantivos; sin embargo, la existencia de los verbos copulativos “estar” y “parecer” permiten introducir términos de emoción que son participios de determinadas formas verbales (“enojado”, “feliz”). Asimismo, los adjetivos pueden presentarse como modificadores de sustantivos en sintagmas nominales ("memorias lastimadas", "panorama desolador", etc.).
- **Notas metodológicas**: Clasificación artesanal
- **Bibliografía**: Plantin, 2014

---

### PRES_EXP — ¿Hay un experienciador explícito?
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Identifica si hay una instancia subjetiva explícita asociada a la emoción.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal
- **Bibliografía**: Plantin, 2014

---

### EXP — Experienciador
- **Tipo de variable**: ACTANTES
- **Valores posibles**: [TEXTO]
- **Definición operativa**: Actante identificado con el lugar psicológico que experimenta la emoción.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal
- **Bibliografía**: Plantin, 2014

---

### TIPO_EXP — Tipo de experienciador
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Instancias enunciativas; 2: Actores del ámbito represivo; 3: Actores vigilados o reprimidos; 4: Actores contemporáneos
- **Definición operativa**: Clasificación de experienciadores en grandes clases actorales.
- **Fundamento teórico**: Clases amplias relevadas en mi investigación doctoral (Colman, 2024)
- **Notas metodológicas**: ---
- **Bibliografía**: ---

---

### MOD_PRES_EXP — Modo de presencia del experienciador
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Presencia gramatical explícita; 2: Impersonal; 3: Metonimia; 4: Implícito/No marcado; 5: Enunciatario transpuesto
- **Definición operativa**: Clasifica cómo se presenta el experienciador en el discurso: de forma explícita, implícita, desplazada o sugerida.
- **Fundamento teórico**: Ver descripción detallada del instrumento.
- **Notas metodológicas**: Clasificación artesanal auxiliada por IA
- **Bibliografía**: ---

---

### EXP_IND — ¿Es el experienciador un actor que posee el sema "ser = individuo"?
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Identifica si el experienciador es individual o plural de tipo humano.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Se incluyen en "1" los actores plurales (agrupamientos de individuos)
- **Bibliografía**: ---

---

### EXP_INST — ¿Es el experienciador un actor que posee el sema "ser = institución"?
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Indica si el experienciador es una institución.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal
- **Bibliografía**: ---

---

### EXP_TEXT — ¿Es el experienciador un actor que posee el sema "ser = texto"?
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Indica si el experienciador es un texto o artefacto discursivo.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal
- **Bibliografía**: ---

---

### EXP_AG — ¿Ocupa el experienciador un rol de agente del proceso emocional?
- **Tipo de variable**: ACTANTES
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Identifica si el experienciador actúa como agente activo o causa de la emoción.
- **Fundamento teórico**: Ver definición detallada.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada
- **Bibliografía**: Plantin, 2014

---

### PRES_FUE — ¿Hay una fuente explícita?
- **Tipo de variable**: Actantes
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Indica si se menciona explícitamente una fuente de la emoción dentro del recorte discursivo.
- **Fundamento teórico**: Se considera la fuente en sentido amplio, no limitada exclusivamente a enunciados de emoción explícitos.
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: Plantin, 2014.

---

### FUENTE — Fuente
- **Tipo de variable**: Actantes
- **Valores posibles**: [Texto libre]
- **Definición operativa**: Actante desencadenante de la emoción identificada en el recorte.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: Plantin, 2014.

---

### TIPO_FUE — Tipo de fuente
- **Tipo de variable**: Actantes
- **Valores posibles**:  
  1: Archivos, documentos, sus características y/o utilidades  
  2: Acontecimientos y procesos represivos del pasado reciente  
  3: Acontecimientos, actividades o actores vigilados  
  4: Relatos y memorias del pasado  
  5: Organismos de DDHH  
  6: Otros
- **Definición operativa**: Clasificación de las fuentes en seis clases generales construidas a partir del análisis de denominadores comunes en los valores registrados en la variable "FUENTE".
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: ---

---

### PRES_MED — ¿Hay un mediador explícito?
- **Tipo de variable**: Actantes
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Indica si se menciona explícitamente un mediador en la experiencia emocional representada.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: Plantin, 2014; Latour, 2008.

---

### MEDIADOR — Mediador
- **Tipo de variable**: Actantes
- **Valores posibles**: [Texto libre]
- **Definición operativa**: Actante que media la conexión entre un experienciador y una fuente de la emoción.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: Plantin, 2014; Latour, 2008.

---

### TIPO_MED — Tipo de mediador
- **Tipo de variable**: Actantes
- **Valores posibles**:  
  1: Documentos, archivos y prácticas policiales / de inteligencia  
  2: Mediadores informativos y comunicacionales  
  3: Relatos testimoniales y prácticas memoriales  
  4: Publicaciones académicas  
  5: Ausente
- **Definición operativa**: Clasificación de los mediadores en cinco tipos amplios según su forma discursiva o material.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: ---

---

### TIPO_MED_AFEC — Tipo de mediación afectiva
- **Tipo de variable**: Actantes
- **Valores posibles**:  
  1: Testimonial  
  2: Memorial  
  3: Judicializante  
  4: Racionalizadora  
  5: Afecto desplazado  
  6: Silenciamiento o sustracción  
  7: Sin mediación
- **Definición operativa**: Tipología que permite clasificar el modo en que los distintos mediadores discursivos o materiales operan como instancias de modulación, habilitación o desplazamiento de las emociones implicadas en los recortes.
- **Fundamento teórico**: La tipología se construyó inductivamente a partir del corpus, con apoyos conceptuales en la semiótica de las pasiones, los estudios de memoria y los análisis pragmático-discursivos.
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada. Se aplicó una codificación monovaluada por recorte.
- **Bibliografía**: ---

---

### PRES_VN — ¿Hay un verificador normativo explícito?
- **Tipo de variable**: Actantes
- **Valores posibles**: 1: Sí; 0: No
- **Definición operativa**: Indica si aparece un actante que valida, impugna o evalúa la legitimidad de la emoción representada.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal.
- **Bibliografía**: ---

---

### VER_NORM — Verificador normativo
- **Tipo de variable**: Actantes
- **Valores posibles**: [Texto libre]
- **Definición operativa**: Actante que verifica la legitimidad normativa de una emoción, en relación con un actor, un espacio o una situación sociocultural definida. Se retoma la noción de “verificador” propuesta por Berrendonner.
- **Fundamento teórico**: ---
- **Notas metodológicas**: ---
- **Bibliografía**: Berrendonner, 1982.

---

### TIPO_VN — Tipo de verificador normativo
- **Tipo de variable**: Actantes
- **Valores posibles**:  
  1: Institucional/Legal  
  2: Ético/Moral  
  3: Político/Ideológico  
  4: Historiográfico/Académico  
  5: Práctico/Profesional  
  6: Social/Comunitario  
  7: Psico/Patologizante  
  8: Sin verificación
- **Definición operativa**: Clasificación del tipo de instancia que valida o deslegitima una emoción según su marco normativo o criterio de legitimación.
- **Fundamento teórico**: Tipología de verificadores normativos construida para identificar los modos de validación o impugnación de emociones en el discurso. Se define “verificador normativo” como toda instancia que establece, explícita o implícitamente, criterios para juzgar una emoción como legítima, razonable o desproporcionada.
- **Notas metodológicas**: Clasificación automática por ChatGPT y revisada. Se prioriza el anclaje predominante del juicio normativo cuando hay ambigüedad.
- **Bibliografía**: ---

---

### EVAL_NORM — Evaluación normativa del verificador
- **Tipo de variable**: Actantes
- **Valores posibles**:  
  1: La emoción se legitima  
  2: La emoción se deslegitima  
  3: Sin evaluación
- **Definición operativa**: Evaluación asignada por el verificador normativo en relación con la legitimidad de la emoción expresada.
- **Fundamento teórico**: Verificación positiva implica que la emoción es considerada comprensible o apropiada; verificación negativa implica que es desacreditada, desmedida o patológica.
- **Notas metodológicas**: ---
- **Bibliografía**: Frijda, 1986

---

### PRES_VO — ¿Hay un verificador observacional explícito?
- **Tipo de variable**: Actantes
- **Valores posibles**:  
  1: Sí  
  0: No
- **Definición operativa**: Indica si el recorte incluye un actante que constata la realización efectiva de la emoción.
- **Fundamento teórico**: ---
- **Notas metodológicas**: Clasificación artesanal
- **Bibliografía**: ---

---

### VER_OB — Verificador observacional
- **Tipo de variable**: Actantes
- **Valores posibles**: [Texto libre]
- **Definición operativa**: Actante que verifica la realización efectiva de la emoción. Retoma la noción de “verificador” desarrollada por Berrendonner.
- **Fundamento teórico**: ---
- **Notas metodológicas**: ---
- **Bibliografía**: Berrendonner, 1982

---

### TIPO_VO — Tipo de verificador observacional
- **Tipo de variable**: Actantes
- **Valores posibles**:  
  1: Documental  
  2: Enunciador  
  3: Experienciadores específicos  
  4: Fuentes citadas  
  5: Testimonial  
  6: Ausencia
- **Definición operativa**: Clasificación del tipo de actante que acredita la efectividad de la emoción, ya sea como partícipe, testigo, evaluador o fuente documental.
- **Fundamento teórico**: Tipología adaptada de Berrendonner (1982), aplicada a un corpus de discursos sobre archivos de inteligencia, que distingue seis formas de verificación observacional según el rol enunciativo y la mediación documental o testimonial.
- **Notas metodológicas**: Clasificación automática por ChatGPT y revisada.
- **Bibliografía**: Berrendonner, 1982

---

### EVAL_OBS — Evaluación observacional del verificador  
- **Tipo de variable**: Actantes  
- **Valores posibles**:  
  1: La emoción se evalúa como realizada o realizable  
  2: La emoción se evalúa como no realizada o no realizable  
  3: Sin evaluación observacional  
- **Definición operativa**: Determina si el verificador observacional (cuando está presente) valida o niega la efectividad empírica de la emoción.  
- **Fundamento teórico**: ---  
- **Notas metodológicas**: Clasificación artesanal  
- **Bibliografía**: ---

---

### SUJ_GR — ¿Con qué actante del simulacro se identifica el sujeto gramatical?  
- **Tipo de variable**: Actantes  
- **Valores posibles**:  
  1: Experienciador  
  2: Fuente  
  3: Emoción  
  4: Mediador  
  5: Atribuidor  
  6: Otros/No corresponde  
- **Definición operativa**: La variable SUJ_GR permite establecer una conexión analítica entre la estructura sintáctica de los recortes discursivos y las funciones actanciales del simulacro emocional. En concreto, clasifica al sujeto gramatical en función de su alineación con alguno de los siguientes roles: (1) Experienciador, (2) Fuente (o desencadenante de la emoción), (3) Emoción como entidad autónoma, (4) Mediador, (5) Atribuidor, o (6) Otros/No corresponde.  
Esta variable cumple un rol central por cuatro motivos principales:  
1) Vincula estructura sintáctica y estructura actancial: Permite observar si el sujeto gramatical ocupa la posición del experienciador de la emoción, si representa a la fuente que la desencadena, o si, en cambio, se identifica con el propio contenido emocional o con un mediador. Esta relación es clave para analizar desde dónde se enuncia la emoción y qué tipo de construcción enunciativa se privilegia.  
2) Revela formas de identificación enunciativa: La codificación del sujeto gramatical según su función actancial permite mapear diferentes formas de empatía, atribución o distanciamiento en el discurso. Por ejemplo, identificar al sujeto gramatical con el experienciador puede sugerir un posicionamiento empático, mientras que su identificación con la fuente puede implicar una atribución de responsabilidad emocional a un otro.  
3) Permite estudiar patrones de subjetivación y posicionamiento: La distribución de las funciones actanciales asignadas al sujeto gramatical habilita el análisis de regularidades discursivas según el tipo de texto, estilo discursivo o tono emocional. Esto es especialmente útil para examinar, por ejemplo, si los discursos testimoniales tienden a asumir al experienciador como sujeto gramatical, mientras que los discursos institucionales delegan esa función en mediadores o fuentes externas. Asimismo, permite identificar casos excepcionales en los que la emoción misma es tematizada como sujeto (caso 3), lo que puede ser indicio de una autonomización afectiva en el discurso.  
4) Facilita cruces con otras variables: Al estar formalizada como variable categórica, SUJ_GR puede ser cruzada con otras dimensiones de análisis —como tipo de mediador, modalidad emocional, estilo discursivo o tipo de fuente— para detectar patrones ideológicos, estrategias retóricas o dispositivos de enunciación característicos de cada corpus.  

Criterio adicional para oraciones compuestas: En los casos en que el simulacro emocional se localiza en una proposición subordinada (por ejemplo, en construcciones como “lo interesante es que…”), se considera únicamente la oración subordinada para el análisis de SUJ_GR, siempre y cuando los demás elementos del simulacro emocional (como el atribuidor, el mediador o la fuente) no se encuentren fuera de dicha proposición. Esto permite aislar con mayor precisión la configuración actancial de la emoción, evitando que estructuras sintácticas más amplias interfieran en la codificación específica del simulacro emocional.  

En suma, SUJ_GR funciona como una variable relacional que articula dimensiones sintácticas, actanciales y enunciativas, proporcionando un instrumento potente para el estudio de la semiotización de la emoción en el discurso.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada  
- **Bibliografía**: ---

---

### TIPO_VERB — Tipo de verbo vinculado a la configuración del simulacro emocional (si aplica)  
- **Tipo de variable**: Actantes  
- **Valores posibles**:  
  1: Transitivo  
  2: Intransitivo  
  3: Copulativo  
  4: Copulativo existencial  
  5: Transitivo pronominal  
  6: No corresponde  
- **Definición operativa**: La variable TIPO_VERB indica el tipo de verbo vinculado a la configuración del simulacro emocional, si corresponde. El tipo se clasifica según la transitividad y la función sintáctica del verbo en el enunciado.  

Criterios de codificación:  
1. Se codifica la transitividad del verbo base que estructura la configuración emocional, independientemente de su forma gramatical concreta (verbo conjugado, infinitivo, participio, gerundio, etc.).  
2. En construcciones pasivas (por ejemplo, participios pasivos como "reconocida", "movilizadora"), se toma en cuenta la transitividad inherente al verbo base, ya que mantiene la relación verbo-agente-paciente, aunque no esté conjugado en forma personal. En estos casos, la categoría será la correspondiente a la transitividad del verbo base (por ejemplo, reconocer es transitivo, por lo que se codifica como 1).  
3. La categoría "6: No corresponde" se asigna cuando no hay verbo explícito vinculado a la emoción o cuando la construcción no permite identificar un verbo estructurante (por ejemplo, en oraciones nominales o frases sin verbo).  
4. Los verbos copulativos incluyen aquellos que funcionan para unir sujeto y atributo (por ejemplo, ser, estar), diferenciando entre copulativo simple (3) y existencial (4).  
5. Se registran los verbos transitivos pronominales (5) cuando la transitividad se acompaña de pronombres reflexivos que afectan la estructura del verbo.  
6. Se consideran únicamente los verbos que forman parte de la estructura actancial interna del simulacro emocional, es decir, aquellos que participan directamente en la configuración de la emoción enunciada o inferida. Verbos que aparecen en el enunciado pero que no forman parte de esta estructura actancial, como aquellos vinculados a la atribución externa de la emoción por otros actores, se codifican como 6 (No corresponde). Por ejemplo, en el recorte: "Allí se registran el interés por desarrollar cursos de aprendizaje en torno de la inteligencia política" (KAHAN1, 138), el verbo "se registran" está vinculado a la atribución del interés y no a la estructura interna del simulacro emocional, por lo cual se codifica como 6.  
- **Notas metodológicas**: Clasificación artesanal auxiliada por IA  
- **Bibliografía**: Plantin, 2014; Colman, 2025

---

### TIPO_VPSI — Tipo de verbo psicológico  
- **Tipo de variable**: Actantes  
- **Valores posibles**:  
  1: VPSI1  
  2: VPSI2  
  3: VPSI2 (reflex.)  
  4: VPSI3  
  5: No corresponde  
- **Definición operativa**: Clasificación del tipo sintáctico-semántico del verbo psicológico presente en el enunciado, basada en la distinción de Plantin (2014) entre verbos psicológicos de primera, segunda y tercera clase, adaptada al funcionamiento del español. Se incluyen además las variantes reflexivas.  

Categorías:  
1. VPsi1: Verbo psicológico de primera clase. El sujeto es la persona que experimenta la emoción (experienciador), el objeto es la fuente o estímulo. “Juan admira a María”  
2. VPsi2: Verbo psicológico de segunda clase. El sujeto es la fuente o estímulo, el objeto directo (introducido con “a”) es el experienciador. La construcción admite pasiva. “El discurso impactó a los oyentes” → “Los oyentes fueron impactados por el discurso”  
3. VPsi2 reflexivo: Variante reflexiva del VPsi2. El experienciador es también el sujeto del verbo, expresado mediante pronombre reflexivo. “Juan se emocionó con la música”  
4. VPsi3: Verbo psicológico intransitivo con complemento de dativo (objeto indirecto). El sujeto es el estímulo, el experienciador aparece como complemento preposicional. No admite pasiva. “La música le gusta a Juan” → ❌ “Juan fue gustado”  
5. No corresponde: No hay verbo psicológico, o el uso no implica una experiencia emocional.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada  
- **Bibliografía**: Plantin, 2014

---

### VERB_MET — Presencia o ausencia de verbo metafórico  
- **Tipo de variable**: Actantes  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Identifica la presencia de un verbo que, aunque no sea un verbo psicológico prototípico, funciona metafóricamente como portador de una experiencia emocional en el fragmento discursivo.  
- **Fundamento teórico**: Basada en Plantin (2014), que reconoce una clase extendida de verbos psicológicos por metáfora, donde verbos con significado literal no emocional adquieren carga afectiva cuando se usan metafóricamente en contextos enunciativos adecuados.  
- **Notas metodológicas**:  
  - Se asigna 1 si el verbo cumple las condiciones de uso metafórico emocional: no es un verbo psicológico canónico, tiene uso metafórico que evoca emoción y el contexto permite inferir el tipo de emoción.  
  - Incluye participios usados con valor metafórico afectivo (ej. “memorias lastimadas”).  
  - Se asigna 0 cuando no hay verbo metafórico, el verbo es un verbo psicológico literal o la emoción solo se expresa mediante adjetivos o sustantivos sin verbo metafórico.  
- **Bibliografía**: Plantin, 2014

---

### VEI — Presencia o ausencia de verbo de evidencia o inferencia  
- **Tipo de variable**: Actantes  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica la presencia de un verbo o construcción verbal que expresa un proceso cognitivo de evidencia, inferencia o reconocimiento, utilizado por un hetero-atribuidor para interpretar o atribuir una emoción a un sujeto o situación desde un soporte de atribución externo.  
- **Fundamento teórico**: Refleja un proceso hermenéutico donde la emoción no es vivida directamente por el experienciador sino inferida discursivamente desde documentos, testimonios, observaciones u otros soportes externos. Marca mediación interpretativa y atribución heterodiegética.  
- **Notas metodológicas**:  
  - Se codifica 1 si hay verbos o construcciones que expresan inferencia o evidencia (ej. confirmar, reconocer, indicar, se podía inferir, resulta claro que), con atribución mediada a otro actor.  
  - Se codifica 0 si la emoción es expresada directamente, no hay verbos de evidencia o inferencia, o el uso es analítico sin atribución emocional concreta.  
  - Ejemplo: “experiencia reconocida por los alumnos como movilizadora” no se codifica como VEI si la emoción es reconocida directamente por los experienciadores sin mediación inferencial.  
- **Bibliografía**: REVISAR LITERATURA  

---

## Modificaciones

---

### PRES_OP_MOD — Presencia o ausencia de operadores de modificación emocional  
- **Tipo de variable**: Modificaciones  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica si en el recorte discursivo se identifica algún operador que modula la emoción, ya sea activándola, inhibiéndola o transformándola.  
- **Fundamento teórico**: Se reconoce que la emoción en el discurso puede ser sometida a procesos de modificación mediante instancias actanciales, enunciativas o retóricas que alteran su emergencia, intensidad o forma.  
- **Notas metodológicas**:  
  - Se codifica 1 solo si hay evidencia clara de dinámica transformativa sobre la emoción (activación, inhibición o pasaje).  
  - Se codifica 0 si la emoción aparece ya expresada o establecida sin mecanismos de modificación visibles.  
  - En caso positivo, se debe describir el operador en OP_MOD.  
- **Bibliografía**: Clasificación artesanal, Colman, 2025

---

### OP_MOD — Operador de modificación emocional  
- **Tipo de variable**: Modificaciones  
- **Valores posibles**: [Texto libre]  
- **Definición operativa**: Descripción textual del operador semiótico o actancial que actúa sobre la emoción, especificando su naturaleza y función (activar, inhibir o modificar).  
- **Fundamento teórico**: Los operadores son agentes, dispositivos discursivos o mecanismos retóricos que producen cambios en el estado emocional atribuido en el discurso.  
- **Notas metodológicas**:  
  - Se registra quién o qué actúa como operador y qué función cumple.  
  - Ejemplos: “la amenaza funciona como operador de activación”, “el juicio del enunciador inhibe la sorpresa”, “la argumentación desplaza el miedo hacia la indignación”.  
- **Bibliografía**: Clasificación artesanal, Colman, 2025

---

### TIPO_OP_MOD — Tipo de operador de modificación emocional  
- **Tipo de variable**: Modificaciones  
- **Valores posibles**:  
  1: Acontecimientos o situaciones históricas  
  2: Dispositivos documentales  
  3: Actantes discursivos o enunciativos  
  4: Material testimonial y narrativo  
  5: Actores sociales o colectivos  
  6: Material cultural, propagandístico o persuasivo  
  7: Otros  
  8: No corresponde  
- **Definición operativa**: Clasificación del tipo de entidad o mecanismo que cumple la función de operador en la modificación emocional.  
- **Fundamento teórico**: Permite distinguir la naturaleza del operador en función de su origen y rol en el discurso.  
- **Notas metodológicas**: Clasificación automática revisada.  
- **Bibliografía**: ---

---

### FUNCION_OP_MOD — Tipo de función básica que cumple el operador emocional identificado  
- **Tipo de variable**: Modificaciones  
- **Valores posibles**:  
  1: Activación  
  2: Inhibición  
  3: Modificación  
  4: No corresponde  
- **Definición operativa**: Categoriza la función primaria que cumple el operador en la dinámica emocional del discurso, distinguiendo si el operador genera, limita o transforma una emoción.  
- **Fundamento teórico**: Diferencia la acción elemental del operador en la gestión del campo emocional, sin entrar en estrategias complejas o trayectorias.  
- **Notas metodológicas**:  
  - Solo se codifica si PRES_OP_MOD=1.  
  - Priorizar la función predominante si hay más de una.  
  - Ejemplos: amenaza que activa (1), juicio que inhibe (2), relato que transforma (3).  
- **Bibliografía**: ---

---

### TIPO_MODIF — Tipo de modificación emocional  
- **Tipo de variable**: Modificaciones  
- **Valores posibles**:  
  1: Transformación  
  2: Sustitución/Conversión  
  3: Resolución  
- **Definición operativa**: Clasifica la forma específica de cambio emocional provocada por el operador, distinguiendo si la emoción cambia cualidad manteniendo objeto valorado, si cambia objeto o si se disipa o neutraliza.  
- **Fundamento teórico**: La modificación emocional puede implicar pasajes internos en el mismo objeto, cambio de objeto valorado o el cierre de la trayectoria afectiva.  
- **Notas metodológicas**:  
  - Se usa principalmente para operadores de inhibición y modificación, no para activaciones.  
  - Ejemplos: pasar de “amar” a “odiar” (transformación), cambiar de objeto emotivo (sustitución), mitigación o fin de emoción (resolución).  
- **Bibliografía**: Parret, 1995a  

---

### TIPO_MANIP — Tipo de manipulación actancial de la emoción  
- **Tipo de variable**: Modificaciones  
- **Valores posibles**:  
  1: Argumentación emocional  
  2: Persuasión afectiva  
  3: Activación emocional/Exhortación  
  4: Inhibición  
  5: Desplazamiento afectivo  
  6: Transferencia empática  
  7: Normalización emocional  
  8: Condicionamiento emocional  
  9: Ocultamiento  
  10: Modelización afectiva  
  11: No corresponde  
- **Definición operativa**: Clasifica las operaciones discursivas o actanciales que buscan modificar o interferir en la emoción del experienciador mediante estrategias semióticas que actúan sobre la configuración afectiva, tales como justificación, persuasión, exhortación, control o desplazamiento emocional.  
- **Fundamento teórico**: Basada en la noción de manipulación semiótica (Greimas y Courtés, 2006; Parret, 1995a) y desarrollos sobre actancialidad emocional (Plantin, 2010). La manipulación emocional se entiende como el conjunto de estrategias discursivas dirigidas a inducir, restringir, desplazar o modelar emociones en el sujeto enunciativo o sus referidos.  
- **Notas metodológicas**:  
  - Los tipos incluyen operaciones argumentativas (legitimación, normalización, modelización, condicionamiento), performativas o exhortativas (persuasión, activación), reorganización del objeto emocional (desplazamiento, transferencia empática) y control del régimen de visibilidad (ocultamiento, inhibición).  
  - La categoría “No corresponde” se usa cuando no hay manipulación actancial identificable.  
  - Se pueden codificar múltiples tipos simultáneamente si están presentes.  
- **Bibliografía**: Plantin, 2010; Greimas y Courtés, 2006; Parret, 1995a  

---

## Identificación y atribución

---

### MODO_IDEN — Modo de identificación de la emoción  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**:  
  1: Directa  
  2: Por señales de salida  
  3: Por señales de entrada  
  4: Mixta  
- **Definición operativa**: Categoriza la vía por la cual la emoción se identifica en el recorte discursivo, ya sea mediante declaración explícita (emoción dicha), a partir de señales observables del estado emocional (señales de salida), o bien por indicios narrativos o descriptivos que sustentan la emoción (señales de entrada).  
- **Fundamento teórico**: Basada en Plantin (2014) y Micheli (2013), que distinguen vías directa e indirectas para identificar emociones en el discurso, incluyendo emociones expresadas, mostradas o sostenidas mediante señales.  
- **Notas metodológicas**: La categoría “Mixta” se asigna cuando coexisten vías combinadas en el mismo fragmento, por ejemplo emoción dicha con señales de salida o entrada. La clasificación requiere lectura interpretativa y análisis contextual.  
- **Bibliografía**: Plantin, 2014; Micheli, 2013  

---

### TIPO_ATR — Tipo de atribución de la emoción  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**:  
  1: Auto-atribución  
  2: Hetero-atribución  
  3: Atribución transpositiva  
- **Definición operativa**: Define quién atribuye la emoción al experienciador: si el propio enunciador (auto-atribución), un tercero (hetero-atribución), o el analista/investigador a partir de señales indirectas (atribución transpositiva).  
- **Fundamento teórico**: Inspirada en Rabatel (2012) y Parret (1995a), se reconoce que la atribución puede ser directa o inferida, y que el análisis discursivo puede realizar atribuciones transpositivas basadas en signos indirectos.  
- **Notas metodológicas**: La asignación requiere evaluación interpretativa sobre la fuente del enunciado emocional y el sujeto atribuyente.  
- **Bibliografía**: Plantin, 2014; Rabatel, 2012; Parret, 1995a  

---

### SOP_ATR — Soporte de la atribución  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**: [Texto libre]  
- **Definición operativa**: Descripción textual del soporte o base desde el cual el atribuidor asigna la emoción al experienciador, pudiendo incluir documentos, testimonios, discursos o procesos interpretativos.  
- **Fundamento teórico**: El soporte es el fundamento discursivo o contextual que habilita la atribución emocional, constituyendo el marco semiótico o material desde el cual se interpreta la emoción.  
- **Notas metodológicas**: Clasificación artesanal, basada en la identificación explícita o inferida del soporte en el recorte.  
- **Bibliografía**: Colman, 2024  

---

### TIPO_SOP_ATR — Tipo de soporte de la atribución  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**:  
  1: Producción académica o interpretativa  
  2: Material institucional o político  
  3: Testimonio o experiencia vivida  
  4: Procesamiento afectivo reflexivo  
- **Definición operativa**: Clasifica el tipo de material o base desde la cual se realiza la atribución de la emoción, diferenciando fuentes académicas, institucionales, testimoniales o procesos internos reflexivos.  
- **Fundamento teórico**: Basado en criterios contextuales que reconocen diferentes tipos de soportes discursivos y materiales para la atribución emocional.  
- **Notas metodológicas**: La codificación requiere lectura interpretativa y contextualización de la fuente o soporte textual.  
- **Bibliografía**: --  

---

### ATRIBUIDOR — Atribuidor de la emoción  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**:  
  1: Enunciador  
  2: Actor discursivo  
  3: Analista  
- **Definición operativa**: Identifica quién realiza la atribución de la emoción al experienciador, pudiendo ser el mismo enunciador, un personaje o actor dentro del discurso, o el analista que interpreta la emoción.  
- **Fundamento teórico**: Reconoce diferentes planos en la atribución emocional, desde la instancia enunciativa hasta la intervención interpretativa externa.  
- **Notas metodológicas**: Clasificación artesanal basada en análisis del contexto y fuente del enunciado.  
- **Bibliografía**: Plantin, 2014  

---

### ATRIB_DIREC — ¿La emoción es atribuible directamente?  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica si la emoción está explícitamente atribuida a un actor o instancia en el discurso (directa) o si la atribución debe inferirse a partir de relaciones semánticas, modalidades o distanciamientos enunciativos (indirecta).  
- **Fundamento teórico**: La distinción ayuda a diferenciar entre emociones expresadas explícitamente y emociones inferidas mediante análisis discursivo, ampliando la comprensión de la atribución emocional.  
- **Notas metodológicas**: Requiere un análisis cuidadoso del vínculo entre términos emocionales y actores en el texto.  
- **Bibliografía**: Colman, 2025  

---

### TIPO_CONF — Tipo de configuración del simulacro emocional  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**:  
  1: Sostenido en sustantivos  
  2: Sostenido en adjetivos  
  3: Ordenados alrededor de verbos psicológicos  
  4: Cualificación afectiva por indicadores cognitivos  
  5: Cualificación afectiva por indicadores de comportamiento  
  6: Cualificación afectiva por indicadores axiológicos  
  7: Cualificación afectiva por componentes descriptivo-narrativos  
  8: Cualificación afectiva por transposición de la situación de reconocimiento potencial  
- **Definición operativa**: Describe el modo principal en que se configura o articula el simulacro emocional en el recorte discursivo, a partir de categorías lingüísticas o semióticas que sostienen la emoción.  
- **Fundamento teórico**: Basado en Plantin (2014) y desarrollos propios, distingue formas variadas en que la emoción se expresa o sostiene en el discurso, desde formas léxicas hasta mecanismos narrativos o inferenciales.  
- **Notas metodológicas**: Requiere lectura e interpretación detallada del recorte, considerando indicadores lingüísticos, semánticos y narrativos.  
- **Bibliografía**: Plantin, 2014; Colman, 2025  

---

### MODO_SEMIOT — Modo de semiotización de la emoción  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**:  
  1: Dicha  
  2: Mostrada  
  3: Sostenida  
- **Definición operativa**: Describe la modalidad mediante la cual la emoción está presente en el recorte discursivo, distinguiendo si la emoción es expresada explícitamente (dicha), manifestada indirectamente a través de indicadores o comportamientos (mostrada) o inferida mediante la representación de situaciones culturalmente asociadas (sostenida).  
- **Fundamento teórico**: Basada en Plantin (2014) y Micheli (2013), esta variable articula la presencia emocional según grados de explicitud e inferencia en el discurso, vinculando modalidades semióticas diversas para capturar la emocionalidad discursiva.  
- **Notas metodológicas**: La codificación se realiza mediante análisis contextual, identificando la forma de presencia emocional predominante en el fragmento. Se permite la interpretación artesanal basada en lectura crítica.  
- **Bibliografía**: Micheli, 2013; Plantin, 2014  

---

### OBJET_EVAL — La emoción aparece objetivada como una cualidad del objeto discursivo que funciona como fuente  
- **Tipo de variable**: Identificación y atribución  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica si la emoción se proyecta como una propiedad o cualidad atribuida al objeto o situación discursiva que actúa como fuente emocional, sin presencia explícita de un experienciador, lo que implica una evaluación subjetiva implícita o comunitaria.  
- **Fundamento teórico**: Inspirada en Apothéloz (1984) y Borel (1984), esta variable reconoce formas de reificación afectiva donde la emoción se convierte en atributo del objeto, lo que afecta la configuración discursiva y la valoración tácita.  
- **Notas metodológicas**: Se codifica como 1 cuando la emoción se construye como propiedad del objeto/situación, incluso si aparece matizada o atenuada por modalizaciones; se codifica como 0 cuando la emoción está vinculada a un sujeto experienciador, explícito o implícito.  
- **Bibliografía**: Apothéloz, 1984; Borel, 1984; Colman, 2025  

---

## Recursos

### INDIC_AX — Presencia de indicadores axiológicos vinculados a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Registra la existencia en el fragmento de expresiones o elementos discursivos que manifiestan juicios de valor sobre personas, situaciones, grupos sociales, acciones u objetos, que sustentan o activan inferencias emocionales. Incluye adjetivos, verbos de juicio, sustantivos valorativos, categorizaciones ideológicas, y marcos narrativos que construyen oposiciones axiológicas. También se considera la valoración implícita expresada a través de reacciones que implican una ruptura normativa o institucional.  
- **Fundamento teórico**: Fundada en una perspectiva semiótica y discursiva, que concibe la emoción como respuesta evaluativa mediada por estructuras de valor en el texto (Amossy, 2000, 2010; Charaudeau y Maingueneau, 2005; Kerbrat-Orecchioni, 1993; Perelman y Olbrechts-Tyteca, 1994).  
- **Notas metodológicas**: La codificación se realiza mediante análisis contextual y crítico, valorando tanto elementos lingüísticos explícitos como inferencias apoyadas en el conocimiento sociocultural. En casos de ambigüedad, se opta por una interpretación restrictiva (valor 0).  
- **Bibliografía**: Amossy, 2000, 2010; Charaudeau y Maingueneau, 2005; Kerbrat-Orecchioni, 1993; Perelman y Olbrechts-Tyteca, 1994  

---

### TEC_ARG — Presencia de técnicas de argumentación vinculadas a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica si en el discurso se emplean técnicas argumentativas orientadas a generar, intensificar o expresar emociones en el destinatario o en el propio argumentador. Se consideran técnicas como apelaciones emotivas, ejemplos conmovedores, preguntas retóricas con efecto afectivo, o manifestaciones emocionales explícitas o implícitas del emisor. No incluye técnicas de refutación ni figuras de agresión, que se codifican por separado.  
- **Fundamento teórico**: Basada en la teoría de la Nueva Retórica de Perelman y Olbrechts-Tyteca (1994), que reconoce la importancia del pathos en la argumentación, y en enfoques retórico-discursivos que distinguen las técnicas argumentativas de otras formas discursivas confrontativas (Reale y Vitale, 2004).  
- **Notas metodológicas**: La codificación requiere una lectura atenta del contexto para distinguir técnicas argumentativas afectivas de refutaciones o figuras agresivas. Ante dudas, se favorece la identificación clara de técnicas con función emocional para asignar valor 1.  
- **Bibliografía**: Perelman y Olbrechts-Tyteca, 1994; Reale y Vitale, 2004  

---

### TEC_REF — Presencia de técnicas de refutación vinculadas a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Registra la presencia o ausencia de técnicas de refutación en el fragmento discursivo que estén afectivamente moduladas o emocionalmente significativas. Se incluyen técnicas como desplazamiento del problema, ejemplo en contrario, argumentación ad hominem, descalificación del adversario, metástasis, paralogismo imputado, apodioxis, inversión del punto de vista, desmitificación, evocación de la realidad, retorsión y autofagia, siempre que expresen o provoquen emociones como indignación, sarcasmo, desprecio o rechazo.  
- **Fundamento teórico**: Basada en la noción de refutación de Reale y Vitale (2004), que la entienden como procedimiento retórico orientado a debilitar la posición del adversario mediante recursos argumentativos cargados afectivamente. Se considera su función en la articulación de la afectividad en contextos polémicos y de confrontación ideológica.  
- **Notas metodológicas**: La codificación requiere identificar la carga emocional asociada a la refutación, diferenciándola de refutaciones neutrales o meramente racionales. Solo se codifican refutaciones con dimensión emocional reconocible.  
- **Bibliografía**: Reale y Vitale, 2004  

---

### FIG_AGR — Presencia de figuras de la agresión vinculadas a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Señala la existencia de figuras retóricas agresivas en el fragmento discursivo, que buscan atacar, desacreditar o desestabilizar al adversario y que están emocionalmente cargadas. Incluye injuria o insulto explícito, sarcasmo, ironía con carga emocional, hipérbole negativa, concesión retórica, ridiculización o parodia, atribución de intenciones maliciosas y discordancias estilísticas o lógicas, siempre con función afectiva intensificadora de emociones negativas o confrontativas.  
- **Fundamento teórico**: Fundamentada en el análisis de la polémica argumentativa según Angenot (1982) y Reale y Vitale (1995), que destacan estas figuras como formas afectivas del discurso confrontativo orientadas a activar indignación, desprecio, burla o temor en el destinatario.  
- **Notas metodológicas**: Se codifica solo la presencia clara y significativa de al menos una figura de agresión con carga emocional. Requiere interpretación contextual para distinguir de otras formas discursivas.  
- **Bibliografía**: Reale y Vitale, 2004  

---

### ESCEN_EMO — Presencia de escenificaciones emocionales (descriptivo-narrativas o figurales)  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica si el recorte contiene componentes discursivos que escenifican afectivamente una situación, hecho, imagen o acontecimiento, contribuyendo a la producción, modulación o inferencia de una emoción. Incluye relatos, descripciones sensoriales o espaciales, metáforas, enumeraciones condensadas y escenas hipotéticas que construyen un escenario emocional.  
- **Fundamento teórico**: Se fundamenta en una perspectiva semiótico-discursiva que considera que la emoción puede construirse discursivamente mediante formas de representación del mundo (Plantin, Fontanille, Adam), a través de relatos, figuras, espacios y objetos cargados afectivamente.  
- **Notas metodológicas**: La codificación se realiza automáticamente y debe distinguirse de meras afirmaciones o evaluaciones emocionales sin escenificación concreta. Se valoran formas tanto amplias (relatos) como condensadas (metáforas).  
- **Bibliografía**: Adam, 2001; Fontanille, 2001  

---

### INDIC_COG — Presencia de marcas discursivas de orientación o evaluación cognitiva explícita vinculadas a la emoción inferida  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Registra la presencia de expresiones que representan procesos cognitivos (focalización, atención, clarificación, evaluación) o marcas modales (certeza, duda, necesidad) vinculadas a la inferencia de una emoción. Incluye metáforas cognitivas, verbos de actividad intelectual y juicios epistémicos, apreciativos o deónticos que afectan el sentido emocional del fragmento.  
- **Fundamento teórico**: Basada en la semiótica discursiva que entiende las emociones como inferidas a partir de operaciones cognitivas y modales del discurso, configurando huellas afectivas indirectas (Colman, Martin & White, Plantin).  
- **Notas metodológicas**: No se codifican expresiones de emociones explícitas ni comportamientos corporales; solo se registran indicios cognitivos y modales que implican afecto. Se incluye la representación de perspectivas enunciativas diversas.  
- **Bibliografía**: Colman, 2025; Martin y White, 2005; Plantin, 2011  

---

### INDIC_COMP — Presencia de indicadores de comportamiento vinculados a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Señala la presencia de acciones, gestos, reacciones corporales o expresiones físicas que permiten inferir una emoción, constituyendo una figurativización corporal o situacional del pathos. Incluye tanto conductas emocionales prototípicas (llorar, gritar) como signos corporales (temblar, mirada fija).  
- **Fundamento teórico**: Inspirada en la semiología del cuerpo y la figurativización pasional (Fontanille), donde la emoción se articula como acontecimiento corporal observable y significativo en el discurso.  
- **Notas metodológicas**: Se excluyen marcas cognitivas o modales y emociones enunciadas explícitamente sin representación comportamental. Se codifica a partir de la lectura del comportamiento descrito o narrado.  
- **Bibliografía**: Fontanille, 2001  

---

### FIG_RET — Presencia de figuras retóricas vinculadas a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica si el recorte contiene figuras retóricas que modulan, intensifican o configuran la expresión afectiva, tales como metáforas, metonimias, hipérboles, ironías, anáforas, paralelismos o interrogaciones retóricas. Estas figuras deben estar vinculadas expresamente a la emoción inferida, ser atribuibles al experienciador señalado y operar como configuraciones formales del afecto en el discurso.  
- **Fundamento teórico**: Basada en la perspectiva discursiva de la retórica como construcción del pathos, donde las figuras retóricas no son meros ornamentos sino estrategias que articulan la pasión como modo de decir (Fontanille, Amossy).  
- **Notas metodológicas**: Codificación automática y revisada, requiere identificar la relación entre figura y emoción, y atribuirla enunciativamente. No se consideran figuras neutrales o ajenas a la emoción.  
- **Bibliografía**: Amossy, 2000, 2010; Beristáin, 1997; Groupe µ, 1970  

---

### MOD_ENUNCIAC — Presencia de modalidades de enunciación vinculadas a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Registra modalidades de enunciación (declarativas, interrogativas, exclamativas, imperativas) que modulan la relación entre enunciador y acto de habla, incidiendo en la tonalidad afectiva y en el posicionamiento emocional del enunciador respecto al discurso.  
- **Fundamento teórico**: Se entiende que las modalidades de enunciación constituyen actos discursivos que producen o intensifican emociones desde la forma misma del enunciado (Etkin, Maingueneau).  
- **Notas metodológicas**: Codificación automática y revisada. Se considera el efecto modal o tonal sobre la emoción, no sólo la forma gramatical.  
- **Bibliografía**: Etkin, 2016; Maingueneau, 2009  

---

### MOD_ENUNCIAD — Presencia de modalidades de enunciado vinculadas a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Registra modalidades epistémicas, apreciativas o deónticas en el contenido del enunciado que modulan grados de certeza, posibilidad, valoración o necesidad y participan en la estructuración emocional del discurso. Incluye verbos modales, adverbios modales y construcciones complejas.  
- **Fundamento teórico**: Fundada en la semiótica discursiva, estas modalidades configuran el compromiso afectivo del enunciador con el contenido y contribuyen a la construcción de la emoción inferida (Etkin, Maingueneau).  
- **Notas metodológicas**: Codificación automática y revisada; se distinguen claramente de modalidades puramente informativas o neutrales.  
- **Bibliografía**: Etkin, 2016; Maingueneau, 2009  

---

### POLIF_HETER — Presencia de marcas de polifonía o heterogeneidad mostrada marcada vinculadas a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica si el recorte presenta huellas lingüísticas explícitas de otras voces enunciativas (citas directas o indirectas, estilo libre indirecto, comillas, preguntas retóricas con destinatarios implícitos) que intervienen en la construcción o expresión de la emoción. No se codifica si sólo hay mención sin reproducción textual ni marcas claras de voz ajena.  
- **Fundamento teórico**: Desde la teoría de la polifonía discursiva, la heterogeneidad enriquece la construcción emocional, permite el diálogo de posiciones y afecta la responsividad afectiva (Authier-Revuz, Ducrot).  
- **Notas metodológicas**: Codificación automática y revisada, requiere identificar marcas lingüísticas explícitas y funcionalidad afectiva.  
- **Bibliografía**: Authier-Revuz, 1984, 1995; Ducrot, 1986; Reyes, 1990  

---

### ECOIC_EIL — Presencia de ecoicidad y/o estilo indirecto libre vinculados a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Indica la presencia de construcciones discursivas que incorporan implícita o semi-citada otra voz o pensamiento dentro del discurso sin citas literales, mediante ecoicidad o estilo indirecto libre, modulando la expresión o producción emocional. Incluye tensiones o resonancias con voces ajenas sin reproducción textual explícita.  
- **Fundamento teórico**: Basada en la noción de ecoicidad y estilo indirecto libre como estrategias de incorporación no literal de otras voces que generan distancia, duda o ironía en la producción emocional discursiva (Tannen, Portillo Fernández).  
- **Notas metodológicas**: Codificación automática y revisada. No incluye citas textuales ni referencias generales sin incorporación discursiva (ej. “se dice que”). Excluye el estilo indirecto clásico con verbos de decir o pensar.  
- **Bibliografía**: Tannen, 1989; Portillo Fernández, 2021  

---

### NEG_POLIF — Presencia de negación polifónica vinculada a la producción o expresión de la emoción  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Registra la presencia de construcciones que combinan negación con incorporación explícita de una voz ajena, modulando o distanciando emocionalmente la expresión, como en “no es cierto que dijeran…”. Esta forma particular de polifonía implica un diálogo en negación para matizar, ironizar o distanciar la emoción.  
- **Fundamento teórico**: Se fundamenta en la teoría de la polifonía discursiva, que incluye formas de negación como modos de introducir heterogeneidad y distanciamiento afectivo (Ducrot).  
- **Notas metodológicas**: Codificación automática y revisada. No se incluyen negaciones simples sin voz ajena ni heterogeneidad discursiva.  
- **Bibliografía**: Ducrot, 1986  

---

### IRONIA — Presencia de ironía  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Identifica la presencia de ironía entendida como efecto de sentido basado en la doble operación enunciativa: atribución literal a un enunciador evocado y desvalorización explícita o implícita por parte del enunciador principal, con una oposición jerarquizada entre puntos de vista que puede ser confrontativa o cómplice. La ironía debe ser claramente atribuible al experienciador de la emoción.  
- **Fundamento teórico**: Fundada en la pragmática de la ironía y su rol modulador afectivo, que genera disociaciones valorativas y reactivación de alineamientos emocionales (Berrendonner, Ducrot, Kerbrat-Orecchioni, Sperber y Wilson).  
- **Notas metodológicas**: Codificación manual o automática con revisión; requiere evidencia inequívoca de la doble operación enunciativa.  
- **Bibliografía**: Berrendonner, 1987; Ducrot, 1986; Kerbrat-Orecchioni, 2013; Reyes, 1984; Sperber y Wilson, 1992; Vitale, 2022; Colman, 2024  

---

### CT_1 — Presencia del eje modal  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Registra si en el recorte se activa el eje modal, es decir, si el acontecimiento es evaluado desde una perspectiva subjetiva o normativa. Se incluye cuando se evidencia una valoración explícita o implícita, tanto en términos afectivos (positivo/negativo) como éticos, jurídicos o ideológicos. Ejemplo: “una injusticia brutal” activa esta categoría por su carga axiológica normativa.  
- **Fundamento teórico**: Se basa en la idea de que la emoción discursiva se construye a través de valoraciones situadas y normativas, que reflejan posicionamientos éticos, ideológicos o afectivos del enunciador.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  

---

### CT_2 — Presencia del eje de clasificación, analogía o metáfora  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Se activa si el acontecimiento es relacionado discursivamente con otros hechos o conceptos por medio de clasificación (inclusión en una categoría predefinida, como “golpe de Estado”) o mediante analogías/metáforas (ej. “una bomba de tiempo”, “un nuevo 2001”). Estas operaciones ubican el acontecimiento en sistemas semánticos o narrativos más amplios.  
- **Fundamento teórico**: Fundamentado en la función de las operaciones discursivas de clasificación y metáfora para estructurar el sentido emocional y narrativo del acontecimiento.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  

---

### CT_3 — Presencia del eje de magnitud o escala  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Registra si el recorte construye discursivamente la intensidad, gravedad o alcance del acontecimiento. Se incluye si se presenta como trascendente, estructural o de gran escala (“la crisis más grave de los últimos años”), o si se cuantifica su impacto (“cientos de muertos”, “miles de desplazados”).  
- **Fundamento teórico**: Basado en la conceptualización del discurso como productor de escalas y dimensiones de intensidad emocional.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  

---

### CT_4 — Presencia del eje temporal  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Se codifica como 1 si el discurso sitúa el acontecimiento explícita o implícitamente en una temporalidad definida (pasado, presente, futuro), o si refiere a su persistencia, recurrencia o transformación en el tiempo. También se incluyen relaciones temporales entre eventos históricos (“desde la dictadura hasta hoy”).  
- **Fundamento teórico**: Considera la dimensión temporal como clave en la construcción discursiva del sentido y la emoción vinculada al acontecimiento.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  

---

### CT_5 — Presencia del eje espacial  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Se activa si el discurso localiza el acontecimiento en un espacio físico, geográfico o geopolítico, o si utiliza construcciones espaciales con carga simbólica o política (“en las villas”, “territorios en disputa”, “el sur global”). Incluye tanto menciones concretas (“en Jujuy”) como figurativas (“zonas grises del Estado”).  
- **Fundamento teórico**: La dimensión espacial como recurso semiótico para situar emocionalmente el acontecimiento.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  

---

### CT_6 — Presencia del eje distancia/proximidad  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Identifica si el recorte construye una relación de cercanía o lejanía respecto del acontecimiento en alguna de sus dimensiones: temporal, espacial o subjetiva. Por ejemplo, un enunciador que se implica explícitamente (“lo vivimos en carne propia”) o que marca distancia temporal (“algo que pasó hace siglos”) activa esta categoría.  
- **Fundamento teórico**: La construcción discursiva de distancia o proximidad como moduladora de la implicación emocional.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  

---

### CT_7 — Presencia del eje causal o de atribución agencial  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Se activa si se explicitan las causas del acontecimiento o se identifican agentes responsables, de forma directa o indirecta. Incluye representaciones causales complejas, menciones a actores concretos (“el gobierno”, “las multinacionales”) o estructuras impersonales con atribución (“fue provocado por…”).  
- **Fundamento teórico**: La atribución causal como mecanismo discursivo que orienta la emocionalidad hacia responsabilidades y explicaciones.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  

---

### CT_8 — Presencia del eje de consecuencias y efectos  
- **Tipo de variable**: Recurso  
- **Valores posibles**:  
  1: Sí  
  0: No  
- **Definición operativa**: Se registra como 1 cuando se explicitan o implican los efectos, consecuencias o afectaciones del acontecimiento. Incluye la representación de sujetos o grupos afectados (“las víctimas”), efectos amplios (“repercusiones económicas”), o la modulación de controlabilidad (“una tragedia evitable”, “algo que nadie pudo prever”).  
- **Fundamento teórico**: El eje efectual como dimensión discursiva que vincula el acontecimiento con sus impactos emocionales y sociales.  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  

---

### TIPOS_CT — Tipos de campos tópicos  
- **Tipo de variable**: Recurso  
- **Valores posibles**: [Texto libre]  
- **Definición operativa**: Agrupa los ejes de informaciones tópicas activadas en los recortes, para generar una clasificación útil para análisis posteriores. Los campos tópicos se organizan en ocho ejes que definen la emoción como posibilidad situada, en función de operaciones de categorización y relación discursiva:  
  1) Eje modal: evaluación subjetiva y normativa del acontecimiento.  
  2) Eje de determinación de relaciones externas: clasificación, analogía o metáfora.  
  3) Eje de intensidad o dimensión: gravedad, alcance o representación estructural.  
  4) Eje temporal: ubicación, persistencia o transformación temporal.  
  5) Eje espacial: localización física o simbólica.  
  6) Eje distancia/proximidad: cercanía o lejanía temporal, espacial o subjetiva.  
  7) Eje causal/agencial: causas y agentes responsables.  
  8) Eje efectual/afectacional: consecuencias y afectaciones del acontecimiento.  
- **Fundamento teórico**: Inspirado en la tópica como sistema de tratamiento de información para la construcción discursiva y emocional, reformulando a Plantin (2014) y Gutiérrez Vidrio y Plantin (2010).  
- **Notas metodológicas**: Clasificación automática, realizada por ChatGPT y revisada.  
- **Bibliografía**: Gutiérrez Vidrio y Plantin, 2010; Colman, 2025  
