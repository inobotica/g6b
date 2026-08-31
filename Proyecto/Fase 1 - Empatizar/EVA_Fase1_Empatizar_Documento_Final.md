# EVA — Enfermera Virtual de Asistencia
## Design Thinking — Fase 1: Empatizar
### Propuesta de Proyecto de Grado

---

## 1. Datos generales

**Proyecto:** EVA — Enfermera Virtual de Asistencia  
**Grupo:** Yi6  
**Asignatura:** Innovación Digital  
**Actividad:** Evaluación sumativa — Proyecto transversal grupal: Design Thinking, Fase 1 — Empatizar  
**Fecha de entrega:** 5 de agosto de 2026  
**Responsable de cargar la presentación:** Daniel Pacheco  

### Integrantes

- Alan Jairo Acosta Resendiz
- Luisa Fernanda Ramírez Caicedo
- Rafael Esteban Rojas Pinilla
- Daniel Pacheco Daza
- Felipe Villada Valderrama

---

## 2. Resumen ejecutivo

EVA — Enfermera Virtual de Asistencia — es una propuesta de sistema inteligente para apoyar el seguimiento domiciliario de la saturación de oxígeno. La solución contempla interacción por voz, recordatorios de medición, procesamiento local mediante un dispositivo embebido, generación de alertas preliminares y, en una etapa posterior, comunicación con cuidadores o prestadores de servicios de salud.

La fase Empatizar se desarrolló con un alcance académico y exploratorio. El segmento inicial priorizado corresponde a prestadores de servicios de salud domiciliaria que suministran concentradores de oxígeno y requieren mayor información sobre el uso de sus equipos y la evolución reportada de sus pacientes.

Como primera aproximación se construyó un mapa de actores y se realizó una prueba piloto de percepción con tres participantes. Los resultados muestran interés preliminar en el monitoreo domiciliario, la interacción por voz y las notificaciones automáticas. Sin embargo, el tamaño de la muestra es reducido y no permite generalizar los resultados. La entrevista con el prestador domiciliario se plantea como el siguiente paso para validar las necesidades institucionales, operativas y clínicas relacionadas con EVA.

---

## 3. Contexto de la problemática

La atención con oxígeno medicinal no termina cuando el equipo es entregado al paciente. En el entorno domiciliario pueden presentarse dificultades relacionadas con:

- el cumplimiento de las rutinas de medición;
- la interpretación de los valores de saturación;
- la comunicación con familiares, cuidadores o personal de salud;
- la identificación de situaciones que requieren atención;
- el registro histórico de las mediciones;
- y el conocimiento que posee el prestador sobre el uso real de los equipos.

En Colombia, cerca de 500.000 personas requieren oxígeno para su tratamiento médico en casa, según la Cámara de Gases Industriales y Medicinales de la ANDI. Esta cifra evidencia la relevancia del seguimiento domiciliario y la necesidad de fortalecer la seguridad, la comunicación y el acompañamiento alrededor del uso de equipos de oxígeno medicinal.

> **Nota sobre las cifras:** se excluyeron porcentajes poblacionales cuya fuente exacta y alcance no pudieron verificarse de manera suficiente para esta entrega.

---

## 4. Punto de partida

### 4.1 Pregunta orientadora

> ¿Qué dificultades, necesidades y expectativas presentan los prestadores de servicios de salud domiciliaria en relación con el uso de equipos de oxígeno y el seguimiento de la saturación de los pacientes en casa?

### 4.2 Problema inicial

Los prestadores de salud domiciliaria suministran equipos esenciales para los pacientes, pero pueden tener visibilidad limitada sobre:

- cómo se utilizan los equipos en el hogar;
- si el paciente cumple las rutinas de medición;
- cómo interpreta los resultados;
- qué ocurre antes de una llamada o solicitud de atención;
- y cuáles señales deberían generar una alerta o acompañamiento adicional.

Al mismo tiempo, los pacientes y cuidadores pueden experimentar incertidumbre al observar una medición, decidir qué acción tomar o comunicar la información a un profesional.

### 4.3 Supuestos iniciales

Antes de realizar la exploración se identificaron los siguientes supuestos:

