# EXPLICACIÓN DETALLADA: DISEÑO 3+3 PARA ESCALADA DE DOSIS
## Protocolo rAMPV-4 en Cáncer Colorectal Metastásico

---

## 1. ¿QUÉ ES EL DISEÑO 3+3?

El **diseño 3+3** es el método estándar más utilizado en ensayos clínicos de **Fase I** oncológicos para determinar la **Dosis Máxima Tolerada (MTD)** de un nuevo fármaco o terapia.

### Principios Básicos:

- **3 pacientes iniciales** por cohorte (dosis)
- **Reglas de escalada/parada simples** basadas en toxicidad limitante de dosis (DLT)
- **Seguridad**: No expone demasiados pacientes a dosis tóxicas
- **Eficiencia**: Permite identificar MTD con ~20-30 pacientes totales
- **Flexible**: Permite adaptaciones según datos observados

---

## 2. ALGORITMO DEL DISEÑO 3+3

### El flujo de decisiones es el siguiente:

```
┌─────────────────────────────────────────────────────────────────┐
│               COMIENZAN 3 PACIENTES EN COHORTE N                │
│                    (Dosis X = 1×10¹⁰ vp)                        │
└─────────────────────────────────────────────────────────────────┘
                            │
                            ▼
        ┌─────────────────────────────────────────┐
        │   OBSERVACIÓN 28 DÍAS (DLT Window)      │
        │   ¿Cuántos de 3 pacientes tienen DLT?  │
        └─────────────────────────────────────────┘
                            │
        ┌───────────────────┼───────────────────┐
        │                   │                   │
        ▼                   ▼                   ▼
    0 DLTs             1 DLT              2-3 DLTs
                                          (≥2 de 3)
        │                   │                   │
        │                   │                   │
    ┌───▼────┐          ┌───▼────┐        ┌────▼──────┐
    │ESCALADA│          │EXPANDIR│        │DETENER Y  │
    │A DOSIS │          │COHORTE │        │RETROTRAER │
    │SUPERIOR│          │A 6     │        │DOSIS      │
    │(+1)    │          │PTES    │        │           │
    └────────┘          └────────┘        └───────────┘
        │                   │                   │
        ▼                   ▼                   ▼
    COHORTE         ESPERAR ANÁLISIS    DOSIS ANTERIOR
    SIGUIENTE       DE 6 PACIENTES      = MTD FINAL
                            │
                    ┌───────┴───────┐
                    │               │
                    ▼               ▼
                ≤1 DLT          ≥2 DLTs
                    │               │
                ESCALADA        DETENER
                CONTINÚA        MTD ENCONTRADA
```

---

## 3. DESGLOSE PASO A PASO DEL PROTOCOLO rAMPV-4

### **Escenario 1: Escalada Rápida (Sin Toxicidad)**

```
COHORTE 1: DOSIS 1.0 × 10¹⁰ vp (3 inyecciones)
│
├─ Paciente 1: SIN DLT ✓ (solo fiebre leve <24h)
├─ Paciente 2: SIN DLT ✓ (dolor local controlado)
└─ Paciente 3: SIN DLT ✓ (asintomático)

RESULTADO: 0 de 3 con DLT
DECISIÓN: ✓ ESCALADA A COHORTE 2 (Dosis 2)

═══════════════════════════════════════════════════════════

COHORTE 2: DOSIS 5.0 × 10¹⁰ vp (3 inyecciones) 
│
├─ Paciente 4: SIN DLT ✓
├─ Paciente 5: SIN DLT ✓
└─ Paciente 6: SIN DLT ✓

RESULTADO: 0 de 3 con DLT
DECISIÓN: ✓ ESCALADA A COHORTE 3 (Dosis 3)

═══════════════════════════════════════════════════════════

COHORTE 3: DOSIS 1.0 × 10¹¹ vp (3 inyecciones)
│
├─ Paciente 7: SIN DLT ✓
├─ Paciente 8: SIN DLT ✓
└─ Paciente 9: SIN DLT ✓

RESULTADO: 0 de 3 con DLT
DECISIÓN: ✓ ESCALADA A COHORTE 4 (Dosis 4)
```

---

### **Escenario 2: Toxicidad Detectada → EXPANSIÓN A 6 PACIENTES**

