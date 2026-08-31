# EVA — Enfermera Virtual de Asistencia
## Plan de trabajo — Design Thinking, Fase 1: Empatizar
### Propuesta de Proyecto de Grado

> **Estado del documento:** borrador para revisión del equipo.  
> **Enfoque de esta entrega:** planeación y preparación de la fase Empatizar.  
> **Fecha límite:** 5 de agosto de 2026, 11:59 p. m. — hora Colombia.

---

## 1. Datos generales

**Proyecto:** EVA — Enfermera Virtual de Asistencia  
**Grupo:** G6: Yi6  
**Asignatura:** Innovación Digital  
**Actividad:** Evaluación sumativa — Proyecto transversal grupal: Design Thinking, Fase 1 — Empatizar  
**Responsable de cargar la presentación:** Daniel Pacheco  

**Integrantes:**

- Alan Jairo Acosta Resendiz
- Luisa Fernanda Ramírez Caicedo
- Rafael Esteban Rojas Pinilla
- Daniel Pacheco Daza
- Felipe Villada Valderrama

---

## 2. Propósito de la entrega

Esta entrega documenta la planeación de la Fase 1 — Empatizar para el proyecto EVA.

Debido al tiempo disponible y a que la actividad fue asignada antes de desarrollar formalmente la primera clase de la asignatura, el grupo se concentra en:

- delimitar el segmento inicial de exploración;
- identificar los actores relacionados con la problemática;
- seleccionar técnicas de empatía apropiadas para el alcance académico;
- preparar una entrevista semiestructurada a un informante clave;
- establecer el formato para documentar evidencias y resultados posteriores;
- definir cómo se analizarán los hallazgos;
- y preparar una guía de presentación breve, clara y visual.

En esta versión no se presentan entrevistas ni hallazgos como si ya hubieran sido obtenidos. Los resultados se incorporarán cuando la técnica sea aplicada.

---

## 3. Alcance académico

Este trabajo es exploratorio y educativo. No pretende:

- diagnosticar hipoxemia;
- reemplazar la valoración de un profesional de salud;
- validar clínicamente un dispositivo;
- demostrar que EVA ya funciona;
- presentar funciones tecnológicas como necesidades confirmadas;
- ni generalizar resultados a todo el mercado.

Sí pretende:

- comprender inicialmente el contexto de los proveedores de oxímetros;
- reconocer necesidades, preocupaciones y dificultades frecuentes;
- identificar actores relacionados con el monitoreo domiciliario;
- preparar una primera recolección cualitativa de información;
- y obtener insumos para refinar el proyecto en entregas posteriores.

> **Acuerdo metodológico:** EVA es una hipótesis de solución que debe ser contrastada con actores reales.

---

## 4. Problemática inicial

El monitoreo de la saturación de oxígeno en el hogar puede presentar dificultades relacionadas con:

- la constancia para realizar mediciones;
- el uso correcto del oxímetro;
- la interpretación de los resultados;
- la reacción ante posibles señales de riesgo;
- la comunicación con cuidadores o entidades de salud;
- y la ausencia de un seguimiento histórico organizado.

Estas dificultades todavía se consideran hipótesis iniciales y deberán ser exploradas mediante la entrevista propuesta.

### Pregunta orientadora

> ¿Qué dificultades, necesidades y expectativas observan los proveedores de oxímetros y soluciones de monitoreo respiratorio domiciliario en relación con el uso de estos dispositivos por parte de pacientes y cuidadores?

---

## 5. Hipótesis de solución: EVA

EVA — Enfermera Virtual de Asistencia — es una propuesta de sistema inteligente para apoyar el seguimiento domiciliario de la saturación de oxígeno.

### Funciones iniciales planteadas

1. **Activación por voz**, para facilitar la interacción con el paciente.
2. **Recordatorios de medición**, para apoyar el cumplimiento de la rutina.
3. **Procesamiento local**, mediante un dispositivo embebido tipo Raspberry Pi.
4. **Modelo local de alerta temprana**, basado inicialmente en el valor de saturación de oxígeno.
5. **Orientación al usuario**, sugiriendo contactar a su entidad de salud cuando se identifique una posible señal de riesgo.
6. **Alerta centralizada futura**, que podría ser enviada a un proveedor o entidad de salud desde un servidor.
7. **Reportes de alertas**, para consultar eventos registrados durante el seguimiento.

