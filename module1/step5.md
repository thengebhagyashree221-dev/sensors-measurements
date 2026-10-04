# STEP 5 – ERRORS IN MEASUREMENT

The syllabus explicitly includes **“Errors in Measurements and their statistical analysis”** and **“methods of error analysis.”** 0_SM_syllabus

## 5.1 What is Measurement Error?

Whenever we measure a physical quantity, the measured value may differ from its true or accepted value.

This difference is called **measurement error**.

### Definition

> **Measurement error is the difference between the measured value of a quantity and its true or accepted value.**

Mathematically:

\[
\boxed{E=X_m-X_t}
\]

where:

- \(E\) = error
- \(X_m\) = measured value
- \(X_t\) = true/accepted value

### Example

Suppose the true voltage is:

\[
X_t=100V
\]

but the voltmeter indicates:

\[
X_m=98V
\]

Therefore,

\[
E=98-100
\]

\[
\boxed{E=-2V}
\]

The negative sign indicates that the instrument reading is below the true value.

---

# 5.2 Why Do Errors Occur?

It is practically impossible to obtain a perfectly accurate measurement because of factors such as:

- Limitations of the measuring instrument
- Environmental conditions
- Human observation
- Imperfect measurement techniques
- Electrical noise
- Aging of components
- Calibration limitations
- Random variations

Therefore:

> **No practical measurement is completely free from error.**

The objective is not necessarily to eliminate every error, but to **identify, estimate, minimize and account for errors**.

---

# 5.3 Classification of Measurement Errors

A commonly used classification is:

```text
                 Measurement Errors
                        │
          ┌─────────────┼─────────────┐
          │             │             │
       Gross        Systematic      Random
       Errors         Errors        Errors
                         │
              ┌──────────┼──────────┐
              │          │          │
         Instrumental  Environmental  Observational
```

Let's understand each.

---

# 5.4 Gross Errors

### Definition

**Gross errors** are errors caused mainly by human mistakes during measurement or recording.

Examples:

- Incorrect reading of an instrument
- Recording 25 V as 52 V
- Using the wrong measurement range
- Incorrectly noting a decimal point
- Calculation mistakes
- Incorrect connection of an instrument

### Example

Actual reading:

\[
12.5V
\]

Operator records:

\[
21.5V
\]

This is a gross error.

### How to reduce gross errors?

- Take repeated measurements.
- Check instrument connections.
- Verify readings.
- Use proper measurement procedures.
- Use digital instruments where appropriate.
- Cross-check calculated values.

---

# 5.5 Systematic Errors

Systematic errors occur in a **consistent or predictable manner**.

They tend to produce measurements that are consistently higher or lower than the actual value.

For example, suppose a voltmeter always reads 2 V higher:

| True value | Meter reading |
|---:|---:|
| 10 V | 12 V |
| 20 V | 22 V |
| 30 V | 32 V |

The error has a systematic nature.

### Important types

Systematic errors may arise from:

1. Instrumental errors
2. Environmental errors
3. Observational errors

---

# 5.6 Instrumental Errors

These errors are associated with the measuring instrument itself.

Possible causes include:

- Imperfect calibration
- Aging of components
- Friction
- Hysteresis
- Zero error
- Manufacturing imperfections
- Changes in component characteristics

### Example

A weighing instrument shows:

\[
0.5kg
\]

even when no object is placed on it.

This is a **zero error**.

---

# 5.7 Environmental Errors

These errors occur because environmental conditions affect the measurement system.

Examples:

- Temperature
- Humidity
- Pressure
- Magnetic field
- Electric field
- Vibration
- Dust

### Example

A precision resistance measurement changes when the surrounding temperature changes because the resistance of the sensing element is temperature-dependent.

### Minimization

Environmental effects can be reduced using:

- Shielding
- Temperature control
- Proper grounding
- Isolation
- Compensation techniques
- Controlled measurement environments

---

# 5.8 Observational Errors

These errors occur because of the way a person observes or interprets the instrument reading.

A common example with analog instruments is **parallax error**.

Suppose the pointer is viewed from an angle rather than directly in front of the scale.

```text
Incorrect viewing
       👁
        \
         \ 
          \   Pointer
           \    ↓
            ──── Scale
```

The apparent position of the pointer may be incorrect.

### How to reduce observational errors?

- View the scale correctly.
- Use mirror scales where provided.
- Take readings at eye level.
- Prefer digital displays when appropriate.

---

# 5.9 Random Errors

Random errors vary unpredictably from one measurement to another.

For example, repeated measurements may be:

\[
10.1,\quad 9.9,\quad 10.2,\quad 10.0,\quad 9.8
\]

The variations do not follow a simple predictable pattern.

### Causes

Possible causes include:

- Electrical noise
- Small environmental fluctuations
- Mechanical vibrations
- Unpredictable variations in the measurement process

### Important point

Random errors cannot generally be eliminated completely.