```
COHORTE 3: DOSIS 1.0 × 10¹¹ vp (3 inyecciones)
│
├─ Paciente 7:  SIN DLT ✓
├─ Paciente 8:  SIN DLT ✓
└─ Paciente 9:  ✓ DLT DETECTADO ❌
                 (Elevación AST/ALT >5× LSN que no reversa)

RESULTADO: 1 de 3 con DLT
DECISIÓN: ⚠️ EXPANDIR COHORTE DE 3 → 6 PACIENTES

Esperamos a que 3 pacientes adicionales se complete la evaluación:

├─ Paciente 10: SIN DLT ✓
├─ Paciente 11: SIN DLT ✓
└─ Paciente 12: SIN DLT ✓

RESULTADO FINAL DE 6: 1 de 6 con DLT (16.7%)
DECISIÓN: ✓ ESCALADA A COHORTE 4 (porque ≤1 de 6 = TOLERABLE)

═══════════════════════════════════════════════════════════

COHORTE 4: DOSIS 2.5 × 10¹¹ vp (2-3 inyecciones)
│
├─ Paciente 13: SIN DLT ✓
├─ Paciente 14: ✓ DLT DETECTADO ❌ (hemorragia hepática)
└─ Paciente 15: ✓ DLT DETECTADO ❌ (elevación bilirrubina severa)

RESULTADO: 2 de 3 con DLT (66.7%)
DECISIÓN: ❌ PARADA INMEDIATA - MTD ENCONTRADA

→ LA DOSIS MTD = COHORTE 3 (1.0 × 10¹¹ vp)
```

---

### **Escenario 3: Toxicidad Severa → ESCALADA RETROACTIVA**

```
COHORTE 4: DOSIS 2.5 × 10¹¹ vp (2-3 inyecciones)
│
├─ Paciente 13: ✓ DLT DETECTADO ❌ (perforación colónica)
├─ Paciente 14: ✓ DLT DETECTADO ❌ (sepsis por inyección)
└─ Paciente 15: SIN DLT ✓

RESULTADO: 2 de 3 con DLT
DECISIÓN: ⚠️ EXPANDIR A 6 para confirmar

├─ Paciente 16: ✓ DLT DETECTADO ❌
├─ Paciente 17: SIN DLT ✓
└─ Paciente 18: SIN DLT ✓

RESULTADO FINAL: 3 de 6 con DLT (50%)
DECISIÓN: ❌ PARADA - ESTA DOSIS ES MUY TÓXICA

→ MTD = DOSIS ANTERIOR = COHORTE 3 (1.0 × 10¹¹ vp)
```

---

## 4. TABLA DE DECISIONES DEL DISEÑO 3+3

| # Pacientes con DLT | Acción | Justificación |
|---|---|---|
| **0 de 3** | ✓ ESCALADA a dosis siguiente | Dosis bien tolerada → probar dosis mayor |
| **1 de 3** | ⚠️ EXPANDIR a 6 pacientes | Resultado ambiguo → necesita más datos |
| **≤1 de 6** (expansión) | ✓ ESCALADA a dosis siguiente | Dosis tolerable incluso con 1 DLT |
| **≥2 de 6** (expansión) | ❌ PARADA - Dosis anterior = MTD | Dosis inaceptablemente tóxica |
| **2-3 de 3** | ❌ PARADA INMEDIATA - Dosis anterior = MTD | Dosis claramente tóxica |

---

## 5. APLICACIÓN ESPECÍFICA AL PROTOCOLO rAMPV-4

### Cohortes Planeadas:

```
COHORTE 1:  1.0 × 10¹⁰ vp × 3 inyecciones = 3.0 × 10¹⁰ vp total
COHORTE 2:  5.0 × 10¹⁰ vp × 3 inyecciones = 1.5 × 10¹¹ vp total
COHORTE 3:  1.0 × 10¹¹ vp × 3 inyecciones = 3.0 × 10¹¹ vp total
COHORTE 4:  2.5 × 10¹¹ vp × 2-3 inyecciones = 5.0-7.5 × 10¹¹ vp total
COHORTE 5:  5.0 × 10¹¹ vp × 2 inyecciones = 1.0 × 10¹² vp total
COHORTE 6:  (Potencial) 10¹² vp × 2 inyecciones = 2.0 × 10¹² vp total (si tolerado)
```

### Cronología Esperada:

```
TIMELINE APROXIMADO:

MES 1-2:   COHORTE 1 (3 ptes) + observación 28 días = 3 ptes totales
MES 2-3:   COHORTE 2 (3 ptes) + observación 28 días = 6 ptes totales
MES 3-4:   COHORTE 3 (3 ptes) + observación 28 días = 9 ptes totales
           [¿Expansión a 6? → 3-4 meses adicionales]
MES 4-6:   COHORTE 4 (3 ptes) + observación 28 días = 12-15 ptes totales
           [¿Expansión a 6? → 3-4 meses adicionales]
MES 6-8:   COHORTE 5 (3 ptes) + observación 28 días = 15-21 ptes totales
MES 8-10:  EXPANSIÓN FINAL (6-9 ptes a MTD) = 21-30 ptes totales

DURACIÓN TOTAL: 12-18 MESES (dependiendo de patrón de DLT)
```