### Límite de la propuesta

EVA no se plantea como un sistema de diagnóstico ni como sustituto de un profesional. Su función sería generar una alerta preliminar y orientar al usuario para que busque apoyo profesional.

---

## 6. Segmento inicial de exploración

### Segmento seleccionado

> Prestadores de servicios de salud domiciliaria que suministran concentradores de oxígeno y realizan seguimiento al uso de sus equipos y a las condiciones de sus pacientes.

### Organización identificada

El grupo cuenta con un contacto en **Oxiayuda**, una empresa prestadora de servicios de salud domiciliaria con 23 años de experiencia en el sector. La organización suministra principalmente concentradores de oxígeno para uso en el hogar y busca obtener mayor información sobre el uso de sus equipos y sobre las condiciones de los pacientes atendidos.

> **Uso del nombre:** la mención pública de Oxiayuda está pendiente de autorización. Mientras no exista consentimiento explícito, en la presentación y en las evidencias se utilizará la descripción “prestador de servicios de salud domiciliaria” o el código **E01**.

### Justificación

Este segmento fue seleccionado porque:

- tiene contacto directo con pacientes que utilizan oxígeno domiciliario;
- conoce dificultades relacionadas con el uso de los equipos en el hogar;
- posee experiencia clínica y operativa;
- puede identificar necesidades de seguimiento, comunicación y reporte;
- tiene interés en obtener información más completa sobre el uso de sus dispositivos y sobre los pacientes;
- y el grupo cuenta con acceso real a un informante clave dentro de la organización.

Esta selección es provisional. En fases posteriores se recomienda ampliar la investigación a pacientes, cuidadores, profesionales de salud y otras entidades prestadoras.

---

## 7. Mapa preliminar de actores

| Actor | Relación con la problemática | Necesidad preliminar por explorar |
|---|---|---|
| Prestador de salud domiciliaria | Suministra concentradores de oxígeno, acompaña a pacientes en el hogar y busca conocer mejor el uso de sus equipos. | Obtener información confiable sobre uso, adherencia, alertas y condiciones del paciente. |
| Paciente | Realiza o recibe la medición y observa el resultado. | Recordar la medición, comprender el dato y saber cuándo solicitar ayuda. |
| Cuidador | Acompaña al paciente y puede tomar decisiones ante una alerta. | Información clara, oportuna y fácil de comunicar. |
| Profesional de salud | Interpreta información y orienta decisiones clínicas. | Datos confiables, contextualizados y con trazabilidad. |
| Entidad o proveedor de salud | Podría recibir alertas o reportes centralizados. | Información priorizada y mecanismos de atención definidos. |
| EVA | Propuesta tecnológica en exploración. | Validar qué funciones aportan valor y cuáles podrían generar riesgos o confusión. |

> Este mapa es preliminar y deberá ajustarse después de la entrevista.

---

## 8. Técnicas de la fase Empatizar

Para esta primera entrega se seleccionan tres técnicas alcanzables:

### 8.1 Mapa de actores

Permite identificar las personas y organizaciones relacionadas con el problema y comprender cómo se conectan entre sí.

**Estado:** elaborado de manera preliminar.

### 8.2 Entrevista semiestructurada a informante clave

Se realizará una entrevista a un proveedor de oxímetros o soluciones de monitoreo domiciliario.

**Objetivo:** comprender su experiencia, las dificultades que observa, las necesidades de sus clientes y su percepción sobre una solución como EVA.

**Estado:** planeada y pendiente de aplicación.

### 8.3 Mapa de empatía

Se construirá después de la entrevista, utilizando exclusivamente la información obtenida del proveedor.

**Estado:** formato preparado y pendiente de completar.

---

## 9. Planeación de la entrevista

### 9.1 Perfil del informante clave

La entrevista será atendida por un coordinador de Oxiayuda, organización prestadora de servicios de salud domiciliaria.

**Información conocida:**

- presta servicios de salud domiciliaria;
- suministra concentradores de oxígeno;
- trabaja principalmente con equipos de uso doméstico;
- cuenta con experiencia clínica;
- tiene 23 años de experiencia en el sector;
- busca obtener mayor información sobre el uso de sus equipos y sobre los pacientes;
- la consulta será virtual;
- Daniel Pacheco es el integrante que gestiona el contacto.

