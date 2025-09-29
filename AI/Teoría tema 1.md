Información sacada del PDF [[TEMA_1_FUNDAMENTOS IA_DAW.pdf]]

**📖 Página 1 – Definición de IA y sistemas de IA**

**🔹 1. Definición de Inteligencia Artificial**

- La **IA** es una **disciplina de la informática y la ingeniería**.
- Su objetivo es **diseñar y construir sistemas** capaces de **emular e incluso superar funciones cognitivas humanas**.
- Integra:
    - **Métodos simbólicos** → lógica, reglas, conocimiento explícito.
    - **Algoritmos de optimización** → buscan la mejor solución a un problema.
    - **Modelos de aprendizaje automático (ML)** → aprenden patrones a partir de datos.
    - **Técnicas híbridas** → combinan enfoques.
- Ámbitos de aplicación: **percepción, razonamiento, planificación, toma de decisiones, interacción y adaptación autónoma** en entornos dinámicos.

---

**🔹 1.1 ¿Qué entendemos por sistemas de IA?**

Un sistema de IA está formado por **módulos especializados** que trabajan juntos para transformar **datos en decisiones automatizadas**.

**Los 10 módulos principales:**

1. **Datos**📊
    - Fuente de información que alimenta el sistema.
    - Tipos:
        - **Estructurados** → tablas, bases de datos.
        - **No estructurados** → texto, imágenes, vídeos.
        - **Semiestructurados** → JSON, XML.
    - Se dividen en **entrenamiento**, **validación** y **prueba**.
2. **Modelo**🧠
    - Es el “cerebro” del sistema.
    - Representación matemática que **aprende patrones** y genera predicciones.
	    -Nota: incluso los modelos más sofisticados no razonan; simplemente generan predicciones a partir de patrones aprendidos, cuya complejidad puede llegar a simular procesos de pensamiento.
    - Puede basarse en: **redes neuronales, árboles de decisión, métodos estadísticos/probabilísticos**.
    - En redes neuronales: se organizan en **capas de neuronas artificiales** que ajustan sus pesos para aproximar funciones complejas.
3. **Algoritmo de entrenamiento** ⚙️
    - Método que permite al modelo aprender.
    - Ajusta parámetros internos para **minimizar el error**.
    - Ejemplos: **gradiente descendente, backpropagation, optimizadores (Adam, RMSprop, etc.)**.
4. **Entrenamiento**🔁
    - Proceso iterativo donde el modelo aprende a partir de los datos.
    - Se realiza en ciclos llamados **épocas**.
    - En cada época se calcula el error y se ajustan los parámetros.
5. **Evaluación**📏
    - Verifica si el modelo ha aprendido correctamente.
    - Se usan datos que **nunca ha visto antes**.
    - Métricas habituales: **precisión, recall, F1-score, MAE, RMSE**.
    - Clave: **sin evaluación rigurosa, no hay calidad ni mejora posible**.
6. **Despliegue**🚀
    - El modelo entrenado se pone en producción.
    - Se convierte en un **servicio accesible** desde aplicaciones.
    - Métodos: **APIs, contenedores (Docker), integración en sistemas existentes**.
7. **Interfaz**🖥️
    - Canal de interacción con el usuario.
    - Ejemplos: **apps, webs, chatbots, APIs**.
8. **Infraestructura**🏗️
    - Recursos que soportan el sistema.
    - Incluye: **CPU, GPU, almacenamiento, redes, servicios en la nube**.
9. **Monitorización**👀
    - Se supervisa el rendimiento del modelo en producción.
    - Permite detectar: **errores, degradación, necesidad de reentrenamiento**.
10. **Seguridad, privacidad y ética** 🔒

- Se aplican medidas para proteger los datos y garantizar **decisiones responsables**.
- Ejemplos: **control de accesos, anonimización, detección de sesgos, cumplimiento normativo**.

---