---

## 6. VENTAJAS DEL DISEÑO 3+3

| Ventaja | Descripción |
|---|---|
| **Seguridad** | Exposición limitada a dosis tóxicas desconocidas; máximo 6 pacientes por cohorte |
| **Eficiencia** | Identifica MTD con ~20-30 pacientes (vs 100+ con métodos tradicionales) |
| **Simplicidad** | Reglas de decisión claras y fáciles de aplicar |
| **Aceptación Regulatoria** | Estándar de facto aceptado por FDA/EMA para estudios oncológicos |
| **Adaptabilidad** | Pueden modificarse incrementos de dosis según hallazgos |
| **Mecanismo de Parada** | Protege contra escalada a dosis peligrosamente altas |

---

## 7. LIMITACIONES DEL DISEÑO 3+3

| Limitación | Implicación |
|---|---|
| **MTD ≠ Dosis Óptima** | MTD es máxima tolerable, pero podría no ser más efectiva que dosis menor |
| **No evalúa eficacia** | Fase I solo evalúa seguridad; eficacia se estudia en Fase II |
| **Dependencia de DLT** | Si definición de DLT es pobre, todo el estudio es comprometido |
| **Tamaño muestral pequeño** | 20-30 pacientes es insuficiente para eventos raros |
| **Factores históricos** | Secuencia de DLTs puede afectar decisiones (ej: primer DLT en paciente 3 vs 1) |

---

## 8. CRITERIOS DE DLT ESPECÍFICOS EN rAMPV-4

Para que el diseño 3+3 funcione correctamente, deben definirse claramente qué es "toxicidad limitante":

### **SÍ es DLT:**

- ✓ Hemorragia intrahepática ≥Grade 3 requiriendo transfusión
- ✓ AST/ALT >5× LSN en 48h sin causa alternativa
- ✓ Bilirrubina >3× LSN no revertida en 7 días
- ✓ Perforación colónica documentada
- ✓ Cualquier toxicidad Grade ≥3 no manejable
- ✓ Neutropenia Grado 4 ≥7 días
- ✓ Fiebre >39°C durando >3 días

### **NO es DLT:**

- ✗ Fiebre <38.5°C controlada con antipiréticos
- ✗ AST/ALT 1-3× LSN reversible en 7-14 días
- ✗ Dolor local Grado 1-2 manejable con analgésicos
- ✗ Náusea controlada con anti-eméticos
- ✗ Citocinas elevadas SIN síntomas sistémicos

---

## 9. EJEMPLO NUMÉRICO COMPLETO: COHORTE 3 CON EXPANSIÓN

Supongamos que en Cohorte 3 (1×10¹¹ vp) observamos:

### **Fase 1: Primeros 3 pacientes**

| Paciente | Síntomas Día 1-7 | Síntomas Día 28 | ¿DLT? |
|---|---|---|---|
| P7 | Fiebre 38°C × 2d, dolor local | ALT 2× LSN (normaliza) | ✓ NO |
| P8 | Fiebre <38°C, sin síntomas | AST 1.5× LSN (normal) | ✓ NO |
| P9 | Fiebre 39.2°C × 5d, deterioro | AST/ALT >5× LSN persiste | ✗ **SÍ DLT** |

**Resultado:** 1 de 3 = 33.3% tasa DLT
**Decisión:** Ambiguo → **EXPANDIR A 6**

---

### **Fase 2: Siguientes 3 pacientes (total 6)**

| Paciente | Síntomas Día 1-7 | Síntomas Día 28 | ¿DLT? |
|---|---|---|---|
| P10 | Fiebre leve, controlada | AST/ALT 1-2× LSN | ✓ NO |
| P11 | Dolor local Grado 2 | Hemoglobina estable | ✓ NO |
| P12 | Sin síntomas relevantes | Laboratorio normal | ✓ NO |

**Resultado Final de 6:** 1 de 6 = 16.7% tasa DLT
**Decisión:** ✓ **ESCALADA A COHORTE 4** (porque ≤1 de 6 es aceptable)

---

## 10. CASOS DE PARADA TEMPRANA