1. Las personas pueden repetir una medición cuando el resultado parece extraño.
2. Los cuidadores pueden sentir incertidumbre al decidir si deben esperar o solicitar ayuda.
3. Los profesionales y prestadores podrían necesitar tendencias y contexto, no únicamente valores aislados.
4. Una interacción por voz podría facilitar el uso para ciertos perfiles de paciente.
5. Las alertas automáticas podrían aportar seguridad, pero también generar confusión si no son claras.
6. El prestador puede necesitar información más completa sobre el uso del equipo y las mediciones realizadas.

Estos supuestos no se consideran hechos confirmados. Su función es orientar la investigación.

---

## 5. Hipótesis de solución: EVA

EVA — Enfermera Virtual de Asistencia — se propone como una herramienta de apoyo para el seguimiento domiciliario de la saturación de oxígeno.

### 5.1 Funciones iniciales

1. **Activación por voz:** permitir una interacción sencilla con el paciente.
2. **Recordatorios de medición:** apoyar el cumplimiento de la rutina definida.
3. **Procesamiento local:** ejecutar funciones iniciales en un dispositivo embebido tipo Raspberry Pi.
4. **Modelo local de alerta temprana:** analizar inicialmente el valor de saturación de oxígeno.
5. **Orientación al usuario:** sugerir que contacte a su entidad de salud cuando se identifique una posible señal de riesgo.
6. **Alerta centralizada futura:** comunicar ciertos eventos a un cuidador, prestador o entidad de salud.
7. **Reportes de alertas:** conservar un registro de eventos relevantes para revisión posterior.

### 5.2 Límite de la propuesta

EVA no se plantea como un sistema de diagnóstico ni como sustituto de un profesional de salud. Su función sería apoyar el seguimiento, generar alertas preliminares y orientar al usuario para que busque acompañamiento profesional.

Las funciones descritas corresponden a hipótesis de solución y deberán ser validadas técnica, clínica, ética y regulatoriamente.

---

## 6. Objetivos de la fase Empatizar

### Objetivo general

Comprender de manera preliminar las necesidades, dificultades, emociones y expectativas relacionadas con el seguimiento domiciliario de la saturación de oxígeno, priorizando la perspectiva de los prestadores de servicios de salud domiciliaria.

### Objetivos específicos

- Identificar los actores relacionados con el seguimiento respiratorio en el hogar.
- Reconocer las necesidades de información del prestador domiciliario.
- Explorar la percepción inicial sobre las funciones propuestas para EVA.
- Comprender los factores que pueden generar confianza o desconfianza.
- Identificar riesgos asociados con alertas, automatización y comunicación.
- Obtener insumos para refinar la propuesta en las fases posteriores de Design Thinking.

---

## 7. Segmento inicial y actores relacionados

### 7.1 Segmento principal

El segmento inicial está compuesto por:

> **Prestadores de servicios de salud domiciliaria que suministran concentradores de oxígeno y realizan seguimiento a sus equipos y pacientes.**

El grupo cuenta con acceso a una organización con experiencia clínica y operativa en atención domiciliaria. Su nombre se mantiene reservado dentro del entregable mientras se confirma la autorización para relacionarla públicamente con la investigación.

### 7.2 Justificación del segmento

Este segmento fue priorizado porque:

- tiene contacto con pacientes que utilizan oxígeno domiciliario;
- conoce dificultades de uso y seguimiento de los equipos;
- recibe reportes, preguntas o solicitudes de los usuarios;
- puede identificar necesidades de comunicación y trazabilidad;
- posee conocimiento clínico y operativo;
- y podría utilizar reportes o alertas generados por EVA en una etapa futura.

### 7.3 Mapa de actores

| Actor | Relación con el problema | Necesidad preliminar |
|---|---|---|
| Prestador de salud domiciliaria | Suministra concentradores de oxígeno y acompaña la atención en el hogar. | Obtener información confiable sobre uso, mediciones, adherencia y alertas. |
| Paciente | Utiliza el equipo, realiza o recibe mediciones y observa los resultados. | Comprender la información y saber cuándo solicitar ayuda. |
| Cuidador | Acompaña al paciente y puede actuar ante una alerta. | Recibir información clara, oportuna y fácil de interpretar. |
| Profesional de salud | Interpreta información y orienta decisiones clínicas. | Contar con datos confiables, contextualizados y trazables. |
| Entidad de salud | Puede recibir reportes o solicitudes de atención. | Priorizar casos y establecer mecanismos de respuesta. |
| EVA | Propuesta tecnológica en exploración. | Validar qué funciones aportan valor y cuáles pueden generar riesgos. |

