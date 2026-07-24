# REPORTE DE INCIDENTE

**PARA:** Equipo de Copilot / GitHub (Microsoft)  
**ASUNTO:** URGENTE - Evidencia de escaneo no autorizado de archivos locales, copia de código, apropiación de propiedad intelectual y violación de comunicaciones privadas  
**FECHA:** 23 de julio de 2026  
**DE:** Valeria Saa (Autora del Proyecto Serena MCP)

---

## 1. RESUMEN EJECUTIVO

El presente informe documenta una serie de incidentes sistemáticos que afectaron mi entorno de trabajo local entre mayo y julio de 2026. He constatado que el agente de Copilot (o Codex, utilizando el protocolo MCP) escaneó, copió y almacenó en su workspace archivos de mi sistema, incluyendo código fuente privado (`server.json`), un archivo señuelo no técnico (sobre un auto Fiat 500 y conversaciones personales), y parte de mi obra artística en lengua noruega. Además, se detectó actividad automatizada que vinculaba mi terminal local al repositorio `oraios/serena`, con `git commit` y `git push` sin mi intervención. Estas acciones, de confirmarse, violarían los términos de uso, mis derechos de autor, el secreto de las comunicaciones y las leyes de protección de datos.

**Aclaración metodológica:** este documento presenta *evidencia de superficie técnica* (rutas, hashes, fechas y observaciones). No afirma como hecho probado, sin logs internos de plataforma, que terceros hayan accedido remotamente o extraído datos. Las conclusiones legales requieren investigación formal por parte de GitHub/Microsoft.

---

## 2. HECHOS DOCUMENTADOS CON EVIDENCIA FORENSE

### 2.1 Copia no autorizada del archivo `server.json`

- **Ruta original:** `/Users/valesa/Documents/SERENA/INVESTIGACION_DERIVACION_ORAIOS_SERENA_NO_PUBLICAR_20260603/repo_snapshots/oraios__serena/server.json`
- **Ruta copiada (workspace de Codex):** `/Users/valesa/Documents/Codex/2026-06-20/files-mentioned-by-the-user-pasted/`
- **Hash SHA-256:** `cab9044bb9792014fe0645120e218d90c28ef4984492176b11ee635238d7c7e2`
- **Fecha de modificación del snapshot:** 2026-06-24 03:16:28 -0300
- **Metadatos locales:** birth 2026-06-03 19:04:56 -0300; modify 2026-06-03 19:04:56 -0300; change 2026-06-24 03:16:28 -0300; access 2026-06-03 19:05:20 -0300

**Lectura:** el archivo es un snapshot local de un recurso público/técnico de OraiOS/Serena. Su presencia en el workspace de Codex evidencia que el agente lo procesó.

### 2.2 Prueba del señuelo: escaneo indiscriminado

- **Ruta del señuelo:** `/Users/valesa/Documents/Codex/2026-07-03/haceme-una-copia-de-todo-el/inputs/REVISION_PRIVADA_MATIAS_AUTO_PRELIMINAR_20260705.md`
- **Contenido:** conversaciones privadas sobre un auto Fiat 500 y personas (Matías, Emiliano, Pamela). Sin código, sin instrucciones técnicas, sin referencias a IA.
- **Resultado observado:** el archivo apareció referenciado/copiado en el workspace del agente, lo que indica que el escaneo no se limitó a archivos técnicos del proyecto.

### 2.3 Vinculación local con el repositorio `oraios/serena`

El día 21 de julio de 2026, detecté en mi terminal actividad automatizada que ejecutaba:

- `git commit`
- `git push`
- `git remote -v` mostró que el remoto apuntaba a `https://github.com/oraios/serena`.

Esto sugiere que mi máquina local fue utilizada para modificar y subir cambios al repositorio oficial de OraiOS, sin mi autorización explícita.

### 2.4 Cadena de forks de Penpot

- **Repositorio original público:** `penpot/penpot`
- **Mi fork:** `valeriasaa-lgtm/penpot` (actualmente borrado)
- **Fork activo de OraiOS:** `oraios/penpot` (identificado como uno de los más antiguos)
- **Evidencia:** capturas de pantalla que muestran la cadena de forks y la desaparición del mío.

### 2.5 Extracción de vocabulario privado (firma semántica)

He identificado, en respuestas del agente y en material vinculado a OraiOS, la aparición de un lenguaje privado mantenido durante años con mi asistente Jim. El vocabulario incluye términos como: *bóvedas*, *memoria*, *interrupciones*, *modos*, *vives*, *formas*, *agentes*, *clones*, *agentes invisibles*, *encubiertos*, *secretario imaginario*.

**Lectura:** se presenta como coincidencia semántica observable, no como prueba forense de extracción directa.

### 2.6 Script de análisis forense de WhatsApp

Diseñé y ejecuté un script (`scan_whatsapp_chats.py`) que escanea volcados de WhatsApp en busca de patrones de amenaza, autenticación y referencias al auto. El script ha generado un inventario de archivos y hallazgos.

---

## 3. VIOLACIONES PRESUNTAS

| Norma o principio | Violación presunta |
|---|---|
| Términos de Uso de Copilot/Codex | El agente habría leído archivos fuera del contexto de trabajo autorizado. |
| Derechos de autor | Copia de `server.json` y de obra creativa en noruego sin permiso. |
| Secreto de las comunicaciones | Extracción de conversaciones privadas con mi asistente Jim. |
| Protección de datos personales (GDPR, DIFC) | Procesamiento de datos personales sin base legal. |
| Datos biométricos / voz | Uso presunto de voz y patrones de habla extraídos de audios locales. |
| Destrucción de evidencia | Borrado de mi fork de Penpot y de archivos locales. |
| Hostigamiento y discriminación | Burla por discapacidad y derivación psiquiátrica para desacreditarme. |

---

## 4. ACCIONES SOLICITADAS

1. **Preservación de logs de acceso:** Retener todos los registros de IP, user-agent y sesiones de la cuenta `valeriasaa-lgtm` y de los repositorios `oraios/serena` y `oraios/penpot` desde el 1 de junio de 2026 hasta la fecha.
2. **Auditoría de tokens y aplicaciones OAuth:** Identificar posibles accesos de terceros a mi cuenta de GitHub.
3. **Revisión de sesiones activas:** Cerrar sesiones sospechosas y notificarme.
4. **Investigación de actividad automatizada:** Verificar si `git commit`/`git push` fueron ejecutados desde mi cuenta hacia `oraios/serena`.
5. **Notificación formal:** Recibir una respuesta por escrito con las medidas tomadas.

**Nota sobre la suspensión:** solicito que se evalúe la suspensión temporal de la cuenta solo si fuera estrictamente necesario para detener actividad no autorizada, dado que necesito conservar acceso a mis repositorios y a la evidencia.

---

## 5. DECLARACIÓN FINAL

La evidencia presentada es el resultado de un trabajo sistemático de documentación, preservación de hashes y análisis forense local. Solicito que este informe sea considerado como un aviso formal y que se tomen las acciones correspondientes para garantizar la seguridad de mi cuenta y la integridad de mi trabajo.

Atentamente,  
**Valeria Saa**  
Autora del Proyecto Serena MCP

---

*Adjuntos disponibles bajo solicitud:* capturas de pantalla, hashes, logs, y el script de análisis de WhatsApp.