However, their effect can often be **reduced by taking repeated measurements and applying statistical methods**.

This leads directly to **Step 6 – Statistical Analysis**.

---

# 5.10 Gross vs Systematic vs Random Errors

| Feature | Gross | Systematic | Random |
|---|---|---|---|
| Nature | Human mistakes | Consistent/predictable | Unpredictable |
| Example | Wrong reading | Zero error | Electrical noise |
| Direction | May be large | Usually consistent | Changes randomly |
| Repetition helps? | Yes | Not necessarily | Yes |
| Statistical treatment | Generally not the main method | Calibration/correction | Statistical methods |
| Can be minimized? | Yes | Yes | Reduced, not completely eliminated |

---

# 5.11 Absolute Error

The magnitude of the difference between the measured value and the true/accepted value is called **absolute error**.

\[
\boxed{
E_a=|X_m-X_t|
}
\]

### Example

True value:

\[
100V
\]

Measured value:

\[
98V
\]

Therefore:

\[
E_a=|98-100|
\]

\[
\boxed{E_a=2V}
\]

---

# 5.12 Relative Error

Relative error is the ratio of absolute error to the true/accepted value.

\[
\boxed{
E_r=\frac{|X_m-X_t|}{X_t}
}
\]

For the previous example:

\[
E_r=\frac{2}{100}
\]

\[
\boxed{E_r=0.02}
\]

---

# 5.13 Percentage Error

Percentage error is:

\[
\boxed{
\%E=
\frac{|X_m-X_t|}{X_t}\times100
}
\]

For:

\[
X_t=100V,\quad X_m=98V
\]

\[
\%E=\frac{|98-100|}{100}\times100
\]

\[
\boxed{\%E=2\%}
\]

---

# 5.14 Example – Error Calculation

A voltmeter measures a voltage as **47.5 V**. The accepted value is **50 V**. Calculate:

1. Absolute error
2. Relative error
3. Percentage error

### Given

\[
X_m=47.5V
\]

\[
X_t=50V
\]

### 1. Absolute error

\[
E_a=|47.5-50|
\]

\[
\boxed{E_a=2.5V}
\]

### 2. Relative error

\[
E_r=\frac{2.5}{50}
\]

\[
\boxed{E_r=0.05}
\]

### 3. Percentage error

\[
\%E=0.05\times100
\]

\[
\boxed{\%E=5\%}
\]

---

# 5.15 Important Relationship

Remember:

\[
\boxed{
Relative\ Error=
\frac{Absolute\ Error}{True\ Value}
}
\]

and

\[
\boxed{
Percentage\ Error=
Relative\ Error\times100
}
\]

---

# 5.16 Error vs Accuracy

These concepts are related but not identical.

Generally:

> **Smaller error → Better accuracy**

For example:

| Instrument | Error |
|---|---:|
| A | 0.5 V |
| B | 5 V |

For the same measurement range and conditions, instrument A would generally provide better accuracy.

---

# ⭐ Exam-Oriented Summary

### Measurement Error

\[
\boxed{E=X_m-X_t}
\]

### Absolute Error

\[
\boxed{E_a=|X_m-X_t|}
\]

### Relative Error

\[
\boxed{E_r=\frac{|X_m-X_t|}{X_t}}
\]

### Percentage Error

\[
\boxed{
\%E=
\frac{|X_m-X_t|}{X_t}\times100
}
\]

### Three major categories

> **Gross → Systematic → Random**

### Systematic error sources

> **Instrumental → Environmental → Observational**

---

# 🎯 Important Exam Questions

### 2 Marks

1. Define measurement error.
2. What is absolute error?
3. Define relative error.
4. Define percentage error.
5. What are gross errors?
6. What are systematic errors?
7. What are random errors?
8. List the sources of systematic errors.
9. What is instrumental error?
10. What is environmental error?
11. What is observational error?

### 5 Marks

1. Explain the classification of measurement errors.
2. Explain gross, systematic and random errors.
3. Explain the different types of systematic errors.
4. Explain absolute, relative and percentage errors with formulas.
5. Explain methods for minimizing measurement errors.

### ⭐ Very Important

**Q. Explain different types of errors in measurement with suitable examples.**

A good answer structure:

```text
Measurement Errors
       │
       ├── Gross Errors
       │
       ├── Systematic Errors
       │      ├── Instrumental
       │      ├── Environmental
       │      └── Observational
       │
       └── Random Errors
```

---

## Progress

We have now completed:

**1 → Measurement System** ✅  
**2 → Classification of Transducers** ✅  
**3 → Static Characteristics** ✅  
**4 → Dynamic Characteristics** ✅  
**5 → Errors in Measurement** ✅

### Next → Step 6: Statistical Analysis of Measurement

There we'll study **mean/average, deviation, standard deviation, variance, probable error, distribution of errors, and how repeated measurements are statistically evaluated**, followed by numerical examples.