### 9.2 Información pendiente de confirmar

- cargo exacto del coordinador que atenderá la entrevista;
- formación profesional específica;
- fecha y hora de la entrevista;
- duración estimada;
- autorización para mencionar públicamente el nombre Oxiayuda;
- autorización para usar citas textuales;
- autorización para utilizar capturas, fotografías o grabaciones;
- nivel de anonimización solicitado;
- posibilidad de mencionar datos institucionales o comerciales.

### 9.3 Modalidad

La entrevista podrá realizarse mediante:

- llamada telefónica;
- videollamada;
- conversación presencial;
- formulario con respuestas abiertas;
- o notas de voz.

### 9.4 Duración estimada

Entre 20 y 30 minutos.

### 9.5 Presentación al participante

> Somos estudiantes de la Especialización en Inteligencia Artificial y estamos desarrollando un ejercicio académico de Design Thinking relacionado con el monitoreo domiciliario de la saturación de oxígeno. Queremos comprender su experiencia como prestador de servicios de salud domiciliaria y conocer los principales retos que observa en el uso de equipos de oxígeno y dispositivos de seguimiento en el hogar. No buscamos recopilar información clínica ni evaluar tratamientos. Las respuestas se utilizarán únicamente con fines académicos. Antes de citar, grabar, tomar capturas o mencionar el nombre de la organización, solicitaremos su autorización expresa.

---


### 9.6 Tratamiento de privacidad y autorización

Hasta recibir autorización expresa, el grupo aplicará las siguientes reglas:

- no publicará el nombre del coordinador;
- no incluirá datos de pacientes;
- no compartirá historias clínicas ni información sensible;
- utilizará el código **E01** para identificar al informante;
- describirá a la empresa como “prestador de servicios de salud domiciliaria” si no autoriza el uso de su nombre;
- no usará capturas, fotografías, grabaciones ni citas textuales sin consentimiento;
- separará claramente la información institucional de cualquier dato personal o clínico.

La autorización podrá solicitarse al inicio de la entrevista mediante una pregunta directa y quedar registrada en las notas del grupo.

---

## 10. Guía de entrevista semiestructurada

La entrevista debe priorizar experiencias reales y ejemplos concretos. EVA se presentará solamente después de explorar primero la experiencia del proveedor.

### Bloque A — Perfil y contexto

1. ¿Cuál es su función dentro de la organización y cómo se relaciona con la atención domiciliaria, los concentradores de oxígeno y el seguimiento de pacientes?
2. ¿Cuánto tiempo lleva trabajando con este tipo de dispositivos?
3. ¿Qué perfiles de pacientes o familias utilizan con mayor frecuencia los servicios y equipos de la organización?
4. ¿En qué situaciones suelen requerirse concentradores de oxígeno u otros dispositivos de monitoreo en el hogar?

### Bloque B — Necesidades y dificultades de los usuarios

5. ¿Cuáles son las dudas más frecuentes de los pacientes y cuidadores sobre el uso de los equipos en casa?
6. ¿Qué dificultades de uso, adherencia o seguimiento suelen reportar?
7. ¿Qué errores o confusiones aparecen con mayor frecuencia durante el uso de los equipos o la toma de mediciones?
8. ¿Qué hacen normalmente los usuarios cuando observan un valor que consideran preocupante?
9. ¿Qué información sobre el uso de los equipos o el estado del paciente le hace falta actualmente a la organización?
10. ¿Existen perfiles de usuario para los cuales el uso del dispositivo sea especialmente difícil?

### Bloque C — Confianza, interpretación y alertas

11. ¿Qué factores hacen que un usuario confíe o desconfíe de una medición?
12. ¿Considera útil mostrar mediciones anteriores o tendencias además del valor actual?
13. ¿Qué características debería tener una alerta para ser útil y no generar confusión?
14. ¿Qué riesgos identifica en un sistema que genere alertas automáticamente?
15. ¿Qué información debería recibir el usuario antes de recomendarle que contacte a su entidad de salud?

### Bloque D — Validación inicial de EVA

