# MODULE I – FUNDAMENTALS OF MEASUREMENTS  
## Step 3: Static Characteristics of Transducers

The syllabus specifies **“Characteristics of Transducers – Static and Dynamic”** as part of Module I. 0_SM_syllabus

The syllabus does not individually list the static characteristics, so the following notes explain the **standard static characteristics used in measurement and instrumentation**.

---

# 3.1 What are Static Characteristics?

When a transducer is used to measure a quantity that is **constant or changing very slowly with time**, its performance is described using **static characteristics**.

For example, suppose an RTD is being used to measure a slowly changing temperature.

```text
Constant / Slowly changing input
              ↓
          Transducer
              ↓
           Output
```

The relationship between input and output under these conditions is used to determine the **static characteristics**.

### Definition

> **Static characteristics are the performance characteristics of a measuring instrument or transducer when the measured quantity is either constant or varying very slowly with time.**

---

# 3.2 Important Static Characteristics

The important characteristics are:

1. Accuracy
2. Precision
3. Sensitivity
4. Linearity
5. Resolution
6. Threshold
7. Hysteresis
8. Repeatability
9. Reproducibility
10. Range
11. Span
12. Dead zone
13. Drift

Let's understand them one by one.

---

# 3.3 Accuracy

### Definition

**Accuracy** indicates how close the measured value is to the true or accepted value.

Suppose the actual temperature is:

\[
T_{true}=100^\circ C
\]

and the instrument reads:

\[
T_{measured}=99^\circ C
\]

The measurement is quite accurate because the measured value is close to the true value.

### Error

\[
\boxed{Error = Measured\ Value - True\ Value}
\]

For the above example:

\[
Error=99-100=-1^\circ C
\]

### Percentage error

\[
\boxed{\%Error =
\frac{|Measured-True|}{True}\times100}
\]

Therefore,

\[
\%Error=\frac{|99-100|}{100}\times100
\]

\[
\boxed{\%Error=1\%}
\]

### Remember

> **Accuracy → Closeness to the true value**

---

# 3.4 Precision

**Precision** indicates the degree of agreement among repeated measurements.

Suppose the same quantity is measured four times:

\[
10.01,\quad 10.02,\quad 10.01,\quad 10.02
\]

The values are very close to each other.

Therefore, the instrument has **high precision**.

However, if the actual value is 10.50, these measurements are not accurate.

### Important distinction

An instrument can be:

- Accurate but not precise
- Precise but not accurate
- Both accurate and precise
- Neither accurate nor precise

### Remember

> **Precision → Closeness of repeated measurements to each other**

---

# 3.5 Accuracy vs Precision

This is a very important examination concept.

| Accuracy | Precision |
|---|---|
| Closeness to true value | Closeness among repeated measurements |
| Related to error | Related to repeatability/consistency |
| Indicates correctness | Indicates consistency |
| Can be improved by calibration | Can be improved by reducing random variations |

### Example

True value = **50 V**

#### Case 1

Measurements:

\[
49.9,\ 50.1,\ 50.0
\]

→ Accurate and precise.

#### Case 2

Measurements:

\[
45.1,\ 45.2,\ 45.1
\]

→ Precise but not accurate.

Why?

They are very close to one another but far from 50 V.

---

# 3.6 Sensitivity

### Definition

**Sensitivity** is the ratio of change in output to the corresponding change in input.

\[
\boxed{
Sensitivity=\frac{\Delta Output}{\Delta Input}
}
\]

For a continuous input-output relationship:

\[
\boxed{
S=\frac{dy}{dx}
}
\]

where:

- \(x\) = input
- \(y\) = output

### Example

Suppose a temperature sensor produces:

- 0 V at 0°C
- 1 V at 100°C

Then:

\[
Sensitivity=
\frac{1-0}{100-0}
\]

\[
\boxed{S=0.01V/^\circ C}
\]

or

\[
\boxed{S=10mV/^\circ C}
\]

### Meaning

A highly sensitive instrument produces a relatively large change in output for a small change in input.

---

# 3.7 Linearity

Ideally, the output of a transducer should vary linearly with its input.

