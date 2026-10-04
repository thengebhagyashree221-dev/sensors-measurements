# MODULE I – FUNDAMENTALS OF MEASUREMENTS
## Step 4: Dynamic Characteristics of Transducers

Your syllabus specifies **“Characteristics of Transducers – Static and Dynamic”** under Module I. 0_SM_syllabus

The syllabus does not list the individual dynamic characteristics or mathematical models. So the detailed concepts below are the **standard instrumentation treatment of dynamic characteristics** used to explain this syllabus topic.

---

# 4.1 What are Dynamic Characteristics?

In the previous step, we considered an input that was **constant or changing very slowly**.

But in real applications, the measured quantity may change rapidly with time.

For example:

- Temperature suddenly increases.
- Pressure changes rapidly.
- Motor speed changes.
- Vibration occurs.
- An electrical signal changes with time.

In such cases, the output of the transducer may **not change instantaneously** with the input.

Therefore, we need to study its **dynamic characteristics**.

### Definition

> **Dynamic characteristics describe the performance of a measuring instrument when the input quantity varies with time.**

---

# 4.2 Static vs Dynamic Characteristics

| Static Characteristics | Dynamic Characteristics |
|---|---|
| Input is constant or slowly varying | Input varies with time |
| Steady-state behavior is studied | Time-dependent behavior is studied |
| Accuracy | Speed of response |
| Sensitivity | Fidelity |
| Linearity | Lag |
| Resolution | Dynamic error |
| Hysteresis | Time constant |
| Drift | Rise time / settling time |

### Easy way to remember

> **Static → How accurately does the instrument measure a steady value?**

> **Dynamic → How quickly and accurately does it follow a changing value?**

---

# 4.3 Important Dynamic Characteristics

The important dynamic characteristics generally considered are:

1. Speed of response
2. Fidelity
3. Lag
4. Dynamic error
5. Time constant
6. Rise time
7. Settling time
8. Dynamic response of first-order systems
9. Dynamic response of second-order systems

---

# 4.4 Speed of Response

### Definition

**Speed of response** is the ability of an instrument to respond quickly to a change in the input.

Suppose the actual temperature suddenly changes from:

\[
20^\circ C \rightarrow 80^\circ C
\]

A fast sensor should quickly indicate the new temperature.

```text
Input
  │       ┌──────────────
  │       │
  │───────┘
  └────────────────────── Time


Output
  │          ┌───────────
  │        /
  │      /
  │─────
  └────────────────────── Time
```

The output takes some time to reach the final value.

### High speed of response

The output reaches the final value quickly.

### Low speed of response

The output takes longer.

---

# 4.5 Fidelity

### Definition

**Fidelity** is the ability of a measurement system to reproduce changes in the input signal without distortion.

In simple terms:

> **Fidelity tells us how faithfully the instrument follows the input.**

Suppose the input varies as:

```text id="2p3m7m"
Input:
   /\/\__/\/\__/\/\__
```

An instrument with good fidelity produces an output with the same general shape:

```text id="g6f1ck"
Output:
   /\/\__/\/\__/\/\__
```

An instrument with poor fidelity may distort the waveform.

### Important point

Fidelity is particularly important when measuring **rapidly changing or dynamic signals**.

---

# 4.6 Lag

### Definition

**Lag** is the delay in the response of an instrument relative to a change in the input.

Suppose the input changes at:

\[
t=0
\]

but the instrument begins responding after some delay.

```text id="u6uwgq"
Input
  │    ┌──────────────
  │────┘
  └────────────────── Time
       ↑
       Input changes


Output
  │        ┌──────────
  │───────┘
  └────────────────── Time
          ↑
       Output responds
```

This difference represents response lag.

---

# 4.7 Types of Lag

Two commonly discussed forms are:

### 1. Retardation-type lag

The instrument responds slowly because of physical properties.

Example:

A thermometer placed in hot water does not immediately reach the water temperature.