📌 **Idea clave de la página 1:**  
Un sistema de IA no es solo un modelo entrenado, sino una **combinación de módulos interdependientes** (datos, entrenamiento, despliegue, monitorización, seguridad…).  
La **evaluación rigurosa** y la **ética** son fundamentales para garantizar calidad, fiabilidad y responsabilidad.

---

**📖 Página 2 – Analogía teatral de los módulos de IA**

El texto propone entender los **módulos de un sistema de IA** comparándolos con los **elementos de una obra de teatro** 🎭. Esto ayuda a visualizar cómo cada parte cumple un rol específico, pero todas deben trabajar en conjunto.

---

**🎭 Analogía teatral de los módulos**

- **Datos → El guion** 📜  
    Los datos son el guion que los actores deben aprender para representar bien la obra.
- **Modelo → El actor principal** 🎭  
    El modelo es quien interpreta el guion. Debe comprenderlo y actuar correctamente.
- **Algoritmo de entrenamiento → El director** 🎬  
    El director guía al actor, corrigiendo y mejorando su actuación.
- **Entrenamiento → Los ensayos** 🔁  
    El actor repite la obra muchas veces hasta perfeccionarla.
- **Evaluación → El estreno privado** 👥  
    Antes del estreno oficial, se prueba la obra con un público reducido para comprobar si funciona bien.
- **Despliegue → El estreno oficial** 🌍  
    Ahora la obra se presenta ante el público general, es decir, el modelo se usa en el mundo real.
- **Interfaz → Escenario y decorado** 🎨  
    Es lo que ve el público y la forma en la que interactúa con la obra.
- **Infraestructura → El teatro** 🏛️  
    Incluye el edificio, las luces, el sonido… sin infraestructura no hay función.
- **Monitorización → El equipo técnico** 🔧  
    Vigila que todo funcione bien durante la representación.
- **Seguridad, privacidad y ética → Las normas del teatro** ⚖️  
    Son las reglas de acceso, respeto al público, seguridad y ética profesional.

---

**📌 Reflexión final de la página**

- La **IA moderna es un sistema complejo** que combina muchas disciplinas:
    - Ingeniería de datos
    - Diseño de interfaces
    - Arquitectura de software
    - Ética computacional
- **No basta con entrenar un modelo**: hay que entender cómo se integra en la vida real, cómo afecta a las personas y qué consecuencias puede tener.
- Los sistemas de IA **no solo calculan**, también **toman decisiones, interactúan con usuarios e influyen en su entorno**.
- Por eso, el diseño y supervisión de la IA requieren una **visión crítica, ética y global**.

---

📌 **Idea clave de la página 2:**  
Un sistema de IA se entiende mejor si se ve como una **obra de teatro**, donde cada módulo tiene un rol. La colaboración de todos es necesaria para que funcione. Pero además, la IA no se limita a la técnica: hay que considerar su **impacto real, social y ético**.

---

**📖 Página 3 – Aprendizaje y razonamiento en IA**

**🔹 ¿Qué significa que la IA “aprende”? 🤖📚**

- En IA, **aprender no es comprender**, sino **ajustar parámetros internos** para mejorar en una tarea concreta.
- Proceso:
    1. El modelo recibe **ejemplos con sus respuestas correctas**.
    2. Compara su salida con la respuesta real.
    3. Calcula el **error**.
    4. Ajusta sus parámetros para mejorar en la siguiente iteración.
    5. Este ciclo se repite miles de veces durante el **entrenamiento**.
- Se basa en **algoritmos de optimización** que reducen la diferencia entre lo que el modelo predice y lo que debería predecir.
- Ejemplo: **descenso del gradiente**.

👉 Clave: El aprendizaje en IA es **automático**, pero **estadístico**, no implica verdadera comprensión.

---

**🔹 ¿Qué significa que la IA “razona”? 🧠⚙️**

- Razonar en IA es **simular procesos estructurados de pensamiento** como:
    - Descomponer problemas en pasos lógicos.
    - Inferir consecuencias.
    - Planificar acciones.
    - Mantener coherencia contextual en varias interacciones.
