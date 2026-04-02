# Hoja de Ruta para Construir un Sistema de Normas de Construccion en Neuquen

La forma correcta de construir este sistema no es arrancar con automatizaciones o con IA avanzada, sino crear primero una base documental confiable y una estructura que despues pueda crecer sin romperse. La prioridad es: fuente oficial, orden, trazabilidad y recien despues consulta inteligente.

## Fase 1: Fundamento documental
Objetivo: reunir el material base con criterio y evitar construir sobre datos dudosos.

1. Defini el alcance inicial.
Elegi un recorte acotado para empezar, por ejemplo:
- Plottier
- Neuquen Capital
- Centenario

2. Identifica solo fuentes primarias.
Prioriza:
- Municipios y digestos oficiales
- Colegio de Arquitectos / consejos profesionales
- Organismos tecnicos como Camuzzi, ENARGAS, EPEN, EPAS
- Boletines y organismos provinciales cuando corresponda

3. Descarga unicamente documentos oficiales.
Guarda:
- codigos urbanos
- codigos de edificacion
- ordenanzas complementarias
- requisitos de tramites
- normas tecnicas de servicios

4. Nombra y archiva con un estandar fijo.
Ejemplo:
- `Plottier_Codigo_Planeamiento_Ord3558_2014.pdf`
- `Neuquen_Codigo_Edificacion_Ord6485.pdf`

Si no sabes si algo esta vigente, no lo asumas:
- marca `A verificar`

## Fase 2: Estructura minima sostenible
Objetivo: que el sistema sea simple, usable y mantenible desde el dia 1.

Arma una estructura como esta:

```text
/Normativa-Construccion
  /01_Fuentes_Originales
    /Plottier
    /Neuquen
    /Centenario
    /Provincial
    /Servicios
  /02_Fichas
    /Plottier
    /Neuquen
    /Centenario
  /03_Base_Maestra
  /04_Cambios_y_Actualizaciones
```

La regla es:
- el PDF original no se toca
- la interpretacion va en fichas separadas
- la base maestra referencia siempre el documento fuente

## Fase 3: Base maestra
Objetivo: dejar de depender de la memoria y empezar a gestionar informacion.

Crea una base en Notion, Airtable o incluso Excel con estos campos:
- `ID`
- `Municipio`
- `Tema`
- `Tipo de norma`
- `Numero oficial`
- `Titulo`
- `Fecha`
- `Estado de vigencia`
- `Fuente oficial`
- `Archivo`
- `Palabras clave`
- `Notas`
- `Ultima verificacion`

Esto te da trazabilidad. Sin esta capa, despues la IA mezcla todo.

## Fase 4: Fichas practicas por documento
Objetivo: convertir PDFs largos en informacion consultable.

Por cada norma importante, hace una ficha con:
- resumen ejecutivo
- alcance
- parametros clave
- articulos relevantes
- tramites involucrados
- dudas o ambiguedades
- modificatorias conocidas

Los parametros prioritarios a extraer son:
- `FOS`
- `FOT`
- retiros
- alturas maximas
- zonificacion
- usos permitidos
- densidad
- requisitos de planos
- exigencias de servicios

No intentes extraer todo de golpe. Primero hace 3 a 5 fichas bien hechas.

## Fase 5: Capa de consulta con IA
Objetivo: usar IA sin perder confiabilidad.

Cuando ya tengas PDFs ordenados y fichas minimas, recien ahi:
- subi los documentos a NotebookLM o sistema similar
- pregunta siempre por dato + fuente + articulo
- usa la IA para resumir, comparar y ubicar informacion
- valida todo lo importante contra el PDF

La IA no reemplaza la fuente. La IA acelera la lectura.

## Fase 6: Politica de calidad
Objetivo: que el sistema siga siendo confiable cuando crezca.

Defini estas reglas:
- no cargar documentos sin fuente oficial
- no afirmar vigencia si no esta verificada
- no mezclar interpretacion con texto normativo
- toda respuesta importante debe citar documento y articulo si existe
- toda actualizacion debe dejar registro

Esto es lo que hace sostenible el sistema.

## Fase 7: Mantenimiento
Objetivo: evitar que se vuelva obsoleto.

Establece una revision periodica:
- mensual si el volumen es bajo
- quincenal si trabajas mucho con tramites

Revisa:
- nuevas ordenanzas
- modificatorias
- cambios en requisitos municipales
- cambios en normativas de servicios

Guarda cada cambio en `04_Cambios_y_Actualizaciones`.

## Fase 8: Automatizacion
Objetivo: automatizar solo cuando el sistema ya tiene criterio.

Recien despues podes sumar `n8n` para:
- detectar nuevas publicaciones
- descargar documentos
- generar borradores de ficha
- marcar posibles cambios
- enviar alertas

No conviene automatizar antes de tener:
- estructura
- base maestra
- reglas de calidad
- criterios de vigencia

## Orden recomendado de implementacion
1. Elegir 2 o 3 municipios iniciales.
2. Reunir PDFs oficiales base.
3. Crear estructura de carpetas.
4. Crear base maestra.
5. Hacer primeras fichas manuales.
6. Probar consultas con IA.
7. Ajustar criterios.
8. Automatizar actualizacion.

## Version minima viable correcta
Si quieres hacerlo de a poco pero bien, tu MVP deberia ser este:
- `3 municipios`
- `10 a 20 documentos oficiales`
- `1 base maestra`
- `5 fichas completas`
- `1 herramienta de consulta con citas`

Eso ya te da valor real sin sobreconstruir.