Why?

Because heat needs time to transfer to the sensing element.

---

### 2. Measurement lag

The measuring system takes time to respond to a changing input because of the characteristics of its sensing and processing elements.

---

# 4.8 Dynamic Error

### Definition

**Dynamic error** is the difference between the instantaneous value of the input and the corresponding measured value when the input is changing with time.

\[
\boxed{
Dynamic\ Error =
True\ instantaneous\ value -
Measured\ value
}
\]

For example:

Actual temperature:

\[
80^\circ C
\]

Sensor indicates:

\[
72^\circ C
\]

Then:

\[
Dynamic\ Error=80-72
\]

\[
\boxed{Dynamic\ Error=8^\circ C}
\]

This error can occur because the sensor cannot respond instantaneously.

---

# 4.9 Time Constant

The **time constant** is one of the most important concepts in dynamic response.

Consider a simple **first-order measurement system**.

For a step input, the output gradually approaches its final value.

```text
Output
  │                    ───── Final value
  │                .-'
  │             .-'
  │          .-'
  │       .-'
  │    .-'
  │_.-'
  └──────────────────────── Time
          ↑
       τ (time constant)
```

For a first-order system, after **one time constant \(\tau\)**, the output reaches approximately:

\[
\boxed{63.2\%}
\]

of its final value for a step input.

---

# 4.10 First-Order System

A first-order measurement system can be represented by:

\[
\boxed{
\tau\frac{dy}{dt}+y=Kx
}
\]

where:

- \(x\) = input
- \(y\) = output
- \(K\) = static sensitivity
- \(\tau\) = time constant

Its transfer function is:

\[
\boxed{
\frac{Y(s)}{X(s)}
=
\frac{K}{\tau s+1}
}
\]

---

# 4.11 Step Response of a First-Order System

For a step input, the response is:

\[
\boxed{
y(t)=KX_0\left(1-e^{-t/\tau}\right)
}
\]

where:

- \(X_0\) = magnitude of step input
- \(KX_0\) = final output
- \(\tau\) = time constant

If normalized with respect to the final value:

\[
\boxed{
\frac{y(t)}{y(\infty)}
=
1-e^{-t/\tau}
}
\]

---

# 4.12 Significance of Time Constant

The time constant tells us how quickly a first-order instrument responds.

For a first-order system:

| Time | Approx. output |
|---|---:|
| \(t=\tau\) | 63.2% |
| \(t=2\tau\) | 86.5% |
| \(t=3\tau\) | 95.0% |
| \(t=4\tau\) | 98.2% |
| \(t=5\tau\) | 99.3% |

Therefore, after approximately:

\[
\boxed{5\tau}
\]

the output is practically at its final value.

### Important exam point

> **Smaller time constant → faster response.**

> **Larger time constant → slower response.**

---

# 4.13 Example – Time Constant

Suppose a first-order temperature sensor has:

\[
\tau=2s
\]

How much time is approximately required to reach 95% of the final value?

From the table:

\[
95\%\approx3\tau
\]

Therefore:

\[
t=3(2)
\]

\[
\boxed{t=6s}
\]

---

# 4.14 Rise Time

**Rise time** is the time taken by the output to rise from a specified lower percentage to a specified upper percentage of its final value.

Commonly:

\[
10\% \rightarrow 90\%
\]

is used.

For a first-order system:

\[
\boxed{t_r\approx2.2\tau}
\]

Thus, if:

\[
\tau=0.5s
\]

then:

\[
t_r=2.2(0.5)
\]

\[
\boxed{t_r=1.1s}
\]

---

# 4.15 Settling Time

**Settling time** is the time required for the output to enter and remain within a specified band around its final value.

For example, if the tolerance is ±2%, the output must reach the region:

\[
98\%\leq Output\leq102\%
\]

and remain there.

For a first-order system, approximately:

\[
\boxed{t_s\approx4\tau}
\]

for a 2% criterion.

