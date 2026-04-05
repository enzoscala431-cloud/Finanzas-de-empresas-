# Unidad 1 Introducción — Valor del Dinero en el Tiempo
> Finanzas de Empresas 2025

---

## Índice
1. [Concepto de Interés](#1-concepto-de-interés)
2. [Interés Simple](#2-interés-simple)
3. [Interés Compuesto](#3-interés-compuesto)
4. [Tasas Financieras: TNA, TEA y CFT](#4-tasas-financieras-tna-tea-y-cft)
5. [Operación de Descuento](#5-operación-de-descuento)
6. [Valor Presente](#6-valor-presente)
7. [Anualidad](#7-anualidad)
8. [Perpetuidad](#8-perpetuidad)
9. [Sistemas de Amortización](#9-sistemas-de-amortización)
10. [Meses de Gracia](#10-meses-de-gracia)
11. [Ejercicios Resueltos](#11-ejercicios-resueltos)

---

## 1. Concepto de Interés

> El interés es el **extra** que uno tiene que pagar o cobrar por usar dinero (o cualquier bien) durante un cierto tiempo.

Pensalo así: el interés es como **alquilar plata**. Si alguien te presta $10.000, al final del período le devolvés los $10.000 más una tarifa = el interés.

**Dos principios fundamentales de esta unidad:**

> *"El valor de $1 hoy es mayor al valor de $1 mañana"*

> *"El valor de $1 seguro es mayor al valor de $1 riesgoso"*

Esto se debe a dos razones:
- **Costo de oportunidad** — si tenés la plata hoy, podés invertirla y hacerla crecer.
- **Riesgo** — cuanto más tiempo pasa, más incertidumbre hay sobre si vas a cobrar.

---

## 2. Interés Simple

Los intereses generados durante toda la inversión se calculan **siempre sobre el capital inicial**. Los intereses que se acumulan no pasan a formar parte de la deuda.

### Fórmulas

```
Is = Po × i × n

Vf = Po + Is

Vf = Po × [1 + i × n]
```

| Variable | Significado |
|---|---|
| `Is` | Interés simple generado |
| `Vf` | Valor futuro (lo que terminás pagando) |
| `Po` | Principal / valor actual (capital inicial) |
| `i` | Tasa de interés del período |
| `n` | Número de períodos |

### Ejemplo

Préstamo de $10.000 a 5 años con tasa simple del 10% anual:

| Año | Capital base | Interés del año | Deuda acumulada |
|---|---|---|---|
| 1 | $10.000 | $1.000 | $11.000 |
| 2 | $10.000 | $1.000 | $12.000 |
| 3 | $10.000 | $1.000 | $13.000 |
| 4 | $10.000 | $1.000 | $14.000 |
| 5 | $10.000 | $1.000 | **$15.000** |

> Siempre se calcula sobre los $10.000 originales, nunca sobre la deuda acumulada.

---

## 3. Interés Compuesto

Los intereses generados **se suman al capital** y a partir de ese momento también generan intereses. Es decir, se pagan intereses sobre intereses.

> ⚠️ Pagar los intereses no convierte al sistema en simple. Lo que cambia es que al pagar evitás que se sumen al capital, pero la fórmula sigue siendo compuesta.

### Capitalización

**Capitalizar** = sumar los intereses al capital para que luego esos intereses también generen intereses.

La capitalización puede ser: mensual, trimestral, semestral, anual, diaria, o incluso continua (segundo a segundo).

### Fórmula

```
Vf = Po × (1 + i/m)^(m×n)
```

| Variable | Significado |
|---|---|
| `Vf` | Valor futuro |
| `Po` | Principal / valor actual |
| `i` | Tasa de interés nominal del período |
| `n` | Número de períodos |
| `m` | Número de capitalizaciones por período |

### Comparación Simple vs. Compuesto

| Característica | Interés Simple | Interés Compuesto |
|---|---|---|
| Base de cálculo | Siempre el capital inicial | Capital + intereses acumulados |
| Crecimiento | Lineal | Exponencial |
| Uso en la práctica | Menos común, más fácil | El más usado |
| Conviene al deudor | A largo plazo | A corto plazo |

---

## 4. Tasas Financieras: TNA, TEA y CFT

### Tasa Nominal Anual (TNA)

- Es un **valor de referencia** para las operaciones financieras.
- Se usa solo como base del cálculo, **no representa la tasa real** que pagás.
- Corresponde al interés compuesto.
- *Ej: un banco ofrece TNA 12% con capitalización mensual → eso NO significa que ganás 12% real en el año.*

### Tasa Efectiva Anual (TEA)

- Es la tasa **real** que efectivamente ganás o pagás en un año cuando los intereses se capitalizan más de una vez.
- Siempre es **mayor que la TNA** (a más capitalizaciones, mayor diferencia).

```
TEA = (1 + TNA/m)^m - 1
```

**Ejemplo:** TNA = 12% con capitalización mensual (m = 12):
```
TEA = (1 + 0,12/12)^12 - 1 = 12,68%
```

> Aunque la TNA dice 12%, en realidad pagás 12,68% efectivo anual.

### Costo Financiero Total (CFT)

- Es la tasa **más completa y realista** al tomar un préstamo.
- Se obtiene sumando a la TEA todos los cargos asociados: comisiones, seguros, gastos administrativos, etc.
- Se expresa como tasa efectiva anual.

```
CFT = TEA + comisiones + seguros + gastos administrativos + ...
```

### Resumen comparativo

| Tasa | Incluye | Uso |
|---|---|---|
| **TNA** | Solo interés nominal | Base de cálculo |
| **TEA** | Efecto de la capitalización | Tasa real anual |
| **CFT** | TEA + todos los cargos | Comparar préstamos realmente |

> Para comparar dos préstamos, siempre hay que mirar el **CFT**, no la TNA.

---

## 5. Operación de Descuento

> ⚠️ *La pasamos rápido — solo interesa saber qué es.*

Es un instrumento financiero a **corto plazo** donde una entidad financiera te **anticipa** el importe de un crédito (cheque, pagaré, factura) que todavía no venció.

**¿Cómo funciona?**
- Tenés un cheque que vence en 60 días pero necesitás la plata ahora.
- Se lo das al banco → el banco te da la plata hoy.
- El banco después le cobra al que emitió el cheque.
- El banco te da **menos** de lo que dice el cheque (se queda con intereses y comisiones).
- Si el deudor no paga → **vos** le tenés que devolver la plata al banco (no el banco asume el riesgo).

### Fórmula

```
VA = VN × (1 - c - n_días × t_desc) - G
```

| Variable | Significado |
|---|---|
| `VA` | Valor actual (plata que recibís) |
| `VN` | Valor nominal del crédito |
| `c` | Comisiones variables |
| `n` | Número de días hasta el vencimiento |
| `t` | Tasa nominal de operación |
| `G` | Gastos varios |

---

## 6. Valor Presente

> **¿Cuánto vale hoy una cantidad de dinero que voy a recibir en el futuro?**

Cuanto más lejos esté el dinero en el tiempo, **menos vale hoy**, porque podrías invertir ese dinero ahora y hacerlo crecer.

### Fórmula general

```
VP = Σ [ Cj / (1 + i)^j ]    para j = 1 hasta n
```

| Variable | Significado |
|---|---|
| `Cj` | Valor del pago en el período j |
| `i` | Tasa de interés o descuento |
| `(1+i)^j` | Factor de descuento para el período j |

### Ejemplo

Te prometen 3 pagos de $1.000 en los próximos 3 años. Tasa: 10% anual.

```
VP = 1.000/1,10 + 1.000/1,10² + 1.000/1,10³
VP = 909 + 826 + 751
VP = $2.486
```

> Los $3.000 que vas a recibir en el futuro hoy solo valen **$2.486**, porque perdés la oportunidad de invertir esa plata durante ese tiempo.

---

## 7. Anualidad

Es una serie de **pagos o cobros iguales** que ocurren durante un número específico de períodos.

### Características
- Pagos siempre del **mismo monto**
- Durante **n períodos** fijos
- Con una **tasa de interés** aplicada
- En la anualidad ordinaria, los pagos ocurren al **final** de cada período

### Fórmula del Valor Presente

```
VP = A × [ (1+i)^n - 1 ] / [ i × (1+i)^n ]
```

Donde `A` (o `C`) es el monto fijo de cada cuota.

> Es mucho más práctica que sumar el VP de cada pago individualmente, especialmente cuando hay muchos períodos.

### Ejemplo

Mismos datos que antes: 3 pagos de $1.000, tasa 10%:
```
VP = 1.000 × [(1,10)³ - 1] / [0,10 × (1,10)³]
VP = 1.000 × [1,331 - 1] / [0,10 × 1,331]
VP = 1.000 × 0,331 / 0,1331
VP = $2.486  ✓  (mismo resultado que la sumatoria)
```

---

## 8. Perpetuidad

Una corriente de pagos que se extiende **por siempre** (n → ∞). Es como una anualidad infinita.

- Se usa para proyectos de muy largo plazo donde no podés generar el dinero a corto plazo.
- *Ej: pagar el mantenimiento de un parque para siempre.*
- No es muy común en la práctica.

### Fórmula

```
VP = C / (i - g)
```

| Variable | Significado |
|---|---|
| `C` | Pago periódico |
| `i` | Tasa de descuento |
| `g` | Tasa de crecimiento de los pagos (si los pagos son constantes, g = 0) |

---

## 9. Sistemas de Amortización

> **Amortización** = proceso de devolver un préstamo en partes a lo largo del tiempo.

Cada cuota se compone de:
- **Amortización** → devuelve parte del capital prestado → va al **Estado Patrimonial**
- **Interés** → el costo de usar ese dinero → va al **Estado de Resultados** (es deducible del impuesto a las ganancias)

Existen **3 sistemas:**

---

### 9.1 Sistema Francés

- **Cuota constante** (siempre la misma, mientras la tasa sea fija)
- El interés se calcula sobre el saldo pendiente → va disminuyendo con el tiempo
- La amortización va aumentando para compensar y mantener la cuota constante
- Los primeros meses pagás casi todo de interés y poco capital

```
Cuota pura = Amortización + Interés = CONSTANTE
```

**Cómo resolverlo en Excel:**
1. Colocar el Valor Actual
2. Calcular la tasa mensual (si dan anual: ÷ 12)
3. Calcular la cuota: `-PAGO(tasa; períodos; VA)`
4. Calcular el interés: `saldo anterior × tasa`
5. Calcular la amortización: `cuota - interés`
6. Nuevo saldo: `saldo anterior - amortización`

**Ventaja:** cuota predecible, fácil de planificar.  
**Desventaja:** al principio casi no bajás capital → si cancelás antes, no te ahorrás tanto.

| Período | Cuota | Interés | Amortización | Saldo |
|---|---|---|---|---|
| 1 | $X | Alto | Bajo | ↓ poco |
| ... | $X | ↓ | ↑ | ↓ |
| n | $X | Bajo | Alto | $0 |

---

### 9.2 Sistema Alemán

- **Amortización fija** (siempre la misma porción de capital)
- Interés **decreciente** (se calcula sobre el saldo que baja mes a mes)
- **Cuota decreciente** (capital fijo + interés que baja = cuota que baja)
- En la mitad del período debés exactamente la **mitad** del préstamo

```
Amortización = VA / n  (constante)
Interés = saldo × tasa  (decreciente)
Cuota = Amortización + Interés  (decreciente)
```

**Cómo resolverlo:**
1. Colocar el Valor Actual
2. Amortización = VA / nro de períodos (constante, fijar con $)
3. Interés = saldo × tasa (varía)
4. Cuota alemana = amortización + interés
5. Sumar IVA y seguro si corresponde
6. Nuevo saldo = saldo anterior - amortización

**Ventaja:** ideal si pensás cancelar antes → al tener amortización constante, reducís capital rápido.  
**Desventaja:** la primera cuota es muy alta.

---

### 9.3 Sistema Americano

- Durante todo el período **solo pagás intereses**
- El **capital se paga todo junto al final**
- El interés es constante (siempre sobre el saldo inicial, que no cambia)
- También podés no pagar los intereses → se capitalizan
- Es el **menos usado** para préstamos personales

**Cómo resolverlo:**
1. Calcular el interés mensual (constante) y prolongar
2. El saldo de la deuda es igual en todos los períodos (nunca baja hasta el final)
3. En el último mes: sumar toda la amortización → saldo = 0

### Comparación de los 3 sistemas

| Característica | Francés | Alemán | Americano |
|---|---|---|---|
| Cuota | Constante | Decreciente | Solo interés + capital al final |
| Amortización | Creciente | Constante | Todo al final |
| Interés | Decreciente | Decreciente | Constante |
| Primera cuota | Media | **La más alta** | La más baja |
| Saldo a mitad del período | Más de la mitad | Exactamente la mitad | Capital completo |
| Conveniente para | Cuota fija predecible | Cancelar antes de tiempo | Inversiones que generan flujo al final |

---

## 10. Meses de Gracia

Son un **período inicial** del préstamo donde el deudor no está obligado a pagar la cuota completa. Se da al principio como ayuda para acomodarse financieramente.

- Se pueden aplicar a **cualquier sistema** de amortización
- Hay **dos tipos:**

### Gracia Parcial
- Solo pagás los **intereses** del período
- No amortizás nada del capital
- El saldo inicial queda igual
- Al terminar la gracia, empezás a pagar como si recién comenzara el plan
- Los intereses se calculan sobre el capital inicial

```
Cuota durante gracia parcial = saldo × tasa  (solo interés)
```

**En Excel:** la cuota normal se calcula con `n - meses de gracia` períodos.  
**A mano:** se usa siempre `n` completo.

### Gracia Total
- **No pagás nada** — ni capital ni intereses
- Los intereses no pagados se **capitalizan** (se suman a la deuda)
- Terminás debiendo más al final de la gracia
- La cuota posterior se calcula sobre el nuevo saldo (mayor al original)

```
Nuevo saldo = saldo original × (1 + i)^meses_de_gracia
```

### Resumen

| | Gracia Parcial | Gracia Total |
|---|---|---|
| ¿Qué pagás? | Solo intereses | Nada |
| ¿Cambia el saldo? | No | Sí (aumenta) |
| ¿Conviene más? | Sí (menos intereses totales) | No (capitalizan) |

---

## 11. Ejercicios Resueltos

---

### Ejercicio 1 — Interés Simple vs. Compuesto

**Datos:**
- Préstamo: $10.000
- Interés compuesto: 10% anual
- Valor final compuesto a 5 años: $16.105
- Pregunta: ¿qué tasa simple da el mismo resultado?

**Resolución:**

**Paso 1 — Calcular el interés total:**
```
Is = Vf - Po = $16.105 - $10.000 = $6.105
```

**Paso 2 — Despejar la tasa simple:**
```
Is = Po × i × n
i = Is / (n × Po)
i = $6.105 / (5 × $10.000)
i = 0,1221 = 12,21% anual
```

**Conclusión:** con interés compuesto alcanza el 10% anual, pero con interés simple necesitás el **12,21% anual** para llegar al mismo valor final. Esto demuestra el efecto del interés sobre interés del sistema compuesto.

---

### Ejercicio 2 — TNA a TEA

**Datos:**
- TNA = 12% anual
- Capitalización mensual (m = 12)

**Resolución:**
```
TEA = (1 + TNA/m)^m - 1
TEA = (1 + 0,12/12)^12 - 1
TEA = (1 + 0,01)^12 - 1
TEA = 1,1268 - 1
TEA = 0,1268 = 12,68%
```

**Conclusión:** aunque el banco anuncia una TNA del 12%, la tasa efectiva real es **12,68%** por efecto de la capitalización mensual.

---

### Ejercicio 3 — Valor Presente

**Datos:**
- 3 pagos anuales de $1.000
- Tasa de descuento: 10% anual

**Resolución:**
```
VP = 1.000/(1,10)¹ + 1.000/(1,10)² + 1.000/(1,10)³
VP = 909,09 + 826,45 + 751,31
VP = $2.486,85
```

**Con fórmula de anualidad:**
```
VP = 1.000 × [(1,10)³ - 1] / [0,10 × (1,10)³]
VP = 1.000 × [0,331] / [0,1331]
VP = $2.486,85  ✓
```

**Conclusión:** los $3.000 futuros hoy solo valen **$2.487** aproximadamente.

---

### Ejercicio 4 — Sistema Francés con Gracia Parcial

**Datos:**
- Préstamo: $15.000
- TNAV: 15% anual → tasa mensual = 15%/12 = 1,25%
- Plazo: 36 meses
- 2 meses de gracia parcial

**Resolución:**

**Meses de gracia (mes 1 y 2):**
```
Interés = $15.000 × 1,25% = $187,50
Amortización = $0
Saldo = $15.000 (no cambia)
```

**A partir del mes 3 (34 cuotas restantes en Excel, 36 a mano):**
```
Cuota = -PAGO(1,25%; 34; 15.000)  → calcular con calculadora
```
La cuota es constante. El interés va bajando período a período y la amortización va subiendo.

---

### Ejercicio 5 — Sistema Francés con Gracia Total

**Datos:** mismos que el ejercicio anterior pero con **gracia total** (2 meses).

**Durante los 2 meses de gracia:**
```
No se paga nada.
Los intereses se capitalizan:
Nuevo saldo = $15.000 × (1 + 0,0125)² = $15.000 × 1,02516 = $15.377,34
```

**A partir del mes 3:**
La cuota se calcula sobre el **nuevo saldo** de $15.377,34 en lugar de $15.000 → cuota más alta que con gracia parcial.

> **Conclusión:** la gracia total siempre termina siendo más cara porque los intereses se capitalizan y aumentan la deuda.

---

*Resumen basado en los apuntes de la cátedra — Finanzas de Empresas 2025*