### Relación general entre actores

```text
                 Profesional de salud
                         │
Paciente ── Cuidador ── EVA ── Prestador domiciliario
                         │
                  Entidad de salud
```

---

## 8. Metodología

La exploración se desarrolló mediante técnicas cualitativas y descriptivas propias de la fase Empatizar.

### 8.1 Mapa de actores

Se utilizó para identificar las personas y organizaciones relacionadas con el seguimiento respiratorio domiciliario y visualizar sus relaciones.

### 8.2 Prueba piloto de percepción

Se realizó una prueba piloto exploratoria con tres participantes para conocer su percepción inicial sobre el concepto de EVA.

Los participantes tenían diferentes niveles de experiencia con dispositivos médicos. La actividad evaluó:

- importancia percibida del monitoreo en casa;
- aceptación de la interacción por voz;
- utilidad de notificar a un cuidador;
- percepción sobre el uso de inteligencia artificial;
- confianza preliminar en las alertas;
- y facilidad de uso percibida.

La prueba evaluó una **descripción conceptual** de EVA. No se probó un dispositivo funcional ni la capacidad técnica o clínica del sistema.

### 8.3 Entrevista semiestructurada al prestador

Como continuación de la fase Empatizar, se diseñó una entrevista semiestructurada para un informante clave perteneciente a un prestador de servicios de salud domiciliaria.

La entrevista se organiza en cuatro bloques:

1. Perfil y contexto.
2. Necesidades y dificultades de los usuarios.
3. Confianza, interpretación y alertas.
4. Validación inicial de EVA.

La aplicación de esta entrevista permitirá profundizar en la perspectiva institucional y operativa del segmento principal.

### 8.4 Mapa de empatía preliminar

Se construyó un mapa de empatía inicial a partir de las necesidades expresadas en la prueba piloto y de los supuestos de investigación.

El mapa debe considerarse preliminar, debido a que todavía requiere contraste con la entrevista al prestador y con una muestra más amplia de usuarios y cuidadores.

---

## 9. Consideraciones éticas y de privacidad

El grupo definió los siguientes acuerdos:

- La participación es voluntaria.
- La actividad tiene fines académicos.
- No se solicitan historias clínicas ni diagnósticos.
- No se ofrecen recomendaciones médicas.
- No se solicita modificar tratamientos.
- Se utilizan códigos o descripciones generales para proteger la identidad.
- Las citas, fotografías, capturas o grabaciones requieren autorización.
- Los participantes pueden omitir preguntas.
- No se publican datos sensibles de pacientes.
- El nombre del prestador se mantiene reservado hasta recibir autorización.
- EVA se presenta como una herramienta de apoyo, no de diagnóstico.

---

## 10. Resultados de la prueba piloto

### 10.1 Análisis descriptivo

La prueba piloto contó con tres participantes. Debido al tamaño de la muestra, los resultados se presentan mediante frecuencias y porcentajes descriptivos.

| Aspecto evaluado | Resultado |
|---|---:|
| Considera importante monitorear la saturación en casa | 3 de 3 — 100 % |
| Utilizaría un asistente de voz para recibir orientación | 3 de 3 — 100 % |
| Considera útil notificar automáticamente al cuidador | 3 de 3 — 100 % |
| Considera útil el análisis mediante inteligencia artificial | 2 de 3 — 67 % |
| Expresó confianza preliminar en el concepto de detección de una emergencia | 3 de 3 — 100 % |
| Consideró sencillo el uso descrito del dispositivo | 3 de 3 — 100 % |

### 10.2 Interpretación

Los resultados muestran una percepción inicial favorable hacia:

- el seguimiento domiciliario;
- la interacción mediante voz;
- las alertas dirigidas a cuidadores;
- y la facilidad de uso de la solución propuesta.

El resultado de 67 % sobre inteligencia artificial indica una aceptación menor frente a las demás funciones. Esto sugiere que la confianza en la IA puede depender de:

- comprender cómo se genera una alerta;
- conocer las limitaciones del modelo;
- mantener intervención humana;
- explicar qué datos utiliza;
- y permitir que un profesional revise la información.

### 10.3 Alcance de los porcentajes

Los porcentajes corresponden únicamente a una prueba piloto con tres participantes:

- 100 % equivale a 3 de 3.
- 67 % equivale a 2 de 3.

No representan a toda la población objetivo ni constituyen evidencia estadística de aceptación del mercado.

---

## 11. Resultados cualitativos

Durante la prueba piloto se identificaron cuatro temas principales.

### 11.1 Seguridad

> “Me daría tranquilidad saber que alguien será avisado si mi oxígeno baja.”

La posibilidad de notificar a un cuidador o profesional se relaciona con una sensación de acompañamiento y seguridad.

### 11.2 Facilidad de uso

> “Si solo tengo que hablarle al dispositivo, sería mucho más sencillo.”

La interacción por voz puede reducir barreras de uso, especialmente para personas que presentan dificultades con aplicaciones o interfaces complejas.

### 11.3 Atención temprana

> “Muchas veces uno no sabe cuándo realmente debe ir al hospital.”

Los participantes perciben valor en recibir una orientación preliminar que les ayude a decidir cuándo buscar apoyo profesional.

### 11.4 Confianza

> “Me gustaría que el médico pudiera revisar las mediciones.”

La confianza no depende únicamente de la automatización. También se relaciona con la posibilidad de revisión humana y con la participación de profesionales de salud.

---

## 12. Mapa de empatía preliminar

### ¿Qué piensa y siente?

- Puede sentir miedo de que su condición empeore.
- Desea sentirse acompañado y seguro en el hogar.
- Puede tener dificultad para interpretar los valores.
- Necesita confiar en que la alerta es comprensible y responsable.

### ¿Qué ve?

- Equipos médicos que pueden ser difíciles de utilizar.
- Información técnica o médica compleja.
- Familiares preocupados por su salud.
- Mediciones aisladas sin contexto histórico.

### ¿Qué oye?

- “Debes controlar tu oxigenación.”
- “Si te sientes mal, busca atención.”
- “No olvides realizar la medición.”
- Recomendaciones de familiares, cuidadores y profesionales.

### ¿Qué dice y hace?

- Se mide cuando siente algún cambio o malestar.
- Llama a un familiar cuando tiene dudas.
- Pregunta si sus valores son normales.
- Puede olvidar realizar mediciones programadas.

### Dolores o dificultades

- Incertidumbre al interpretar el resultado.
- Olvido de las mediciones.
- Interfaces complejas.
- Falta de información histórica.
- Dudas sobre cuándo intervenir.
- Desconfianza frente a decisiones totalmente automáticas.

### Beneficios esperados

- Recordatorios comprensibles.
- Interacción mediante voz.
- Alertas claras y oportunas.
- Notificación a cuidadores.
- Posibilidad de revisión por profesionales.
- Registro histórico de mediciones y alertas.

---

## 13. Hallazgos e insights preliminares

### Hallazgo 1 — La simplicidad influye en la aceptación

Los tres participantes consideraron sencillo el uso descrito y manifestaron disposición hacia la interacción por voz.

**Insight preliminar:**

> Una solución de monitoreo puede ser rechazada si exige que el paciente utilice interfaces complejas; la interacción debe adaptarse a las capacidades y al contexto del usuario.

**Implicación para EVA:**

Mantener comandos sencillos, mensajes breves y una alternativa accesible a la interacción visual.

### Hallazgo 2 — La alerta adquiere valor cuando conecta al paciente con otra persona

La notificación automática al cuidador fue valorada por los tres participantes.

**Insight preliminar:**

> El usuario no busca únicamente conocer un número; busca sentir que alguien podrá acompañarlo cuando aparezca una posible señal de riesgo.

**Implicación para EVA:**

Diseñar alertas escalonadas y definir claramente a quién se informa, en qué circunstancias y con qué datos.

### Hallazgo 3 — La confianza en la IA requiere explicación y supervisión

Dos de los tres participantes consideraron útil el análisis mediante IA, mientras que uno manifestó reservas o necesidad de mayor explicación.

**Insight preliminar:**

> La confianza no proviene de mencionar inteligencia artificial, sino de comprender sus límites, la información utilizada y la participación de profesionales.

