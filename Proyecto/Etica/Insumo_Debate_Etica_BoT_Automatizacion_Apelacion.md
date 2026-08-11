# Insumo individual para debate grupal
## Ética de Blockchain of Things (BoT) en mercados de carbono
### Enfoque: automatización excesiva, apelación y corrección sin perder inmutabilidad

**Actividad:** Evaluación formativa — Caso Ética de Blockchain de las Cosas  
**Caso base:** Sadawi et al. (2021)  
**Estado:** Insumo individual para discusión del grupo. No corresponde todavía a las dos recomendaciones finales del equipo.

---

## 1. Punto de partida

El caso de Sadawi et al. (2021) propone un sistema jerárquico basado en **Blockchain of Things (BoT)** y **smart contracts** para mejorar el comercio de emisiones de carbono.

Los autores parten de problemas existentes en estos mercados, entre ellos:

- manipulación;
- falta de integridad;
- dificultades de trazabilidad;
- y otras debilidades que afectan un comercio de carbono justo.

Como respuesta, plantean una arquitectura blockchain jerárquica de tres etapas que combina dispositivos conectados, blockchain y contratos inteligentes. Entre los beneficios esperados destacan:

- seguridad;
- inmutabilidad;
- transparencia;
- trazabilidad;
- confianza;
- y automatización de mecanismos de comercio y control.

El objetivo del sistema es mejorar la integridad del mercado de carbono y reducir oportunidades de fraude o manipulación.

Nuestra discusión ética no busca negar esas ventajas. El punto que queremos analizar es qué ocurre cuando la automatización se apoya en un dato que posteriormente resulta incorrecto o discutible.

---

## 2. Riesgo ético seleccionado: automatización excesiva

Nuestro principal riesgo no es la inmutabilidad de blockchain en sí misma.

De hecho, consideramos que conservar un registro histórico que no pueda modificarse arbitrariamente es una de las ventajas más útiles de la propuesta.

El problema aparece cuando se combinan tres elementos:

```text
Dato IoT
   ↓
Registro blockchain
   ↓
Smart contract
   ↓
Consecuencia automática
```

Si el sistema asume que todo dato almacenado es necesariamente correcto, una lectura incorrecta puede convertirse automáticamente en una consecuencia económica o regulatoria.

Por ejemplo, una medición podría verse afectada por:

- error del sensor;
- mala calibración;
- fallo de comunicación;
- configuración incorrecta;
- manipulación;
- mantenimiento deficiente;
- o una situación excepcional que requiera interpretación.

Blockchain puede demostrar con gran confiabilidad **qué dato fue registrado y cuándo**.

Eso no demuestra necesariamente que el dato representara correctamente la realidad física.

Por ello, nuestra preocupación puede resumirse así:

> **La inmutabilidad puede proteger la integridad del registro, pero no garantiza por sí sola la verdad del dato de origen.**

---

## 3. El problema no es “garbage in, garbage forever”

Una reacción simple ante este riesgo sería afirmar que un dato incorrecto almacenado en blockchain queda permanentemente incorrecto.

Nuestra postura es diferente.

Creemos que precisamente la trazabilidad de blockchain puede aprovecharse para construir un sistema donde el dato original jamás sea eliminado, pero pueda ser:

- cuestionado;
- revisado;
- verificado;
- confirmado;
- o sustituido para efectos operacionales mediante un nuevo registro relacionado.

La idea sería conservar el historial completo.

```text
Dato original
     │
     ▼
Registro inmutable
     │
     ├── Sin controversia ──────► VALIDADO
     │
     └── Apelado
            │
            ▼
      Proceso de revisión
            │
            ▼
      Resultado de auditoría
            │
       ┌────┴────┐
       ▼         ▼
 CONFIRMADO   CORREGIDO
                 │
                 ▼
          Nuevo registro/anexo
```

El dato inicial permanece visible.

La corrección no lo borra ni lo reescribe.

En cambio, el sistema agrega nueva evidencia que modifica cuál es el **estado vigente** para las decisiones posteriores.

---

## 4. Nuestra idea central

Nuestra postura puede resumirse en una frase:

> **La inmutabilidad debería aplicarse a la evidencia histórica, no necesariamente a las consecuencias de una decisión automatizada.**