---

# 4.16 Second-Order System

Some measurement systems cannot be adequately represented by a first-order model.

A second-order system is commonly represented by:

\[
\boxed{
\frac{Y(s)}{X(s)}
=
\frac{K\omega_n^2}
{s^2+2\zeta\omega_n s+\omega_n^2}
}
\]

where:

- \(K\) = static sensitivity
- \(\omega_n\) = natural frequency
- \(\zeta\) = damping ratio

These two parameters are particularly important:

### Natural frequency

\[
\omega_n
\]

describes the natural oscillation characteristics of the system.

### Damping ratio

\[
\zeta
\]

describes how oscillations are reduced.

---

# 4.17 Damping Ratio

The response of a second-order system depends strongly on \(\zeta\).

### Case 1: Underdamped

\[
0<\zeta<1
\]

The output oscillates before settling.

```text id="w8drp3"
Output
  │     /\ 
  │    /  \    /\
  │   /    \__/  \__
  │──
  └────────────────── Time
```

---

### Case 2: Critically damped

\[
\zeta=1
\]

The system reaches the final value quickly without oscillation.

---

### Case 3: Overdamped

\[
\zeta>1
\]

The system responds slowly without oscillation.

---

### Case 4: Undamped

\[
\zeta=0
\]

The system continues oscillating.

---

# 4.18 Dynamic Characteristics – Summary

| Characteristic | Meaning |
|---|---|
| Speed of response | How quickly the instrument responds |
| Fidelity | Ability to reproduce input without distortion |
| Lag | Delay between input change and output response |
| Dynamic error | Difference during changing-input conditions |
| Time constant | Measure of response speed of a first-order system |
| Rise time | Time to move from lower to upper specified output level |
| Settling time | Time to remain within specified final-value band |
| Natural frequency | Characteristic frequency of second-order system |
| Damping ratio | Degree to which oscillations are suppressed |

---

# ⭐ Static vs Dynamic – Very Important Question

| Parameter | Static | Dynamic |
|---|---|---|
| Input | Constant / slowly varying | Time-varying |
| Main concern | Steady-state measurement | Time response |
| Accuracy | Important | Important |
| Sensitivity | Important | Important |
| Linearity | Important | Important |
| Speed of response | — | Important |
| Fidelity | — | Important |
| Lag | — | Important |
| Time constant | — | Important |
| Dynamic error | — | Important |

---

# 🎯 Exam Questions

### Short Answer

1. Define dynamic characteristics.
2. What is speed of response?
3. Define fidelity.
4. What is lag?
5. Define dynamic error.
6. What is time constant?
7. What is rise time?
8. Define settling time.
9. What is damping ratio?
10. What is natural frequency?

### Numerical Questions

1. A first-order sensor has a time constant of 2 seconds. Calculate the time required to reach 95% of its final value.
2. A first-order system has a time constant of 0.5 s. Calculate its approximate rise time.
3. Given a first-order transfer function, determine its time constant and response to a step input.
4. Calculate the output of a first-order system at \(t=\tau\), \(2\tau\), and \(3\tau\).

### Long Answer

**Q. Explain the dynamic characteristics of a measuring instrument.**

A good answer should include:

```text
Dynamic Characteristics
       │
       ├── Speed of response
       ├── Fidelity
       ├── Lag
       ├── Dynamic error
       ├── Time constant
       ├── Rise time
       ├── Settling time
       └── Second-order characteristics
             ├── Natural frequency
             └── Damping ratio
```

---

## Next Step → **Step 5: Errors in Measurement**

This is a **very important part of Module I** because the syllabus explicitly requires **“Errors in Measurements and their statistical analysis”** and **“methods of error analysis.”** 0_SM_syllabus

We'll cover:

**True value → Measured value → Error → Gross errors → Systematic errors → Random errors → Absolute error → Relative error → Percentage error → Limiting error → Error calculation → practical numerical problems.**