**Implicación para EVA:**

Explicar que la clasificación es preliminar, evitar lenguaje diagnóstico y permitir revisión humana.

### Hallazgo 4 — Existe incertidumbre sobre cuándo buscar atención

Las respuestas cualitativas evidencian dudas sobre el momento apropiado para acudir a un servicio de salud.

**Insight preliminar:**

> Una alerta debe orientar sin reemplazar el juicio clínico ni generar una falsa sensación de seguridad.

**Implicación para EVA:**

Utilizar mensajes prudentes, recomendar contacto profesional y evitar instrucciones médicas automáticas.

---

## 14. Validación inicial de supuestos

| Supuesto | Resultado preliminar |
|---|---|
| La interacción por voz puede facilitar el uso. | Respaldado preliminarmente: 3 de 3 participantes la utilizarían. |
| La notificación al cuidador puede generar tranquilidad. | Respaldado preliminarmente: 3 de 3 la consideran útil y una cita relaciona la función con seguridad. |
| La inteligencia artificial será aceptada sin necesidad de explicación. | Cuestionado: solo 2 de 3 expresaron aceptación y se identificó necesidad de mayor comprensión. |
| Los usuarios requieren apoyo para decidir cuándo buscar atención. | Respaldado cualitativamente por una de las citas de la prueba piloto. |
| El prestador necesita tendencias, trazabilidad y reportes. | Pendiente de contrastar mediante entrevista al informante clave. |
| La mayoría de errores se deben a la técnica de medición. | No concluyente con la evidencia disponible. |
| Las alarmas sonoras aumentan la ansiedad. | No concluyente con la evidencia disponible. |

---

## 15. Comparación con antecedentes

La literatura sobre Design Thinking en salud resalta la importancia de comprender tanto las necesidades de pacientes como las de proveedores y profesionales antes de diseñar o implementar una solución.

En Colombia existen antecedentes de monitoreo remoto mediante Internet de las Cosas. El Ministerio TIC documentó un proyecto desarrollado por la Pontificia Universidad Javeriana y el Hospital Universitario San Ignacio para realizar seguimiento remoto de pacientes y facilitar la comunicación con cuidadores y personal de salud.

Estos antecedentes son coherentes con algunos elementos valorados en la prueba piloto:

- monitoreo domiciliario;
- comunicación con cuidadores;
- seguimiento remoto;
- facilidad de uso;
- y apoyo a la atención oportuna.

No obstante, EVA deberá demostrar posteriormente que sus funciones son seguras, comprensibles y técnicamente confiables.

---

## 16. Consideraciones regulatorias preliminares

EVA incorpora componentes que podrían relacionarse con dispositivos médicos, equipos biomédicos y software utilizado en salud.

El INVIMA establece requisitos de calidad, seguridad, clasificación de riesgo, registro y vigilancia para dispositivos médicos y equipos biomédicos. Además, el Programa Nacional de Tecnovigilancia busca identificar y gestionar eventos e incidentes asociados con estos productos.

Por lo tanto, en etapas posteriores será necesario:

- determinar la clasificación regulatoria aplicable;
- establecer si EVA o alguno de sus componentes requiere registro o permiso;
- validar la seguridad del hardware y del software;
- documentar riesgos, fallos y limitaciones;
- definir mecanismos de tecnovigilancia;
- y obtener acompañamiento de expertos clínicos y regulatorios.

---

## 17. Limitaciones

La fase desarrollada presenta las siguientes limitaciones:

1. Solo participaron tres personas en la prueba piloto.
2. La muestra no representa a toda la población objetivo.
3. Los participantes pertenecen a contextos similares.
4. No se evaluó el sistema en un entorno clínico.
5. No se utilizó un dispositivo completamente funcional.
6. Las respuestas se basaron en una explicación conceptual de EVA.
7. No se evaluó la precisión de un modelo de inteligencia artificial.
8. No se validaron umbrales clínicos de alerta.
9. La entrevista con el prestador domiciliario se encuentra pendiente.
10. El mapa de empatía es preliminar.
11. No se evaluaron todavía privacidad, seguridad de datos y responsabilidad legal de manera exhaustiva.
12. Los resultados no permiten inferencias estadísticas ni generalizaciones.