Esto permite mantener las propiedades que motivan el uso de blockchain:

- trazabilidad;
- integridad;
- transparencia;
- auditabilidad;
- dificultad de manipulación.

Pero evita tratar al primer dato registrado como una verdad incuestionable.

Un sistema éticamente mejor diseñado debería ser capaz de distinguir entre:

- lo que ocurrió originalmente;
- lo que fue cuestionado;
- qué evidencia apareció posteriormente;
- quién realizó la revisión;
- y cuál es el estado reconocido actualmente.

---

## 5. Recomendación principal para llevar al grupo

> **Incorporar un mecanismo formal de apelación, verificación y corrección mediante registros anexos para las decisiones automatizadas ejecutadas a partir de datos IoT. El dato y la transacción originales deben permanecer inmutables, pero el sistema debe permitir registrar una disputa, documentar la revisión y asociar una corrección o resolución posterior. Para efectos del comercio de carbono, el estado válido debe determinarse a partir de la cadena completa de registros relacionados y no únicamente del primer valor almacenado.**

Esta recomendación no busca eliminar los smart contracts ni reemplazar la automatización por procesos manuales.

Busca agregar una capa de gobernanza para los casos excepcionales.

---

## 6. Ejemplo conceptual

Supongamos que un sensor registra una emisión que genera automáticamente una operación sobre créditos de carbono.

### Diseño sin mecanismo de apelación

```text
Sensor: 100 unidades
        ↓
Blockchain: registra 100
        ↓
Smart contract: ejecuta transacción
        ↓
Resultado definitivo
```

Posteriormente se descubre que el sensor estaba mal calibrado y el valor correcto era 80.

Blockchain hizo correctamente su trabajo: preservó el valor que recibió.

El problema fue que el sistema convirtió ese valor en una consecuencia definitiva sin contemplar un mecanismo de revisión.

### Diseño propuesto

```text
Registro 001
Medición original: 100
Estado: REGISTRADO

Registro 002
Disputa sobre Registro 001
Motivo: posible error de calibración
Estado: EN REVISIÓN

Registro 003
Auditoría del dispositivo
Resultado verificado: 80

Registro 004
Corrección vinculada a Registro 001
Valor reconocido: 80
Estado: SUSTITUIDO PARA EFECTOS OPERATIVOS
```

El sistema conserva que inicialmente se registró 100.

También conserva por qué se cuestionó, qué ocurrió durante la revisión y cuál fue finalmente el valor reconocido.

Nada se borra.

---

## 7. Estado histórico vs. estado vigente

Una consecuencia interesante de nuestra propuesta es que las aplicaciones que consultan la blockchain no deberían preguntar únicamente:

> “¿Cuál fue el dato registrado?”

También deberían poder preguntar:

> **“¿Cuál es el estado vigente de este dato después de considerar todas las revisiones asociadas?”**

Por ejemplo:

```text
REGISTERED
    ↓
VALIDATED
```

o:

```text
REGISTERED
    ↓
DISPUTED
    ↓
REVIEWED
    ↓
CONFIRMED
```

o:

```text
REGISTERED
    ↓
DISPUTED
    ↓
REVIEWED
    ↓
SUPERSEDED
```

Esto preserva el carácter *append-only* del registro: los eventos posteriores complementan la historia en lugar de modificarla.

---

## 8. ¿Por qué mejora la ética del sistema?

### 8.1 Justicia

Una empresa o participante no debería quedar afectado permanentemente por una decisión automatizada derivada de un dato demostrablemente incorrecto.

Un mecanismo de apelación proporciona una vía para cuestionar esa decisión.

### 8.2 Responsabilidad

La revisión puede dejar evidencia de:

- qué sensor produjo el dato;
- cuándo fue registrado;
- qué smart contract actuó;
- qué consecuencia generó;
- quién inició la disputa;
- qué evidencia se revisó;
- quién autorizó la resolución;
- y qué corrección fue aplicada.

Esto fortalece la responsabilidad en lugar de permitir que se responda simplemente:

> “El smart contract lo ejecutó.”

### 8.3 Transparencia

La corrección no elimina la historia anterior.

Un auditor puede observar tanto el error como su solución.

### 8.4 Prevención de daño