- El razonamiento de la IA:
    - **No es consciente ni reflexivo**.
    - Es una **simulación estadística basada en patrones aprendidos**.
    - Aunque parezca que “piensa”, en realidad es una **imitación matemática del razonamiento humano**.

---

**📌 Características del aprendizaje**

- Es **automático**, basado en datos de entrenamiento.
- Usa **algoritmos matemáticos** como descenso del gradiente.
- No implica **comprensión real**, sino detección de patrones.

---

**📌 Formas de razonamiento en IA moderna**

- **Descomposición de tareas** en pasos lógicos.
- Uso de **herramientas externas** (calculadoras, buscadores, bases de datos).
- **Memoria contextual** para mantener coherencia en varias interacciones (ejemplo: ChatGPT recordando lo dicho antes en la conversación).

---

**📝 Reflexión de cierre**

- Aprender en IA no es **comprender**.
- Razonar en IA no es **pensar**.
- Ambos procesos son **simulaciones estadísticas** que permiten realizar tareas complejas, pero **sin conciencia, intención ni juicio humano**.
- Es fundamental **no confundir capacidad técnica con inteligencia real** para evitar sobrevalorar lo que hace una IA.

---

📌 **Idea clave de la página 3:**  
La IA **aprende ajustando parámetros** y **razona simulando procesos lógicos**, pero sin verdadera comprensión ni pensamiento. Esto permite ejecutar tareas complejas, aunque siempre bajo límites estadísticos y computacionales.

---

**📖 Página 4 – Evolución histórica de la IA**

**🔹 Origen del término**

- El término **“Inteligencia Artificial”** fue acuñado en **1956** por **John McCarthy** en la **Conferencia de Dartmouth**.
- Desde entonces, la IA ha pasado por ciclos de **entusiasmo (veranos de la IA)** y **escepticismo (inviernos de la IA)**.

---

**🔹 Hitos clave en la evolución de la IA (1943 – 1970)**

1. **1943 – Neurona McCulloch-Pitts** 🧠
    - Primer modelo matemático de una neurona artificial.
2. **1950 – Prueba de Turing** 🖥️
    - Alan Turing propone un test para evaluar si una máquina muestra comportamiento inteligente.
3. **1956 – Nacimiento del término “IA”** 🤖
    - John McCarthy formaliza el concepto en Dartmouth.
4. **1958 – Perceptrón (Rosenblatt)** 🔗
    - Primer modelo de red neuronal entrenable.
5. **1967 – Algoritmo K-NN (K-Nearest Neighbors)** 📊
    - Algoritmo de clasificación basado en la proximidad de datos.
6. **1970 – Stanford Cart** 🚗
    - Primer robot móvil capaz de **navegar de manera autónoma**.

---

**📌 Reflexión de la página**

- La IA desde el inicio se ha inspirado en el **funcionamiento humano (neuronas, razonamiento, aprendizaje)**.
- Estos hitos marcaron la base de lo que hoy son los algoritmos modernos.
- La historia muestra que la IA **avanza en oleadas**, con fases de gran progreso y momentos de freno.

---

📌 **Idea clave de la página 4:**  
La IA nace en los años 50 con la inspiración de la mente humana y evoluciona gracias a modelos matemáticos, pruebas de inteligencia y los primeros robots autónomos. Es una disciplina que avanza entre fases de optimismo y crisis.

---

**📖 Página 5 – Evolución histórica (segunda parte)**

**🔹 Hitos clave (1976 – 2025)**

1. **1976 – ELIZA** 💬
    - Primer **chatbot** que simulaba una conversación con un terapeuta.
2. **1986 – Retropropagación** 🔁
    - Se populariza el **entrenamiento de redes neuronales profundas** gracias al algoritmo de **backpropagation**.
3. **1997 – Deep Blue vence a Kasparov** ♟️
    - IBM crea un sistema que derrota al campeón mundial de ajedrez, Garry Kasparov.
4. **2011 – Watson gana en Jeopardy!** 🧾
    - IBM demuestra **comprensión de lenguaje natural** en una competencia televisiva.