---

## 18. Conclusiones

La fase Empatizar permitió delimitar un segmento inicial y reconocer que el seguimiento domiciliario no involucra únicamente al paciente. También participan cuidadores, profesionales, entidades de salud y prestadores que requieren información confiable y oportuna.

La prueba piloto con tres participantes mostró una aceptación preliminar de las funciones de interacción por voz, recordatorios, alertas y comunicación con cuidadores. Sin embargo, también evidenció que la confianza en la inteligencia artificial necesita explicaciones claras, límites definidos y participación humana.

Los resultados no validan la efectividad clínica ni técnica de EVA. Su principal aporte consiste en identificar necesidades e hipótesis para continuar la investigación.

La propuesta parece responder a necesidades relacionadas con:

- seguridad;
- acompañamiento;
- facilidad de uso;
- seguimiento;
- atención oportuna;
- y comunicación.

El siguiente paso prioritario es entrevistar al prestador de servicios de salud domiciliaria para comprender sus necesidades de información, operación y seguimiento, y contrastar si las funciones propuestas para EVA aportan valor real.

---

## 19. Próximos pasos

1. Realizar la entrevista semiestructurada al prestador domiciliario.
2. Confirmar autorización para mencionar a la organización y utilizar citas.
3. Ajustar el mapa de empatía con evidencia del informante clave.
4. Ampliar la muestra con pacientes, cuidadores y profesionales.
5. Construir un prototipo funcional de baja fidelidad.
6. Evaluar la usabilidad de la interacción por voz.
7. Analizar el dataset preliminar y determinar su pertinencia.
8. Definir los datos mínimos necesarios para el modelo.
9. Consultar profesionales clínicos para definir criterios de seguridad.
10. Revisar requisitos regulatorios con base en INVIMA.
11. Evaluar privacidad, consentimiento y tratamiento de datos.
12. Avanzar hacia la fase Definir de Design Thinking.

---

## 20. Evidencias de la fase

Las evidencias disponibles o preparadas para la fase son:

- mapa de actores;
- mapa de empatía preliminar;
- descripción del segmento;
- instrumento de prueba piloto;
- resultados cuantitativos de tres participantes;
- citas cualitativas anonimizadas;
- análisis de hallazgos;
- matriz de validación de supuestos;
- guía de entrevista semiestructurada al prestador;
- presentación de resultados;
- y registro de limitaciones.

---

## 21. Referencias

Altman, M., Huang, T. T. K., & Breland, J. Y. (2018). *Design Thinking in Health Care*. Preventing Chronic Disease, 15, 180128. https://doi.org/10.5888/pcd15.180128

Asociación Nacional de Empresarios de Colombia — ANDI. (2023, 7 de junio). *Lanzan campaña con recomendaciones para la adquisición legal y el uso responsable de gases industriales y medicinales*. https://www.andi.com.co/Home/Noticia/17461-lanzan-campana-con-recomendaciones-para

Instituto Nacional de Vigilancia de Medicamentos y Alimentos — INVIMA. (s. f.). *Dispositivos médicos y equipos biomédicos*. https://www.invima.gov.co/productos-vigilados/dispositivos-medicos/dispositivos-medicos-equipos-biomedicos

Instituto Nacional de Vigilancia de Medicamentos y Alimentos — INVIMA. (s. f.). *Programa Nacional de Tecnovigilancia*. https://www.invima.gov.co/productos-vigilados/dispositivos-medicos/programa-nacional-de-tecnovigilancia

Ministerio de Tecnologías de la Información y las Comunicaciones — MinTIC. (2020). *Centro de Excelencia y Apropiación desarrollará proyecto basado en Internet de las Cosas para hacer seguimiento a pacientes con COVID-19*. https://www.mintic.gov.co/portal/historico/w3-article-144822.html

### Fuente de los resultados primarios

Grupo Yi6. (2026). *Prueba piloto exploratoria sobre la percepción de EVA — Enfermera Virtual de Asistencia*. Elaboración propia, tres participantes.

---

## Nota final de alcance

Este documento corresponde a un ejercicio académico de Design Thinking. Los resultados son exploratorios y no constituyen validación clínica, diagnóstico médico, aprobación regulatoria ni evidencia concluyente de aceptación de mercado.