16. ¿Qué opinión le merece un dispositivo que recuerde al paciente realizar la medición?
17. ¿La activación por voz podría facilitar el uso para algunos usuarios? ¿Para cuáles?
18. ¿Qué tan útil podría ser que el análisis inicial se realice localmente, incluso sin conexión permanente a internet?
19. ¿Qué tan útil sería para Oxiayuda recibir reportes sobre uso del equipo, mediciones y alertas? ¿Qué información debería contener?
20. ¿Qué función no debería asumir automáticamente una herramienta como EVA?
21. ¿Qué aspectos de privacidad, confianza o responsabilidad deberían considerarse?
22. ¿Qué recomendación le daría al equipo antes de desarrollar la solución?

### Preguntas de profundización

- ¿Puede darme un ejemplo?
- ¿Qué ocurrió después?
- ¿Por qué considera que sucede?
- ¿Qué fue lo más difícil?
- ¿Cómo reaccionó el usuario?
- ¿Qué habría ayudado en esa situación?

---

## 11. Modelo de registro de la entrevista

### Datos básicos

| Campo | Registro |
|---|---|
| Código del participante | E01 |
| Perfil | Coordinador de prestador de salud domiciliaria |
| Fecha | [Pendiente] |
| Modalidad | Virtual |
| Duración | [Pendiente] |
| Contacto gestionado por | Daniel Pacheco |
| Organización | Oxiayuda — nombre sujeto a autorización |
| Experiencia de la organización | 23 años |
| Tipo de servicio | Suministro de concentradores de oxígeno y atención domiciliaria |
| Formación o experiencia clínica | Sí — detalle pendiente |
| Autorización para mencionar la empresa | [Pendiente] |
| Autorización para citas | [Pendiente] |
| Autorización para capturas o grabaciones | [Pendiente] |

### Registro cualitativo

**Situaciones principales descritas**

- [Pendiente de entrevista]

**Dificultades identificadas**

- [Pendiente de entrevista]

**Necesidades mencionadas o inferidas**

- [Pendiente de entrevista]

**Frases textuales relevantes**

> “[Pendiente de entrevista]”

> “[Pendiente de entrevista]”

**Algo que sorprendió al grupo**

- [Pendiente de entrevista]

**Preguntas que quedaron abiertas**

- [Pendiente de entrevista]

---

## 12. Modelo de mapa de empatía

Este mapa será completado después de la entrevista y representará la perspectiva del proveedor.

### ¿Qué piensa y siente?

- ¿Qué le preocupa sobre los dispositivos y sus usuarios?
- ¿Qué considera importante para ofrecer una solución confiable?
- ¿Qué riesgos quiere evitar?

### ¿Qué ve?

- ¿Qué comportamientos observa en pacientes y cuidadores?
- ¿Qué problemas aparecen durante la compra, instalación o soporte?
- ¿Qué limitaciones encuentra en los oxímetros actuales?

### ¿Qué escucha?

- ¿Qué preguntas recibe de clientes?
- ¿Qué comentarios recibe de profesionales o entidades de salud?
- ¿Qué reclamos o solicitudes son recurrentes?

### ¿Qué dice y hace?

- ¿Cómo orienta actualmente a los compradores?
- ¿Qué recomendaciones entrega?
- ¿Qué acciones toma cuando un usuario reporta una medición preocupante?

### Dolores o frustraciones

- [Pendiente de entrevista]

### Necesidades o beneficios esperados

- [Pendiente de entrevista]

### Evidencias que respaldan el mapa

- Cita E01: “[Pendiente]”
- Situación descrita: [Pendiente]
- Observación del grupo: [Pendiente]

---

## 13. Cómo se analizarán los resultados

| Nivel | Definición | Ejemplo de formato |
|---|---|---|
| Supuesto | Idea inicial del grupo antes de consultar al proveedor. | Creemos que los usuarios olvidan realizar las mediciones. |
| Evidencia | Respuesta, experiencia o cita del participante. | “Muchos compradores preguntan cada cuánto deben medirse”. |
| Hallazgo | Observación construida a partir de la evidencia. | Existe incertidumbre sobre la frecuencia del seguimiento. |
| Insight preliminar | Interpretación que revela una necesidad o tensión relevante. | Un recordatorio sin contexto puede no ser suficiente si el usuario no comprende el propósito de la medición. |
| Necesidad | Necesidad humana o del segmento. | El usuario necesita comprender cuándo, cómo y por qué realizar la medición. |
| Implicación para EVA | Posible cambio o validación de la propuesta. | El recordatorio debería incluir una orientación breve y comprensible. |