```text
Output
  │
  │             /
  │          /
  │       /
  │    /
  │ /
  └──────────────── Input
```

The ideal relationship can be represented as:

\[
y=mx+c
\]

where:

- \(m\) = sensitivity
- \(c\) = intercept

### Non-linearity

In a practical transducer, the actual output may deviate from the ideal straight-line relationship.

```text
Output
  │
  │        actual
  │       /
  │      /
  │     / ideal
  │   /
  │  /
  └──────────────── Input
```

The difference between the actual characteristic and the ideal characteristic is called **non-linearity error**.

---

# 3.8 Resolution

### Definition

**Resolution** is the smallest change in the input quantity that can be detected or measured by an instrument.

### Example

Suppose a digital thermometer displays:

```text
25.0°C
25.1°C
25.2°C
25.3°C
```

The smallest change it can display is:

\[
\boxed{0.1^\circ C}
\]

Therefore, its resolution is **0.1°C**.

### Remember

> **Resolution → Smallest detectable change**

---

# 3.9 Threshold

### Definition

**Threshold** is the minimum value of input that must be applied before the instrument produces a detectable output.

Suppose a sensor does not respond to inputs below 2 mm.

Then:

\[
\boxed{Threshold=2\,mm}
\]

```text
Input
  │
  │             Output begins
  │                  ↑
  │                  │
  └──────────────────┼──────
                    2 mm
                  Threshold
```

### Difference between resolution and threshold

| Resolution | Threshold |
|---|---|
| Smallest detectable change | Minimum input required to initiate response |
| Concerned with changes in input | Concerned with starting response |

---

# 3.10 Hysteresis

Hysteresis occurs when the output for a particular input value depends on whether the input is **increasing or decreasing**.

Consider a sensor whose input is first increased and then decreased.

```text
Output
  │       Increasing
  │      /
  │     / 
  │    / 
  │   / 
  │  / Decreasing
  │ /  /
  │/  /
  └──────────────── Input
```

For the same input value, two different output values may occur.

The difference is called **hysteresis**.

### Example

Suppose a temperature sensor gives:

- 50°C while temperature is increasing
- 48°C while temperature is decreasing

at the same corresponding input condition.

This difference is associated with hysteresis.

### Common causes

- Mechanical friction
- Magnetic effects
- Material properties
- Elastic deformation

---

# 3.11 Repeatability

### Definition

**Repeatability** is the ability of an instrument to produce nearly the same output when the same input is measured repeatedly under the same conditions.

Conditions remain the same:

- Same instrument
- Same operator
- Same environment
- Same method
- Short time interval

### Example

Input = 100 V

Measurements:

\[
99.8,\ 99.9,\ 99.8,\ 99.9\,V
\]

This indicates good repeatability.

---

# 3.12 Reproducibility

**Reproducibility** refers to the ability to obtain similar measurements when measurement conditions are changed.

Changes may include:

- Different operator
- Different instrument
- Different laboratory
- Different time
- Different environmental conditions

### Repeatability vs Reproducibility

| Repeatability | Reproducibility |
|---|---|
| Same conditions | Changed conditions |
| Same instrument | May use different instruments |
| Same operator | May use different operators |
| Usually short-term | Can involve longer time intervals |

### Easy memory trick

> **Repeatability → Repeat under same conditions**

> **Reproducibility → Reproduce under changed conditions**

---

# 3.13 Range

### Definition

The **range** of an instrument specifies the minimum and maximum values of the input quantity that the instrument can measure.

Example:

A voltmeter designed for:

\[
0-300V
\]

has a measurement range of:

\[
\boxed{0\text{ to }300V}
\]

---

# 3.14 Span

### Definition

**Span** is the algebraic difference between the maximum and minimum values of the measurement range.

\[
\boxed{Span=Maximum\ Value-Minimum\ Value}
\]

Example:

Range:

\[
20^\circ C\text{ to }120^\circ C
\]

Therefore:

\[
Span=120-20
\]

\[
\boxed{Span=100^\circ C}
\]

### Range vs Span

| Range | Span |
|---|---|
| Specifies minimum and maximum values | Difference between maximum and minimum |
| Example: 20–120°C | Example: 100°C |

