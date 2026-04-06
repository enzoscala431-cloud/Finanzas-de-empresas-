# Unidad IV — Administración Financiera de Largo Plazo
> Finanzas de Empresas 2025

---

## Índice
1. [Tasa de Descuento](#1-tasa-de-descuento)
2. [VAN — Valor Actual Neto](#2-van--valor-actual-neto)
3. [WACC](#3-wacc)
4. [Riesgo y Rentabilidad](#4-riesgo-y-rentabilidad)
5. [Portafolio y Diversificación](#5-portafolio-y-diversificación)
6. [Coeficiente Beta](#6-coeficiente-beta)
7. [Modelo CAPM](#7-modelo-capm)
8. [FCF y Método Indirecto](#8-fcf-y-método-indirecto)
9. [TIR y PRI](#9-tir-y-pri)
10. [Ejercicios Resueltos](#10-ejercicios-resueltos)

---

## 1. Tasa de Descuento

> La **tasa de descuento** es el precio que se paga por los fondos requeridos para una inversión. Representa la rentabilidad **mínima** que se le exige al proyecto según su riesgo.

```
Tasa de descuento = Costo de oportunidad + Prima de riesgo
```

### Principios clave

> *"El valor de $1 hoy es mayor al valor de $1 mañana"*

> *"El valor de $1 seguro es mayor al valor de $1 riesgoso"*

> *"Solo tiene sentido comparar activos de riesgo equivalente"*

---

## 2. VAN — Valor Actual Neto

El **VAN** trae al presente todos los flujos de caja del proyecto descontados por la tasa de descuento.

```
VAN = FCF₀ + FCF₁/(1+r)¹ + FCF₂/(1+r)² + ... + FCFₜ/(1+r)ᵀ + VT/(1+r)ᵀ
```

| Variable | Significado |
|---|---|
| `FCF₀` | Inversión inicial (generalmente negativa) |
| `FCFₜ` | Flujo de caja libre en el período t |
| `r` | Tasa de descuento (WACC) |
| `VT` | Valor terminal del proyecto |
| `T` | Número de períodos |

### Interpretación

| Resultado | Decisión |
|---|---|
| **VAN > 0** | El proyecto genera valor → **aceptar** |
| **VAN = 0** | Devuelve exactamente lo invertido → indiferente |
| **VAN < 0** | Destruye valor → **rechazar** |

---

## 3. WACC

> El **WACC** es el promedio ponderado del costo de todas las fuentes de financiamiento. Se usa como tasa de descuento del proyecto.

```
WACC = Kd × %D × (1 − tax) + Kac × %ac + Kap × %ap
```

| Variable | Significado |
|---|---|
| `Kd` | Costo de la deuda |
| `%D` | Proporción deuda / (Deuda + PN) |
| `(1 − tax)` | Escudo impositivo |
| `Kac` | Costo del capital propio (CAPM) |
| `Kap` | Costo del capital preferente |

### Costo real de la deuda

```
Costo real = Kd × (1 − tax)
```

**Ejemplo:** Kd = 11%, tax = 40% → Costo real = 6,6%

### Regla de decisión

```
Si VAN > 0 usando WACC → conviene
Si TIR > WACC → conviene
```

---

## 4. Riesgo y Rentabilidad

> **Riesgo** = variabilidad de los resultados respecto a lo esperado. Se mide con **desviación estándar (σ)** y **varianza (σ²)**.

### Los 4 cuadrantes

| | Bajo riesgo | Alto riesgo |
|---|---|---|
| **Alta rentabilidad** | Ideal — poco común | Acciones, startups |
| **Baja rentabilidad** | Bonos, plazo fijo | **El peor — evitar** |

---

## 5. Portafolio y Diversificación

### Tipos de riesgo

| Tipo | Descripción | ¿Se elimina? |
|---|---|---|
| **No sistemático** | Específico de empresa/sector | ✅ Con diversificación |
| **Sistemático** | Riesgo del mercado (COVID, crisis) | ❌ No se puede eliminar |

### Teoría de Markowitz

Combinar activos para lograr la mejor relación riesgo-rentabilidad. Existe un **portafolio de mínimo riesgo** que no es el 100% del activo más seguro, sino una combinación óptima.

### Línea de Mercado de Capitales (CML)

- Inversiones **sobre** la línea → superan al mercado → atractivas
- Inversiones **bajo** la línea → misma rentabilidad con más riesgo → no aceptables

---

## 6. Coeficiente Beta

> **Beta (β)** mide la sensibilidad de una acción frente a los cambios del mercado.

```
β = σᵢₘ / σ²ₘ
```

| Beta | Significado |
|---|---|
| **β = 1** | Se mueve igual que el mercado |
| **β > 1** | Más volátil → más riesgosa |
| **β < 1** | Menos volátil → más estable |
| **β = 0** | No se mueve con el mercado |
| **β < 0** | Se mueve al revés (oro, activos defensivos) |

---

## 7. Modelo CAPM

> Calcula la rentabilidad mínima que exigen los accionistas por el riesgo asumido.

```
Kcp = rf + β × (Erm − rf)

Con riesgo país:
Kcp = rf + β × (Erm − rf) + Riesgo País
```

| Variable | Significado |
|---|---|
| `rf` | Tasa libre de riesgo (bonos USA) |
| `β` | Coeficiente beta |
| `Erm` | Rentabilidad esperada del mercado |
| `Erm − rf` | Prima de riesgo del mercado |

**Ejemplo:** rf = 4%, β = 1,5, Erm = 10%
```
Kcp = 4% + 1,5 × (10% − 4%) = 13%
```

### Tasa libre de riesgo (rf)
- Sin riesgo de default
- Rendimiento esperado = rendimiento real
- Misma moneda y tratamiento inflacionario que el FCF
- Se usan bonos del gobierno USA → **es dato en el parcial**

---

## 8. FCF y Método Indirecto

### Principios del FCF
- Solo el flujo de efectivo real es relevante (no ganancias contables)
- Base incremental (los cambios, no el total)
- Incluir efectos derivados (venta del activo viejo)
- No olvidar necesidades de capital de trabajo
- **Ignorar costos hundidos** (irrecuperables)
- Incluir costos de oportunidad
- Consistencia inflacionaria (todo nominal o todo real)

### Método Indirecto

```
FCF = EBIT × (1 − tax)
    + Depreciación
    − ΔCapital de Trabajo
    − Inversiones operativas
```

> La depreciación se suma porque no es una salida real de efectivo.

---

## 9. TIR y PRI

### TIR — Tasa Interna de Retorno

> La TIR es la tasa que hace VAN = 0. Es la "tasa máxima que puedo usar sin perder plata".

```
TIR > WACC → conviene
TIR < WACC → no conviene
```

**Debilidades:** no sirve bien con flujos no convencionales, no considera la escala, puede haber múltiples TIR.

### PRI — Plazo de Recuperación

> ¿Cuántos años tardo en recuperar la inversión?

```
Aceptar si: PRI ≤ plazo máximo fijado
```

**Problemas:** no considera el valor del dinero en el tiempo, puede aceptar proyectos con VAN negativo.

### Comparación

| Criterio | Considera VDT | Fácil | Confiable |
|---|---|---|---|
| **VAN** | ✅ Sí | Medio | ✅ El mejor |
| **TIR** | ✅ Sí | Medio | Bueno |
| **PRI** | ❌ No | ✅ Muy fácil | Limitado |

---

## 10. Ejercicios Resueltos

### Ejercicio 1 — CAPM con y sin riesgo país

**Datos:** rf = 4%, β = 1,5, Erm = 10%, Riesgo país = 2%

```
Sin riesgo país: Kcp = 4% + 1,5 × 6% = 13%
Con riesgo país: Kcp = 4% + 1,5 × 6% + 2% = 15%
```

### Ejercicio 2 — WACC

**Datos:** Deuda $40.000 al 11% | Capital propio $60.000 | Kcp = 13% | tax = 40%

```
%D = 40% | %CP = 60%
WACC = 11% × 40% × 0,60 + 13% × 60% = 2,64% + 7,80% = 10,44%
```

### Ejercicio 3 — Escudo Fiscal

**Datos:** EBIT = $10.000 | Intereses = $4.400 | tax = 40%

```
Impuesto con deuda:  $5.600 × 40% = $2.240
Impuesto sin deuda:  $10.000 × 40% = $4.000
Ahorro fiscal = $1.760
Costo real deuda = $4.400 − $1.760 = $2.640 = 6,6% ✓
```

### Ejercicio 4 — VAN

**Datos:** Inversión = $50.000 | FCF años 1-3 = $20.000 | r = 10%

```
VAN = −50.000 + 20.000/1,10 + 20.000/1,10² + 20.000/1,10³
VAN = −50.000 + 18.182 + 16.529 + 15.026 = −$263

VAN < 0 → No conviene
```

---

*Resumen basado en los apuntes de la cátedra — Finanzas de Empresas 2025*