> Con una sola entrevista no se hablará de tendencias estadísticas ni de resultados representativos. Se utilizarán expresiones como “hallazgo exploratorio”, “perspectiva del informante” e “insight preliminar”.

---

## 14. Evidencias planeadas

- guía de entrevista utilizada;
- ficha anónima del participante;
- fecha, modalidad y duración;
- respuestas o notas de la conversación;
- citas textuales autorizadas;
- captura, fotografía o evidencia de contacto, si existe autorización;
- mapa de empatía completado;
- hallazgos preliminares;
- necesidades identificadas;
- implicaciones iniciales para EVA;
- y limitaciones de la exploración.

---

## 15. Limitaciones de esta entrega

- La entrega se concentra en la planeación de Empatizar.
- La entrevista aún no ha sido aplicada al momento de preparar este borrador.
- Se seleccionó un único informante clave.
- No se han entrevistado directamente pacientes, cuidadores ni profesionales de salud.
- Los supuestos no deben presentarse como hechos confirmados.
- Las funciones de EVA son hipótesis de solución.
- No existe validación clínica.
- El tiempo asignado para la actividad es reducido.
- La primera aproximación no representa todo el mercado.
- El mapa de empatía se completará después de recibir evidencia real.

### Trabajo posterior recomendado

1. Realizar la entrevista al proveedor.
2. Incorporar las respuestas y citas autorizadas.
3. Completar el mapa de empatía.
4. Extraer hallazgos e insights preliminares.
5. Refinar las funciones de EVA.
6. Ampliar la investigación hacia pacientes, cuidadores y profesionales.
7. Construir posteriormente un recorrido de usuario o Customer Journey.

---

## 16. Recurso técnico preliminar

**Health Status Dataset — Kaggle**  
https://www.kaggle.com/datasets/jacobhealth/health-status-dataset

Este dataset no se presenta como evidencia de la fase Empatizar. Antes de utilizarlo será necesario evaluar:

- variables disponibles;
- calidad de los datos;
- población representada;
- distribución de clases;
- relación real con la saturación de oxígeno;
- restricciones de licencia;
- sesgos;
- y pertinencia para el objetivo de EVA.

---

## 17. Guía de presentación — máximo 10 diapositivas

La presentación debe funcionar como un pitch breve tipo Shark Tank o elevator pitch: visual, clara y con poco texto.

### Diapositiva 1 — Portada

**EVA — Enfermera Virtual de Asistencia**

> Monitoreo domiciliario inteligente para apoyar la identificación temprana de posibles señales de riesgo en la saturación de oxígeno.

Incluir nombre del proyecto, grupo, integrantes, asignatura y una imagen o render del dispositivo.

### Diapositiva 2 — El problema

Mostrar:

- dificultad para mantener una rutina de medición;
- incertidumbre al interpretar valores;
- necesidad de orientación;
- dificultad para comunicar alertas.

Usar lenguaje de hipótesis: “Buscamos comprender si…”

### Diapositiva 3 — La propuesta EVA

> Recordar → Medir → Analizar localmente → Alertar → Orientar → Reportar

Mostrar únicamente las funciones principales.

### Diapositiva 4 — Segmento y actores

Segmento inicial:

> Proveedores de oxímetros y soluciones de monitoreo respiratorio domiciliario.

Mostrar alrededor al paciente, cuidador, profesional y entidad de salud.

### Diapositiva 5 — ¿Por qué empezar con el proveedor?

- conoce dudas frecuentes;
- observa dificultades reales;
- interactúa con distintos tipos de usuario;
- conoce características y limitaciones de los equipos;
- es accesible para la primera exploración.

### Diapositiva 6 — Cómo planeamos Empatizar

Mostrar:

1. mapa de actores;
2. entrevista semiestructurada;
3. mapa de empatía posterior.

Añadir:

> Estado actual: planeación y programación de la aplicación.

### Diapositiva 7 — Modelo de entrevista

Mostrar solamente los bloques:

- perfil y contexto;
- necesidades del usuario;
- dificultades de medición;
- confianza e interpretación;
- alertas;
- validación inicial de EVA.

### Diapositiva 8 — Evidencias y análisis esperado

- ficha del informante;
- notas y citas;
- mapa de empatía;
- hallazgos exploratorios;
- necesidades;
- implicaciones para EVA.