5. **2015 – Baidu usa CNNs** 📷
    - Redes neuronales convolucionales (CNNs) logran una **precisión superior a los humanos** en clasificación de imágenes.
6. **2016 – AlphaGo vence a Lee Sedol** ⚪
    - DeepMind conquista el juego **Go**, considerado más complejo que el ajedrez.
7. **2020 – GPT-3 y AlphaFold** 🤯
    - **GPT-3 (OpenAI):** revoluciona el lenguaje natural con modelos de gran escala.
    - **AlphaFold (DeepMind):** predice estructuras de proteínas con gran precisión.
8. **2021 – DALL·E y Copilot** 🎨💻
    - **DALL·E:** genera imágenes a partir de texto.
    - **GitHub Copilot:** ayuda a programar con sugerencias automáticas de código.
9. **2022 – ChatGPT y Stable Diffusion** 🗨️🖼️
    - Estalla la IA generativa en texto e imagen.
10. **2023 – GPT-4 y Bard** 🌐
    - Llegan los **modelos multimodales** capaces de combinar texto, imágenes y razonamiento avanzado.
11. **2024 – LRM (Large Reasoning Models)** 🧠
    - Surgen modelos diseñados para **razonamiento multietapa y planificación lógica**.
12. **2025 – IA generativa hiperrealista** 🎬
    - Se crean películas completas a partir de prompts con narrativas coherentes.

---

**📌 Reflexión final de la evolución**

- Cada avance amplió el **alcance de la IA** y transformó sectores enteros: medicina, entretenimiento, educación, industria.
- La IA pasó de experimentos básicos a **herramientas capaces de generar contenido, razonar y colaborar con humanos**.
- Hoy estamos en la etapa de la **IA generativa y multimodal**, con gran potencial pero también desafíos éticos y sociales.

---

📌 **Idea clave de la página 5:**  
La historia de la IA muestra un progreso constante hacia sistemas más autónomos, creativos y capaces de razonar. Desde **chatbots simples** hasta **modelos multimodales y generativos actuales**, la IA redefine la relación entre humanos y máquinas.

---

**📖 Página 6 – Clasificación de la IA**

La IA se puede clasificar de distintas formas. En el documento se destacan **tres criterios prácticos**:

---

**🔹 1. Por nivel de capacidad o inteligencia 🧠**

- **IA Débil o Estrecha (ANI – Artificial Narrow Intelligence)**
    - Diseñada para realizar **tareas específicas**.
    - No tiene conciencia ni comprensión general.
    - Ejemplo: **asistentes virtuales** como Siri, Alexa, Google Assistant.
- **IA General (AGI – Artificial General Intelligence)**
    - En teoría, podría **aprender y adaptarse a cualquier tarea** como un ser humano.
    - Aún está en investigación, no existe de forma real.

---

**🔹 2. Por arquitectura o enfoque ⚙️**

- **IA Simbólica**
    - Basada en **reglas, lógica y conocimiento explícito**.
    - Ejemplo: sistemas expertos de los años 80.
- **IA Conexionista**
    - Basada en **redes neuronales y aprendizaje estadístico**.
    - Ejemplo: redes profundas (Deep Learning).
- **IA Híbrida**
    - Combina lo mejor de la simbólica y la conexionista.
    - Busca mayor precisión, capacidad de razonamiento y flexibilidad.

---

**🔹 3. Por tarea o aplicación 📲**

Clasifica la IA según el **uso específico**:

- **IA Conversacional** 💬
    - Ej.: chatbots, asistentes de voz.
- **IA Predictiva** 📊
    - Ej.: modelos de riesgo financiero, predicción de ventas, mantenimiento predictivo.
- **IA Generativa** 🎨📝
    - Ej.: generación de texto, imágenes, música, programación asistida.
- **IA Autónoma** 🚗🤖
    - Ej.: robots industriales, vehículos sin conductor, drones inteligentes.

---

**📌 Reflexión de la clasificación**

