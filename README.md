# Normas-Construccion-Neuquen

Repositorio de trabajo para pensar y construir, de forma gradual y sostenible, un sistema de gestión y consulta de normas de construcción para Neuquén y su área de influencia.

---

## 📁 Estructura del Repositorio

```
/Normas-Construccion-Neuquen
│
├── README.md                              ← Este archivo
├── template_ficha.md                      ← Plantilla para fichas normativas
│
├── /01_Fuentes_Originales                 ← PDFs oficiales descargados
│   ├── /Neuquen_Capital
│   ├── /Plottier
│   ├── /Centenario
│   └── /Senillosa
│
├── /02_Fichas                             ← Fichas prácticas por norma
│   ├── /Neuquen_Capital
│   ├── /Plottier
│   ├── /Centenario
│   └── /Senillosa
│
├── /03_Base_Maestra                       ← Base de datos central
│   └── base_maestra.csv                   ← CSV con todos los metadatos
│
└── /04_Cambios                            ← Registro de actualizaciones
```

---

## 🚀 Cómo usar este sistema

### Paso 1: Descargar documentos oficiales
- Guardar los PDFs originales en `/01_Fuentes_Originales/[Municipio]/`
- Nombrar archivos con estándar: `{Municipio}_{Tipo}_{Número}_{Año}.pdf`
- Ejemplo: `Plottier_Codigo_Planeamiento_Ord3558_2014.pdf`

### Paso 2: Crear ficha normativa
- Usar `template_ficha.md` como base
- Guardar en `/02_Fichas/[Municipio]/[nombre-del-documento].md`
- Extraer: FOS, FOT, retiros, altura, zonificación, usos permitidos

### Paso 3: Registrar en base maestra
- Agregar una línea a `/03_Base_Maestra/base_maestra.csv`
- Completar todos los campos obligatorios
- Actualizar campo "Última Verificación"

### Paso 4: Documentar cambios
- Guardar registros de actualizaciones en `/04_Cambios/`
- Formato: `YYYY-MM-DD_[descripcion].md`

---

## 📋 Campos de la Base Maestra

| Campo | Descripción |
|-------|-------------|
| `ID` | Identificador único (ej: NQN-001) |
| `Municipio` | Neuquen_Capital, Plottier, Centenario, Senillosa |
| `Nombre del Documento` | Título completo del documento |
| `Número de Ordenanza` | Número y año (ej: 3558/2014) |
| `Fecha` | Fecha de sanción/publicación |
| `Vigencia` | Vigente / Derogada / A verificar |
| `FOS` | Factor de Ocupación de Suelo |
| `FOT` | Factor de Ocupación Total |
| `Retiros` | Distancias mínimas de retiro |
| `Altura Máxima` | Altura permitida en metros o pisos |
| `Zonificación` | Zonas aplicables |
| `Usos Permitidos` | Residencial, comercial, industrial, etc. |
| `Densidad` | Unidades habitacionales por hectárea |
| `Fuente Oficial` | URL o referencia de descarga |
| `Artículos Clave` | Artículos más consultados |
| `Trámites Involucrados` | Aprobación, recepción, etc. |
| `Requisitos de Planos` | Exigencias específicas de presentación |
| `Exigencias de Servicios` | Agua, luz, cloacas, gas |
| `Notas` | Observaciones adicionales |
| `Última Verificación` | Fecha de última revisión de vigencia |

---

## 🏛️ Municipios Prioritarios

| Municipio | Prioridad | Estado |
|-----------|-----------|--------|
| Neuquén Capital | Alta | Pendiente |
| Plottier | Alta | Pendiente |
| Centenario | Media | Pendiente |
| Senillosa | Baja | Pendiente |

---

## 📚 Documentación Adicional

- `docs/hoja-de-ruta-sistema-normativo.md`: Metodología completa en 8 fases
- `docs/notas-arquitectura-abierta.md`: Decisiones técnicas postergadas

---

## ⚠️ Reglas de Calidad

1. **No cargar documentos sin fuente oficial**
2. **No afirmar vigencia si no está verificada**
3. **No mezclar interpretación con texto normativo**
4. **Toda respuesta importante debe citar documento y artículo**
5. **Toda actualización debe dejar registro**

---

## 🎯 Objetivo del Repo

Que funcione como referencia viva para ordenar decisiones y avanzar sin improvisar ni sobrediseñar la solución demasiado pronto.

---

**Versión actual:** MVP en construcción  
**Última actualización:** 2026-04-02