### Diapositiva 9 — Qué esperamos aprender

- principales dificultades del mercado;
- necesidades del proveedor y sus clientes;
- riesgos de las alertas automáticas;
- valor de los recordatorios;
- utilidad de la activación por voz;
- información necesaria para una alerta centralizada;
- funciones que EVA debería modificar o descartar.

### Diapositiva 10 — Próximos pasos y cierre

- aplicar la entrevista;
- completar el mapa de empatía;
- refinar EVA;
- ampliar la exploración a usuarios finales;
- pasar posteriormente a la fase Definir.

Frase de cierre:

> EVA busca que una medición no sea solamente un número, sino una señal comprensible que ayude al paciente a buscar apoyo en el momento adecuado.

---

## 18. Recomendaciones de diseño

- Una idea principal por diapositiva.
- Evitar párrafos extensos.
- Usar diagramas, íconos y flujos.
- Mantener una paleta de máximo tres colores principales.
- Usar tipografía legible.
- Resaltar el nombre EVA.
- Diferenciar problema, hipótesis y evidencia.
- No presentar resultados que todavía no existen.
- Mantener visible el enfoque humano y académico.
- Reservar detalles técnicos para anexos.

---

## 19. Bibliografía y recursos sugeridos

- Stanford d.school. Recursos sobre Design Thinking y métodos de empatía.
- IDEO.org. *The Field Guide to Human-Centered Design*.
- Organización Mundial de la Salud. Materiales educativos relacionados con oximetría de pulso.
- Material académico de la asignatura Innovación Digital, cuando sea publicado.
- Health Status Dataset de Kaggle, únicamente como recurso técnico preliminar.
- Documentación técnica oficial de Raspberry Pi para futuras decisiones de implementación.

> Las referencias definitivas deben verificarse y formatearse según el estilo solicitado por el docente.

---

## 20. Checklist de revisión

### Contenido

- [ ] EVA aparece con su nombre completo correcto.
- [ ] El segmento inicial está claramente definido.
- [ ] La problemática está formulada como hipótesis.
- [ ] Las funciones de EVA se presentan como propuesta inicial.
- [ ] Se describen las tres técnicas de empatía.
- [ ] La entrevista tiene objetivo, perfil y preguntas.
- [ ] Existe un formato de registro.
- [ ] El mapa de empatía está marcado como pendiente.
- [ ] Se reconocen las limitaciones.
- [ ] No se inventan entrevistas, citas ni resultados.

### Presentación

- [ ] Tiene máximo 10 diapositivas.
- [ ] Se entiende en pocos minutos.
- [ ] Mantiene una narrativa de problema, propuesta y plan de validación.
- [ ] Utiliza elementos visuales.
- [ ] Tiene ortografía revisada.
- [ ] Incluye referencias cuando sea posible.
- [ ] Todos los integrantes revisaron la versión final.
- [ ] Daniel Pacheco cuenta con el archivo definitivo para cargar.

---

## 21. Estado de pendientes

| Pendiente | Responsable | Estado |
|---|---|---|
| Confirmar cargo y formación del coordinador de Oxiayuda | Daniel Pacheco | En gestión |
| Confirmar autorización para mencionar a Oxiayuda | Daniel Pacheco | En gestión |
| Confirmar autorización para citas, capturas o grabaciones | Daniel Pacheco | En gestión |
| Programar entrevista virtual | Daniel Pacheco / coordinador de Oxiayuda | En gestión |
| Aplicar entrevista | Coordinador de Oxiayuda y equipo | Pendiente |
| Registrar evidencias | [Por definir] | Pendiente |
| Completar mapa de empatía | [Por definir] | Pendiente |
| Incorporar resultados en una entrega posterior | Todo el grupo | Pendiente |
| Preparar presentación de máximo 10 diapositivas | Compañera responsable | En proceso |
| Revisar contenido final | Todo el grupo | Pendiente |
| Cargar presentación | Daniel Pacheco | Pendiente |

---

## Nota final

Este documento corresponde a una planeación académica de la fase Empatizar. No constituye validación clínica, diagnóstico médico ni evidencia de aceptación de mercado. Las decisiones posteriores sobre EVA deberán apoyarse en investigación adicional con usuarios, cuidadores, proveedores y profesionales de salud.