- Cada clasificación responde a una **perspectiva distinta** (capacidad, arquitectura, aplicación).
- En la práctica, muchos sistemas actuales combinan varias categorías:
    - Por ejemplo, **ChatGPT** es **conversacional + generativo**, basado en **IA conexionista (redes neuronales)**, y todavía dentro de la **IA débil**.

---

📌 **Idea clave de la página 6:**  
La IA puede clasificarse según su **nivel de capacidad (ANI vs AGI)**, su **arquitectura (simbólica, conexionista, híbrida)** o su **aplicación (conversacional, predictiva, generativa, autónoma)**. Esta clasificación ayuda a entender sus usos y limitaciones actuales.

---

**📖 Página 7 – Ramas de la IA**

La mente humana hace muchas cosas (hablar, ver, aprender, razonar, moverse, decidir).  
Por eso, la IA no se resuelve con un solo enfoque, sino con **subdisciplinas especializadas**.

---

**🔹 Aprendizaje Automático (Machine Learning – ML) 📊**

- Permite que los sistemas **aprendan a partir de datos** sin estar programados explícitamente para cada tarea.
- Tipos principales:
    - **Supervisado** → se entrena con ejemplos etiquetados.
    - **No supervisado** → busca patrones en datos sin etiquetas.
    - **Por refuerzo** → aprende con recompensas/castigos por sus acciones.
    - **Semisupervisado / autosupervisado** → combinan ambos enfoques.

👉 En los **modelos avanzados (LLMs)** aparecen fenómenos como:

- **Representación implícita**: los modelos codifican conocimiento internamente en vectores.
- **Razonamiento emergente**: capacidades complejas que surgen espontáneamente en modelos grandes.

---

**🔹 Aprendizaje Profundo (Deep Learning – DL) 🧠**

- Subcategoría del ML.
- Utiliza **redes neuronales con múltiples capas**.
- Muy eficaz en:
    - Reconocimiento de voz.
    - Visión por computadora.
    - Generación de texto.
- Los **transformers** han revolucionado el procesamiento de lenguaje y la creación de contenido.

---

**🔹 Procesamiento del Lenguaje Natural (PLN) 💬**

- Se centra en la **interacción entre máquinas y lenguaje humano**.
- Tareas:
    - Comprensión de texto.
    - Generación automática de lenguaje.
    - Traducción automática.
    - Sistemas conversacionales (chatbots).

---

**🔹 Visión por Computadora 👁️**

- Permite que los sistemas **interpreten imágenes y vídeos**.
- Aplicaciones:
    - Reconocimiento de objetos y rostros.
    - Segmentación de escenas.
    - Reconstrucción 3D.

---

**🔹 Robótica 🤖**

- Combina **percepción sensorial + planificación + control de movimiento**.
- Permite que los robots interactúen físicamente con su entorno.
- Usa: sensores, algoritmos de decisión y mecanismos de acción en **tiempo real**.

---

**🔹 Interacción Humano–IA y Ética ⚖️**

- Se enfoca en cómo los sistemas inteligentes se relacionan con las personas.
- Incluye:
    - Interfaces adaptativas.
    - Explicabilidad de modelos.
    - Reconocimiento de emociones.
    - Seguridad, privacidad y gobernanza de la IA.

---

**📌 Reflexión final de la página**

- Estas ramas **no funcionan de forma aislada**.
- La verdadera inteligencia emerge de la **combinación de todas**.
- Ejemplo: un asistente virtual necesita PLN + ML/DL + razonamiento implícito + interacción humano-IA + visión/robótica.
- En IA, como en la mente humana: **todo está conectado**.

---

📌 **Idea clave de la página 7:**  
La IA se organiza en ramas como **ML, DL, PLN, visión por computadora, robótica y ética**. Cada una resuelve un aspecto distinto de la inteligencia, pero la verdadera potencia surge cuando se **integran entre sí**.

---

**📖 Página 8 – Modelos de IA con Deep Learning (LLM y LRM)**

**🔹 Recordatorio**

