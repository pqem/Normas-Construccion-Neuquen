# Notas de Arquitectura Abierta

## Estado actual
La arquitectura del sistema queda abierta por ahora. La decision de implementacion se posterga hasta validar mejor el flujo de trabajo, el tipo de documentos, la frecuencia de actualizacion y el nivel real de consulta que se necesita.

La prioridad actual no es elegir stack, sino consolidar:
- criterio de fuentes oficiales
- estructura documental consistente
- base maestra con trazabilidad
- fichas practicas por norma
- reglas de calidad y vigencia

## Opciones de implementacion para evaluar mas adelante
Estas opciones quedan registradas solo como referencia. No implican una decision cerrada.

### Opcion 1: Base documental simple
- Carpeta estructurada de PDFs y fichas
- Base maestra en Excel o Notion
- Consulta asistida con NotebookLM

Ventaja:
- simple, barata y rapida de poner en marcha

Riesgo:
- escalabilidad limitada y automatizacion baja

### Opcion 2: Base documental con automatizacion liviana
- Repositorio o carpeta maestra versionada
- Base de metadatos en Notion, Airtable o planilla
- n8n para seguimiento de actualizaciones y generacion de borradores
- NotebookLM o GPT con documentos cargados

Ventaja:
- buen equilibrio entre orden, velocidad y mantenimiento

Riesgo:
- depende de varios servicios y requiere disciplina operativa

### Opcion 3: Sistema RAG propio
- Almacen documental centralizado
- Base estructurada de metadatos
- Indexacion semantica o vectorial
- Interfaz de consulta propia
- Automatizaciones de ingesta y alertas

Ventaja:
- mayor control, consultas mas potentes y crecimiento a largo plazo

Riesgo:
- complejidad tecnica mas alta y mayor costo de implementacion

## Criterios para decidir la arquitectura despues
Cuando llegue el momento de definir la implementacion, la decision deberia evaluarse segun:
- volumen real de documentos
- frecuencia de actualizacion normativa
- necesidad de trabajar solo o con equipo
- necesidad de trazabilidad legal fina
- presupuesto disponible
- tiempo de mantenimiento aceptable
- necesidad o no de interfaz propia
- necesidad de respuestas con citas exactas y auditoria

## Decision correcta por ahora
La decision correcta en esta etapa es no fijar arquitectura antes de validar el flujo documental, la base maestra, el criterio de vigencia y la utilidad real de las consultas. Primero se consolida el metodo. Despues se elige la implementacion.