La automatización sigue resolviendo el caso normal, pero las situaciones anómalas pueden escalar a revisión antes de producir o mantener consecuencias desproporcionadas.

### 8.5 Confianza

Un mercado puede generar mayor confianza cuando sus participantes saben que:

- los registros no se pueden manipular silenciosamente;
- pero los errores demostrables tampoco son irreversibles.

---

## 9. Automatización por defecto, revisión humana por excepción

No proponemos que una persona valide manualmente cada medición o cada transacción.

Eso eliminaría buena parte de la eficiencia que Sadawi et al. buscan mediante smart contracts y automatización.

Nuestra propuesta sería:

> **Automatización por defecto; revisión humana por excepción.**

El flujo normal permanece automático.

La intervención adicional aparece cuando existe, por ejemplo:

- una disputa formal;
- una lectura fuera de parámetros razonables;
- evidencia de fallo del sensor;
- inconsistencias entre fuentes;
- sospecha de manipulación;
- o una consecuencia económica relevante que requiera revisión.

Esto permite conservar eficiencia sin asumir que automatización significa ausencia de supervisión.

---

## 10. Condiciones que debería tener el mecanismo de apelación

Para que la propuesta no se convierta simplemente en una nueva oportunidad de manipulación, el proceso debería incluir reglas claras.

### Identidad

Debe quedar registrado quién:

- genera la medición;
- inicia una disputa;
- realiza la revisión;
- y aprueba la resolución.

### Evidencia

La apelación debería requerir evidencia verificable, por ejemplo:

- informe de calibración;
- comparación con sensores independientes;
- registro de mantenimiento;
- auditoría técnica;
- evidencia de fallo;
- o verificación por una entidad autorizada.

### Trazabilidad

Cada registro posterior debe referenciar criptográficamente al evento que está complementando o cuestionando.

### Separación de funciones

Cuando sea posible, quien se beneficia directamente de una corrección no debería ser la única parte que decide sobre ella.

### Estados claros

El sistema debería distinguir como mínimo entre:

- registrado;
- validado;
- disputado;
- en revisión;
- confirmado;
- corregido o sustituido.

### Reversibilidad de consecuencias

Cuando una corrección sea aceptada, los smart contracts posteriores deberían utilizar el estado vigente.

Si una transacción económica ya ocurrió, una nueva operación correctiva debería compensarla sin borrar la operación original.

---

## 11. Relación con el diseño de Sadawi et al.

Es importante diferenciar qué proviene del artículo y qué proponemos nosotros.

### El artículo sí propone

Sadawi et al. plantean:

- un esquema jerárquico de tres etapas;
- integración de blockchain con dispositivos IoT;
- uso de smart contracts;
- transparencia;
- trazabilidad;
- inmutabilidad;
- mecanismos automatizados de comercio;
- y mecanismos automatizados de control.

Los autores presentan estas propiedades como mejoras frente a problemas de manipulación e integridad del comercio de carbono.

### Nuestra propuesta añade

A partir de ese diseño identificamos un riesgo ético adicional:

> cuanto mayor sea la automatización de las consecuencias, más importante resulta contar con mecanismos para cuestionar datos y decisiones incorrectas.

El esquema explícito de:

```text
dato original
+
disputa
+
auditoría
+
anexo correctivo
=
estado vigente
```

es nuestra propuesta para el debate.

No debe atribuirse a Sadawi et al. salvo que una lectura completa posterior del artículo muestre un mecanismo equivalente.

---

## 12. Preguntas para discutir con el grupo

### ¿Un dato almacenado en blockchain debe considerarse verdadero?

Nuestra respuesta sería:

**No necesariamente.**

Blockchain puede proporcionar evidencia sólida de que un determinado valor fue registrado de determinada forma y en determinado momento.

La veracidad física de la medición depende también de la calidad y confiabilidad de su origen.

### ¿Permitir correcciones destruye la inmutabilidad?

**No, si la corrección es un nuevo registro.**

No proponemos modificar:

```text
100 → 80
```

en el mismo bloque.

Proponemos conservar:

```text
Registro original: 100
Registro posterior: el valor 100 fue disputado
Auditoría: valor correcto 80
Corrección: para efectos actuales, utilizar 80
```

La historia completa permanece inmutable.