- El **modelo** es el “cerebro” de la IA.
- Su **estructura y capacidad** dependen de la disciplina utilizada (redes neuronales, árboles de decisión, etc.).
- Con el **aprendizaje profundo (DL)** se diseñan **modelos más avanzados**, como los **LLM** y **LRM**, con capacidades cognitivas sofisticadas.

---

**🔹 5.1 ¿Qué son los LLM? (Large Language Models) 📚🤖**

- Son modelos entrenados con **enormes cantidades de texto**.
- Objetivo: generar **lenguaje fluido y coherente**.
- Características:
    - Basados en **arquitectura Transformer** (procesa secuencias con atención contextual).
    - Aprenden prediciendo el **siguiente token/palabra** dado un contexto.
    - Ejemplos: **GPT, BERT, Claude, PaLM, LLaMA**.
- Relación con ML/DL:
    - Usan **aprendizaje profundo supervisado** y datasets masivos.
    - Funcionan con **representación implícita** (no entienden el lenguaje, pero lo codifican en vectores).
    - Exhiben **razonamiento emergente**: realizan tareas complejas (traducción, resumen, programación) sin entrenamiento específico.

---

**🔹 5.2 ¿Qué son los LRM? (Large Reasoning Models) 🧠**

- Evolución de los LLM, pensados no solo para generar lenguaje, sino para **razonar, planificar y resolver problemas complejos**.
- Incorporan:
    - **Descomposición de problemas** en pasos lógicos.
    - **Acceso a herramientas externas** (calculadoras, bases de datos, buscadores).
    - **Verificación de resultados** y consistencia lógica.
- Relación con ML/DL:
    - También usan **aprendizaje profundo**, pero añaden **razonamiento simbólico o semisimbolico**.
    - Combinan DL con técnicas clásicas de IA (planificación lógica, búsqueda, etc.).
    - Más fiables en tareas críticas que requieren **precisión y lógica multietapa**.
- Ejemplos de aplicación: diagnóstico médico, planificación estratégica, resolución de problemas complejos.

---

**🔹 5.3 ¿Cómo interactúan los LLM y LRM? 🔗**

- **LLM como base, LRM como extensión**
    - Muchos LRM se construyen encima de arquitecturas de LLM y luego se ajustan para razonamiento complejo.
- **Sistemas híbridos**
    - Algunos modelos actuales (ej. GPT-4 con herramientas, Claude con cadenas de pensamiento) ya mezclan generación + razonamiento.
- **Separación modular**
    - Se puede usar un LLM para generar texto y un LRM para validar/corregir/razonar sobre la salida.

---

**📌 Conclusión de la página**

- **LLM** → dominan el lenguaje y muestran razonamiento emergente como efecto secundario.
- **LRM** → buscan razonar de forma explícita y estructurada.
- Ambos dependen de ML/DL, pero los **LRM representan un paso hacia una IA más lógica, confiable y aplicable en tareas críticas**.

---

📌 **Idea clave de la página 8:**  
Los **LLM** son expertos en lenguaje, mientras que los **LRM** están diseñados para razonar de forma estructurada. Juntos marcan la evolución de la IA moderna hacia sistemas más útiles, lógicos y confiables.

---

**📖 Página 9 – Desafíos éticos de la IA**

La IA plantea **riesgos sociales, legales y éticos** que deben afrontarse para un desarrollo responsable.

---

**🔹 1. Sesgos algorítmicos ⚖️**

- Los algoritmos aprenden de **datos históricos**, que pueden contener prejuicios.
- Esto perpetúa **discriminación** en ámbitos como:
    - Justicia.
    - Salud.
    - Contratación laboral.

---

**🔹 2. Privacidad y protección de datos 🔒**

- La IA procesa grandes volúmenes de **información personal**.
- Problemas:
    - Uso de datos sin consentimiento.
    - Vigilancia encubierta.
    - Riesgo de filtraciones.

---

**🔹 3. Responsabilidad y transparencia 👤**

