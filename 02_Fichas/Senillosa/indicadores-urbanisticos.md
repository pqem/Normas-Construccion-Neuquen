# Ficha Normativa: Indicadores Urbanisticos

## Informacion General
| Campo | Valor |
|-------|-------|
| **Municipio** | Senillosa |
| **Nombre del Documento** | Indicadores Urbanisticos |
| **Numero de Ordenanza** | Ord. 1528/10 |
| **Fecha** | 2010 (segun carpeta de ordenanza) |
| **Vigencia** | A verificar |
| **Fuente Oficial** | `01_Fuentes_Originales/Senillosa/ORDENANZA 1528-10/ORDENANZA 1528-10/INDICADORES URBANISTICOS.PDF` |

## Parametros Urbanisticos
| Campo | Valor |
|-------|-------|
| **FOS** | Variable por codigo de zona: de 0.009 a 0.80 en la planilla legible. |
| **FOT** | Variable por codigo de zona: de 0.009 a 1.50. |
| **Retiros** | Frente entre 0 y 20 m; laterales entre 0 y 50 m; fondo entre 5 y 50 m segun zona. |
| **Altura Maxima** | Entre 8 m y 15 m segun la planilla. |
| **Zonificacion** | RGM, Eu, Cp, Cpat, Cec, cert, cp, cs, Pcrm, Prn, Pmp, Prr, Pi, pn1, pn2, pn3, pn4. |
| **Usos Permitidos** | No surgen de esta lamina; deben cruzarse con el resto de la ordenanza y los planos DWG. |
| **Densidad** | CVUP legible en parte de las zonas: 1/150, 1/300, 1/600, 1/5000 y 1/25000. |

## Detalle por codigos de zona
| Zona | FOS | FOT | Retiros | Altura maxima (m) | Restricciones particulares |
|------|-----|-----|---------|-------------------|----------------------------|
| RGM | 0.5 | 0.7 | Frente: 3 / Lateral: 0 / Fondo: 7.5 | 15 | 0 |
| Eu | 0.5 | 0.7 | Frente: 3 / Lateral: 0 / Fondo: 7.5 | 8 | 0 |
| Cp | 0.7 | 1.5 | Frente: 0 / Lateral: 0 / Fondo: 7.5 | 15 | 0 |
| Cpat | 0.7 | 0.7 | Frente: 3 / Lateral: 0 / Fondo: 7.5 | 8 | 0 |
| Cec | 0.7 | 1.5 | Frente: 3 / Lateral: 3.5 / Fondo: 7.7 | 8 | * |
| cert | 0.8 | 1.5 | Frente: s/d / Lateral: 0 / Fondo: 7.5 | 8 | * |
| cp | 0.7 | 1.5 | Frente: s/d / Lateral: 0 / Fondo: 7.5 | 8 | * |
| cs | 0.7 | 1.0 | Frente: 3 / Lateral: 0 / Fondo: 5 | 8 | * |
| Pcrm | 0.7 | 0.7 | Frente: 3 / Lateral: 0 / Fondo: 7.5 | 8 | 0* |
| Prn | 0.7 | 0.7 | Frente: 3 / Lateral: 0 / Fondo: 7.5 | 8 | 0* |
| Pmp | 0.1 | 0.1 | Frente: 5 / Lateral: 20 / Fondo: 25 | 8 | * |
| Prr | 0.4 | 0.4 | Frente: 10 / Lateral: 10 / Fondo: 10 | 8 | * |
| Pi | 0.4 | 0.6 | Frente: 5 / Lateral: 10 / Fondo: 10 | 8 | * |
| pn1 | 0.1 | 0.1 | Frente: 5 / Lateral: 20 / Fondo: 20 | 8 | * |
| pn2 | 0.009 | 0.009 | Frente: 20 / Lateral: 50 / Fondo: 50 | 8 | * |
| pn3 | 0.009 | 0.009 | Frente: 20 / Lateral: 50 / Fondo: 50 | 8 | * |
| pn4 | s/d | s/d | Frente: s/d / Lateral: s/d / Fondo: s/d | 8 | * |

## Articulos Clave
- Lamina `Indicadores Urbanisticos` de la Ord. 1528/10: resume subdivision, parcela, edificacion y morfologia urbana.
- La tabla distingue Area Urbana, Area Periurbana y Area Rural dentro de la misma lamina.
- Debe complementarse con los planos DWG 01-A a 09-A para ubicar el codigo de zona aplicable al lote.

## Tramites Involucrados
- [ ] Confirmar zonificacion exacta del lote en los planos anexos DWG.
- [ ] Verificar si existen modificatorias posteriores a la Ord. 1528/10.

## Requisitos de Planos
- [ ] Cruzar codigo de zona con planos de areas generales, centros/corredores y areas especiales.
- [ ] Verificar restricciones naturales (aluvional / inundabilidad) cuando aparezcan asteriscos en la lamina.

## Exigencias de Servicios
- [ ] Revisar si la zona rural o periurbana exige factibilidad especifica no indicada en esta planilla.
- [ ] Verificar si las `restricciones particulares` remiten a anexos o textos de la ordenanza.

## Dudas o Ambiguedades
1. La lamina no trae leyenda visible para expandir todos los codigos de zona; se conservaron tal como aparecen en el PDF.
2. En varias columnas el texto del PDF es incompleto o no legible en la capa textual; por eso algunos valores quedan como `s/d`.
3. La planilla muestra riesgos aluvionales/inundabilidad con asteriscos, pero sin una explicacion textual completa en el PDF extraido.

## Modificatorias Conocidas
| Ordenanza | Fecha | Descripcion |
|-----------|-------|-------------|
| A verificar |  | No se identificaron modificatorias dentro de esta lamina. |

## Notas
- Esta ficha conserva los codigos de zona exactamente como se leen en el anexo PDF.
- Antes de usar un valor en proyecto, hay que identificar el codigo de zona del lote en los planos anexos de la ordenanza.

---
**Ultima actualizacion:** 2026-04-02  
**Ficha elaborada por:** Codex