El protocolo puede detenerse en cualquier momento si:

1. **Dos cohorts consecutivos muestran ≥2 DLTs de 6:** Criterio formal de parada
2. **DLT inaceptable:** Ej: muerte, complicación quirúrgica en cohort temprano
3. **Falta de seguridad:** Si primeros 3-6 pacientes all get severe toxicidad
4. **Pérdida de reclutamiento:** Si es imposible enrolar 3+ pacientes por cohorte
5. **Cambio de contexto:** Ej: si emerge nuevo fármaco más efectivo

---

## 11. ANÁLISIS ESTADÍSTICO FINAL

Una vez identificado MTD (o RP2D después de expansión), se reporta:

```
TABLA FINAL DE RESULTADOS:

Dosis (vp)          N Ptes    DLTs    Tasa DLT    Status
─────────────────────────────────────────────────────────
1.0 × 10¹⁰          3         0       0%          Escalada
5.0 × 10¹⁰          3         0       0%          Escalada
1.0 × 10¹¹          6         1       16.7%       Escalada
2.5 × 10¹¹          6         3       50%         MTD Found
─────────────────────────────────────────────────────────

MTD = 1.0 × 10¹¹ vp × 3 inyecciones (3×10¹¹ vp total)
RP2D = 1.0 × 10¹¹ vp × 3 inyecciones (recomendado para Fase IIb)

Expansion Cohort (Dosis RP2D):
N Adicional = 9 pacientes
Confirmación de seguridad y farmacodinámica
```

---

## 12. TRANSICIÓN A FASE IIb

Después de completar Fase I con diseño 3+3:

1. **MTD/RP2D identificada:** ✓ Dosis segura para uso
2. **Farmacodinámica caracterizada:** Replicación viral, respuesta inmune
3. **Perfil de AE documentado:** Qué esperar, cómo manejar
4. **Datos viabilidad:** Confirmación que administración es factible

**Fase IIb usará:**
- Dosis = RP2D establecida
- N = 25-50 pacientes
- Objetivo: Evaluar EFICACIA (% respuesta, supervivencia)
- Diseño: Posiblemente comparativo vs control

---

## RESUMEN: FLUJO COMPLETO 3+3 EN rAMPV-4

```
┌──────────────────────────────────────────────────────────────┐
│                    DISEÑO 3+3 COMPLETO                        │
│              rAMPV-4 Cáncer Colorectal Metastásico            │
└──────────────────────────────────────────────────────────────┘

FASE DE ESCALADA (Cohorts 1-5/6):
│
├─ COHORTE 1: 1×10¹⁰ vp × 3 inj [3 ptes] → 0 DLT → Escalada
├─ COHORTE 2: 5×10¹⁰ vp × 3 inj [3 ptes] → 0 DLT → Escalada
├─ COHORTE 3: 1×10¹¹ vp × 3 inj [3→6 ptes] → 1 DLT → Escalada
├─ COHORTE 4: 2.5×10¹¹ vp × 2-3 [6 ptes] → 3 DLT → PARADA
│
└─ ✓ MTD ENCONTRADA = COHORTE 3 (1×10¹¹ vp)

FASE DE EXPANSIÓN:
│
└─ COHORTE EXPANSIÓN: 1×10¹¹ vp × 3 [6-9 ptes adicionales]
                      → Confirmación seguridad
                      → Caracterización farmacodinámica
                      → RP2D recomendado para Fase IIb

RESULTADO FINAL:
│
└─ N Total = 21-34 pacientes
   Duración = 12-18 meses
   RP2D = 1×10¹¹ vp × 3 inyecciones (3×10¹¹ vp total)
```

---

## REFERENCIAS Y LECTURAS RECOMENDADAS

1. O'Quigley J, et al. Continual Reassessment Method: A Practical Design for Phase I Clinical Trials in Cancer. Biometrics. 1990.

2. Storer BE. Design and Analysis of Phase I Clinical Trials. Biometrics. 1989;45(3):925-937.

3. ICH Guidelines for Phase I Dose Escalation Studies. FDA/EMA Guidance Documents.

4. FDA Guidance: Dose-Escalation Study Design. Center for Drug Evaluation and Research. 2020.

5. ASCO Guidelines: Phase I Trial Design and Conduct. Journal of Clinical Oncology. 2020.

---

**Documento preparado:** 13 de enero de 2026
**Propósito:** Educación sobre diseño 3+3 para protocolo rAMPV-4
**Nivel:** Intermedio-Avanzado (para investigadores clínicos, regulatorios, DSMB)