---

# 3.15 Dead Zone

A **dead zone** is a range of input values over which there is **no observable change in output**.

```text
Output
  │
  │
  │             /
  │            /
  │___________/
  └──────────────── Input
             ↑
          Dead Zone
```

For example, if an instrument produces no output change for an input change between 0 and 2 mm, that region represents the dead zone.

### Dead zone vs Threshold

- **Threshold:** minimum input required to initiate response.
- **Dead zone:** range over which input changes produce no output change.

---

# 3.16 Drift

**Drift** is the slow change in instrument output even when the input remains constant.

Suppose a temperature sensor is placed in a constant-temperature environment:

\[
25^\circ C
\]

Initially it reads:

\[
25.0^\circ C
\]

After several hours it reads:

\[
26.0^\circ C
\]

even though the actual temperature remains constant.

This change is called **drift**.

### Causes of drift

- Temperature changes
- Aging of components
- Mechanical stress
- Component deterioration
- Environmental effects

---

# 3.17 Types of Drift

The important types are:

### 1. Zero Drift

The entire calibration characteristic shifts by a constant amount.

```text
Output
  │       /
  │      / Original
  │     /
  │    /
  │   / Shifted
  │  /
  └────────────── Input
```

The output has an offset.

---

### 2. Sensitivity Drift

The slope of the calibration characteristic changes.

```text
Output
  │       /
  │      / Original
  │     /
  │    /
  │   / 
  │  / Changed sensitivity
  │ /
  └──────────────── Input
```

The sensitivity of the instrument changes.

---

### 3. Zeros + Sensitivity Drift

Both the intercept and slope change.

---

# 3.18 Static Characteristics – Quick Summary

| Characteristic | Meaning |
|---|---|
| Accuracy | Closeness to true value |
| Precision | Closeness among repeated measurements |
| Sensitivity | Output change / Input change |
| Linearity | Closeness to ideal linear relationship |
| Resolution | Smallest detectable input change |
| Threshold | Minimum input needed to initiate response |
| Hysteresis | Different output for increasing/decreasing input |
| Repeatability | Same result under same conditions |
| Reproducibility | Similar result under changed conditions |
| Range | Minimum to maximum measurable value |
| Span | Maximum − Minimum |
| Dead zone | Input region producing no output change |
| Drift | Output changes with constant input |

---

# 3.19 Important Formulas

### Sensitivity

\[
\boxed{S=\frac{\Delta Output}{\Delta Input}}
\]

### Percentage Error

\[
\boxed{
\%Error=
\frac{|Measured-True|}{True}\times100
}
\]

### Span

\[
\boxed{Span=Maximum-Minimum}
\]

### Relative Sensitivity

\[
\boxed{
S=\frac{dy}{dx}
}
\]

---

# 🎯 Important Exam Questions

### 2 Marks

1. Define static characteristics.
2. Define accuracy.
3. Define precision.
4. What is sensitivity?
5. Define resolution.
6. What is threshold?
7. Define hysteresis.
8. What is repeatability?
9. What is reproducibility?
10. Define range and span.
11. What is drift?
12. What is dead zone?

### 5 Marks

1. Explain the static characteristics of a transducer.
2. Explain accuracy and precision with suitable examples.
3. Explain sensitivity and linearity.
4. Explain resolution, threshold and dead zone.
5. Explain hysteresis and its causes.
6. Differentiate between repeatability and reproducibility.
7. Explain range, span and drift.

### ⭐ Very Important

**Q. Explain the static characteristics of a measuring instrument/transducer.**

For a long-answer question, organize the answer as:

```text
Static Characteristics
       │
       ├── Accuracy
       ├── Precision
       ├── Sensitivity
       ├── Linearity
       ├── Resolution
       ├── Threshold
       ├── Hysteresis
       ├── Repeatability
       ├── Reproducibility
       ├── Range
       ├── Span
       ├── Dead Zone
       └── Drift
```

---

### Next Step → **Step 4: Dynamic Characteristics of Transducers**

We will cover **speed of response, fidelity, lag, dynamic error, time constant, first-order and second-order systems**, including the important response curves and formulas.