- Pregunta clave: **¿quién responde si la IA comete un error grave?**
- Falta de claridad en cómo se toman decisiones.
- Dificulta la **rendición de cuentas** en sectores críticos.

---

**🔹 4. Manipulación emocional y social 🧠**

- La IA puede influir en:
    - Opiniones políticas.
    - Decisiones de consumo.
    - Estado emocional de las personas.
- Riesgo: pérdida de autonomía individual y amenaza a la democracia.

---

**🔹 5. Impacto en el empleo 👷‍♂️**

- Automatización puede **reemplazar trabajos**.
- Genera **desigualdad y desempleo** en ciertos sectores.
- También redefine el rol de profesionales en áreas como medicina, educación o derecho.

---

**🔹 6. Falta de regulación 📜**

- El desarrollo tecnológico va más rápido que las leyes.
- Necesidad de **normas claras** que:
    - Protejan a los ciudadanos.
    - No frenen la innovación.

---

**📌 Reflexión final de la página**

- La IA no es solo una tecnología, sino una **herramienta con impacto profundo en la sociedad**.
- Si no se controla, puede **amplificar desigualdades y generar riesgos éticos graves**.
- La regulación y la supervisión son **imprescindibles**.

---

📌 **Idea clave de la página 9:**  
Los principales problemas éticos de la IA son los **sesgos, la privacidad, la responsabilidad, la manipulación social, el impacto en el empleo y la falta de regulación**. Afrontarlos es clave para un uso justo y seguro de esta tecnología.

---

**📖 Página 10 – Regulación ética de la IA en Europa**

**🔹 6.1 Regulación ética en Europa: AI Act 🇪🇺**

- Europa ha aprobado la **AI Act**, la primera normativa integral sobre IA en el mundo.
- Clasifica los sistemas de IA en **cuatro niveles de riesgo**:

|**Nivel de riesgo**|**Ejemplos**|**Regulación aplicada**|
|---|---|---|
|**Inaceptable** ❌|Manipulación psicológica, vigilancia biométrica|**Prohibidos** completamente|
|**Alto riesgo** ⚠️|Selección de personal, justicia, salud|Supervisión estricta + auditorías obligatorias|
|**Riesgo limitado** ℹ️|Chatbots, asistentes virtuales|Transparencia: el usuario debe saber que habla con una IA|
|**Bajo riesgo** ✅|Videojuegos, filtros de spam|Sin regulación específica|

- Además: los contenidos generados por IA (textos, imágenes, vídeos) deben estar **etiquetados claramente** para evitar confusión.

---

**📖 Página 11 – Propuestas éticas complementarias**

**🔹 6.2 Medidas adicionales en Europa**

1. **Gobernanza ética como ventaja competitiva**
    - Muchas empresas europeas adoptan:
        - **Comités internos de IA responsable**.
        - Figuras como el **Data & AI Ethics Officer**.
        - **Canales de denuncia** para reportar incidentes éticos.
    - Beneficio: genera **confianza** y refuerza la **posición en el mercado**.
2. **Protección de creatividad y derechos de autor** 🎨📚
    - Problema: muchas IA se entrenan con **obras protegidas sin permiso**.
    - Esto afecta a **creadores, artistas y escritores**.
    - Propuestas:
        - Transparencia en el uso de datos culturales.
        - Definición legal de qué es una “obra generada por IA”.
        - Mecanismos de protección para la **autoría humana**.

---

**📖 Página 12 – En la actualidad**

**🔹 6.3 Situación actual en Europa**

- Europa busca una **IA ética, humana y sostenible**.
- Sin embargo, enfrenta críticas:
    - Regulación demasiado rápida.
    - Riesgos para startups y sectores creativos.
- Desafío: equilibrar **innovación y seguridad**.

---

**📌 Reflexión final de estas páginas**

- Europa se posiciona como **líder mundial en regulación ética de IA**.
- El reto es no frenar la innovación mientras se **protege a los ciudadanos y creadores**.
- La clave está en una **IA responsable**, transparente y centrada en el ser humano.