# Unidad I — Introducción · Valor del Dinero en el Tiempo

> **Finanzas de Empresas · Ing. Industrial · UNCUYO**

---

## ¿Qué son las Finanzas de Empresas?

Disciplina que estudia cómo las empresas obtienen y administran sus recursos financieros para maximizar su valor. Se enfoca en tres decisiones fundamentales:

- **Decisión de inversión:** ¿En qué activos invertir?
- **Decisión de financiamiento:** ¿Cómo obtener los fondos necesarios?
- **Decisión de dividendos:** ¿Qué hacer con las ganancias?

---

## El Principio del Valor del Dinero en el Tiempo

> **Un peso hoy vale más que un peso mañana.**

¿Por qué? Porque el dinero disponible hoy puede invertirse y generar rendimientos. Este principio es la base de toda la matemática financiera.

### Conceptos clave

- **Valor Presente (VP):** Lo que vale hoy un flujo de dinero futuro.
- **Valor Futuro (VF):** Lo que valdrá en el futuro un dinero disponible hoy.
- **Tasa de interés (i):** El precio del dinero en el tiempo. Puede ser el costo de la deuda o la rentabilidad mínima exigida.
- **Período (n):** El número de períodos de tiempo considerados.

---

## Interés Simple vs. Interés Compuesto

### Interés Simple

El interés se calcula **siempre sobre el capital original**. No se acumula.

```
VF = VP × (1 + i × n)
```

| Variable | Significado |
|:---|:---|
| VF | Valor Futuro |
| VP | Valor Presente (capital inicial) |
| i | Tasa de interés por período |
| n | Número de períodos |

**Ejemplo:** $1.000 al 10% simple durante 3 años → VF = 1.000 × (1 + 0,10 × 3) = **$1.300**

---

### Interés Compuesto

El interés se calcula sobre el capital **más los intereses acumulados**. Los intereses generan intereses.

```
VF = VP × (1 + i)^n
```

**Ejemplo:** $1.000 al 10% compuesto durante 3 años → VF = 1.000 × (1,10)³ = **$1.331**

> La diferencia entre simple y compuesto crece exponencialmente con el tiempo. Por eso Einstein decía que el interés compuesto es "la octava maravilla del mundo".

---

## Valor Presente y Descuento

Para calcular cuánto vale hoy un pago futuro, se **descuenta** ese valor:

```
VP = VF / (1 + i)^n
```

**Ejemplo:** ¿Cuánto vale hoy recibir $1.331 en 3 años si la tasa es 10%?
VP = 1.331 / (1,10)³ = **$1.000**

---

## Tasas de Interés

### Tasa Nominal vs. Tasa Efectiva

| Concepto | Definición |
|:---|:---|
| **Tasa Nominal (TNA)** | Tasa anunciada, sin considerar la frecuencia de capitalización |
| **Tasa Efectiva (TEA)** | Tasa real que incorpora la capitalización en el período |

### Conversión de tasas

Si la tasa nominal es `i_nom` y se capitaliza `m` veces por año:

```
TEA = (1 + i_nom / m)^m − 1
```

**Ejemplo:** TNA del 12% capitalizable mensualmente:
TEA = (1 + 0,12/12)^12 − 1 = (1,01)^12 − 1 ≈ **12,68%**

### Tasa Real vs. Tasa Nominal (efecto inflación)

```
(1 + i_real) = (1 + i_nominal) / (1 + inflación)
```

---

## Anualidades

Una **anualidad** es una serie de pagos iguales realizados a intervalos regulares.

### Valor Presente de una Anualidad

```
VP = PMT × [ 1 − (1 + i)^−n ] / i
```

### Valor Futuro de una Anualidad

```
VF = PMT × [ (1 + i)^n − 1 ] / i
```

| Variable | Significado |
|:---|:---|
| PMT | Pago periódico constante |
| i | Tasa de interés por período |
| n | Número de períodos |

**Ejemplo:** Depósitos de $500 por mes durante 12 meses al 1% mensual:
VF = 500 × [(1,01)^12 − 1] / 0,01 = **$6.341,25**

---

## Perpetuidades

Una **perpetuidad** es una anualidad que dura para siempre.

```
VP = PMT / i
```

**Ejemplo:** Un bono que paga $100 por año indefinidamente, con tasa del 5%:
VP = 100 / 0,05 = **$2.000**

---

## Aplicaciones prácticas

### Préstamos y Amortización

Cada cuota de un préstamo tiene dos componentes:

```
Cuota = Intereses del período + Amortización del capital
```

La cuota fija de un préstamo se calcula como:

```
PMT = VP × i / [ 1 − (1 + i)^−n ]
```
---

## Resumen de Fórmulas Clave

| Fórmula | Expresión |
|:---|:---|
| Valor Futuro (simple) | VF = VP × (1 + i × n) |
| Valor Futuro (compuesto) | VF = VP × (1 + i)^n |
| Valor Presente | VP = VF / (1 + i)^n |
| Tasa Efectiva Anual | TEA = (1 + i_nom/m)^m − 1 |
| Tasa Real | (1 + i_real) = (1 + i_nom) / (1 + π) |
| VP Anualidad | VP = PMT × [1 − (1+i)^−n] / i |
| VF Anualidad | VF = PMT × [(1+i)^n − 1] / i |
| Perpetuidad | VP = PMT / i |
| Cuota préstamo | PMT = VP × i / [1 − (1+i)^−n] |

---

*Resumen  — UNCUYO 2025*