### ¿Por qué no detener todas las transacciones hasta una revisión humana?

Porque eso eliminaría buena parte de la eficiencia de los smart contracts.

La revisión debería reservarse para excepciones y situaciones de mayor riesgo.

### ¿Qué ocurre si alguien apela únicamente para retrasar una obligación?

El derecho a disputar tampoco debería ser ilimitado.

Deberían existir:

- causales de apelación;
- evidencia mínima;
- plazos;
- autoridades o verificadores;
- y consecuencias para disputas fraudulentas.

### ¿Quién debería decidir si una corrección es válida?

No debería decidirlo automáticamente la parte beneficiada.

El modelo de gobernanza podría utilizar:

- verificadores certificados;
- auditorías independientes;
- organismos reguladores;
- o mecanismos de consenso entre actores autorizados.

La forma concreta dependerá del mercado regulado.

### ¿El smart contract debería poder corregir automáticamente una decisión?

Puede **ejecutar** automáticamente la corrección una vez que el proceso de verificación determine el nuevo estado.

Lo que no proponemos es que el propio smart contract resuelva autónomamente una controversia compleja cuando esta depende de evidencia externa o interpretación humana.

---

## 13. Posible formulación para la recomendación grupal

Como punto de partida para que el equipo la discuta:

> **Recomendamos incorporar al sistema BoT un mecanismo auditable de apelación y corrección para los eventos que generen consecuencias automáticas. Los registros originales deben permanecer inmutables, mientras que las disputas, verificaciones y resoluciones se agregarían como nuevos registros vinculados. De esta forma, la blockchain conserva la trazabilidad completa, pero los smart contracts pueden operar sobre el último estado validado y no sobre un dato que posteriormente haya sido demostrado como incorrecto. La medida reduciría riesgos de automatización excesiva, fortalecería la justicia y la responsabilidad y permitiría corregir errores sin sacrificar la integridad histórica del sistema.**

---

## 14. Posible segunda línea de discusión

La actividad final exige dos recomendaciones.

Nuestra recomendación principal es la de apelación y corrección.

Como segunda línea para discutir con el grupo —sin decidirla todavía— podríamos evaluar alguna de estas posibilidades:

- gobernanza y certificación de dispositivos IoT;
- privacidad y minimización de la información pública;
- eficiencia energética del mecanismo blockchain;
- auditoría independiente de smart contracts;
- o definición jurídica de responsabilidades entre sensores, operadores, desarrolladores y participantes del mercado.

La decisión debería tomarse después de conocer los argumentos de los demás integrantes.

---

## 15. Postura individual resumida

No consideramos que la solución ética sea reducir la automatización hasta volver manual el sistema.

Los smart contracts y la blockchain pueden aportar eficiencia, transparencia y trazabilidad al mercado de carbono.

Sin embargo, un sistema automatizado responsable debe reconocer que sus entradas pueden fallar.

Por ello:

> **Un registro no debe poder borrarse, pero sí debe poder discutirse.**

Y cuando la evidencia demuestre que fue incorrecto:

> **la corrección también debe quedar registrada de forma inmutable.**

El resultado sería un sistema que no intenta esconder sus errores, sino que preserva tanto el error como la evidencia de cómo fue identificado y corregido.

---

## 16. Referencia principal

Sadawi, A. A., Madani, B., Saboor, S., Ndiaye, M., & Abu-Lebdeh, G. (2021). *A comprehensive hierarchical blockchain system for carbon emission trading utilizing blockchain of things and smart contract*. **Technological Forecasting and Social Change, 173**, 121124.  
https://doi.org/10.1016/j.techfore.2021.121124

### Fuente consultada

Elsevier — ScienceDirect. Registro oficial del artículo, resumen, aspectos destacados y descripción del marco CHBETS.  
https://www.sciencedirect.com/science/article/pii/S0040162521005576

---

## Nota para el grupo

Este documento pretende servir como **aporte individual al debate**. La recomendación final del taller debe construirse después de comparar esta posición con los riesgos y propuestas identificados por los demás integrantes.

También conviene distinguir en la versión final entre:

- características que Sadawi et al. efectivamente proponen;
- riesgos éticos inferidos por el grupo;
- y modificaciones de diseño propuestas por nosotros.
