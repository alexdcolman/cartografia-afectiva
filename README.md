# Cartografía afectiva

Este repositorio presenta un análisis computacional de emociones en textos especializados que integra saberes de semiótica, análisis del discurso, teoría de la argumentación, retórica y lingüística textual (entre otras disciplinas dentro del amplio campo de los estudios del lenguaje), NLP y modelos de lenguaje (LLM) para modelar la emergencia, modulación y distribución emocional en discursos académicos, políticos, administrativos y culturales.

## Autoría

Este proyecto fue desarrollado por:

- **[Alex Colman](https://independent.academia.edu/AlexColman1)**

Para dudas o colaboraciones, podés contactarme vía GitHub o correo:
alexdcolman@gmail.com


## Descripción del proyecto

Este repositorio documenta un proyecto interdisciplinario que combina conocimientos expertos en semiótica, análisis del discurso, lingüística textual, teoría de la argumentación y retórica con herramientas de procesamiento de lenguaje natural (NLP) y modelos de lenguaje (LLM). El objetivo es desarrollar una metodología para analizar computacionalmente la emergencia, modulación y distribución de emociones en discursos especializados —académicos, políticos, administrativos y culturales— mediante aprendizaje automático y visualizaciones que facilitan la interpretación de los datos emocionales.

## Objetivos

- Construir una **base de datos anotada** con variables semiótico-discursivas que permitan un análisis inferencial riguroso de las emociones en textos especializados.

- Desarrollar un metalenguaje operativo para describir las emociones como procesos discursivos complejos, tomando como unidad el **simulacro emocional** —una configuración sintáctico-actancial que permite identificar y atribuir emociones a experienciadores específicos—. Este metalenguaje articula **92 variables que capturan dimensiones estructurales, semántico-pragmáticas y actanciales, incluyendo características contextuales, categorías emocionales, componentes modales, temporales, aspectuales y estésicos, así como roles actanciales**. Además, incorpora **indicadores axiológicos, estrategias argumentativas y recursos retóricos que orientan la interpretación afectiva**, lo que posibilita un análisis integral y sistemático.

- Aplicar **técnicas de análisis exploratorio** (*clustering*, análisis de componentes principales) para identificar **patrones emergentes** en los datos emocionales.

- Implementar procesos de **clasificación semiautomatizada mediante modelos de lenguaje a gran escala (LLMs)**, mediante el diseño de prompts *ad hoc* y la validación de resultados con control experto.

- Desarrollar **modelos de clasificación supervisada** para distintos problemas específicos, a partir del empleo de conjuntos de variables seleccionados según el enfoque analítico.

- Generar **visualizaciones interactivas** que faciliten la interpretación y comunicación de los hallazgos, tales como mapas emocionales, campos de emoción, perfiles de experienciadores y series temporales afectivas.

- Producir un **documento metodológico replicable** que permita a especialistas en estudios del lenguaje y el discurso incorporar el análisis computacional de emociones en sus investigaciones.

## Herramientas y tecnologías

- Python: pandas, scikit-learn, seaborn, matplotlib, openpyxl, spaCy, llama-index, transformers

- LLMs: GPT-4 API (OpenAI) para clasificación semiautomatizada y validación interpretativa

- NLP: técnicas de extracción léxica, análisis de tópicos, análisis morfosintáctico

- Dimensionalidad: PCA, clustering jerárquico, k-means

- Visualización: Plotly, Altair, matplotlib, seaborn

## Estructura del repositorio

    📁 [data/](https://github.com/alexdcolman/cartografia-afectiva/tree/data)                         ← Base anotada (anónima) y conjuntos de variables
    📁 notebooks/                    ← Notebooks exploratorios y de análisis
    📁 prompts/                      ← Lista documentada de prompts usados en clasificación
    📁 visualizations/               ← Ejemplos de salidas gráficas y dashboards
    📄 diccionario_variables.md      ← Detalle completo de todas las variables, sus códigos, valores y notas metodológicas
    📄 discusion_sintesis.md         ← Síntesis del documento "tecnologias_del_afecto.md"
    📄 marco_teorico.md              ← Fundamentación filosófico-semiológica del enfoque sobre emoción y discurso
    📄 metodologia.md                ← Descripción paso a paso del flujo metodológico, desde la anotación hasta el modelado
    📄 README.md                     ← Este archivo
    📄 tecnologias_del_afecto.md     ← Discusión crítica sobre el uso de LLMs vs. modelado experto en análisis afectivo

## Ejemplos de visualizaciones

- Mapas emocionales: distribución espacial de categorías emocionales según variables discursivas.

- Campos de emoción: configuraciones de polaridades afectivas en torno a una fuente o evento emocional.

- Perfiles de experienciadores: asociaciones entre tipo de actor y dominio emocional.

- Series temporales afectivas: progresión emocional en textos extensos.

## Clasificación semiautomatizada con LLM

Se implementa un flujo iterativo de prompts con verificación semiótica-humana para clasificar recortes discursivos según variables como:

- Modos de presencia de la emoción

- Dominancia corporal / cognitiva

- Modalidad de existencia de la emoción

- Tipo de experienciador

- Formas de figurativización y manipulación actancial

Cada fragmento es clasificado mediante uno o más prompts específicos y, si es necesario, retroalimentado para mejora de coherencia interna.

## Documentos adicionales

- metodologia.md: Descripción paso a paso del proceso metodológico.

- diccionario_variables.md: Diccionario completo de variables con notas metodológicas detalladas.

- marco_teorico.md: Fundamento teórico del enfoque, con eje en la filosofía simondoniana y su articulación con la semiótica, la lingüística y el análisis del discurso.

- modelo_vs_IA.md: Ensayo sobre los límites del análisis escalable automatizado y la necesidad de marcos expertos en la definición de variables.

## Licencia

Este proyecto se publica bajo la licencia GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007. Podés reutilizar y modificar el código citando adecuadamente.

## Agradecimientos

Agradezco especialmente a [Mathi Gatti](https://mathigatti.com/) por las valiosas conversaciones que venimos compartiendo sobre el vínculo entre LLMs y conocimiento experto, y por las ideas que surgieron en relación con el análisis emocional de textos infantiles, en el contexto de un proyecto conjunto en desarrollo.

También, a [María Alejandra Vitale](https://uba.academia.edu/AlejandraVitale) por sus orientaciones críticas y su generosidad intelectual, que fueron clave en la elaboración de este trabajo.
