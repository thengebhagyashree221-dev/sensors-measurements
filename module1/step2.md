# MODULE I – FUNDAMENTALS OF MEASUREMENTS  
## Step 2: Classification of Transducers

The syllabus specifically includes **“Classification and Characteristics of Transducers – Static and Dynamic”** under Module I. 0_SM_syllabus

> **Note:** The syllabus only specifies the topic; it does not list the individual classification categories. The classifications below are therefore standard measurement/instrumentation concepts used to explain this syllabus topic.

---

# 2.1 What is a Transducer?

A **transducer** is a device that converts a physical quantity into another form of energy, usually an electrical signal, which can be measured, processed, transmitted, or displayed.

### Basic concept

```text
Physical Quantity
     │
     ▼
┌──────────────┐
│  Transducer  │
└──────────────┘
     │
     ▼
Electrical Signal
```

### Examples

| Physical quantity | Transducer | Output |
|---|---|---|
| Temperature | Thermocouple | Voltage |
| Displacement | LVDT | Voltage |
| Pressure | Pressure sensor | Electrical signal |
| Strain | Strain gauge | Change in resistance |
| Light | Photodiode | Current |
| Force | Load cell | Electrical signal |

---

# 2.2 Why Are Transducers Required?

Most physical quantities cannot be directly processed by electronic systems.

For example, suppose we want to measure **temperature**.

A computer cannot directly understand:

> "The temperature is 35°C."

A temperature sensor converts the temperature into an electrical quantity:

```text
Temperature
    ↓
Temperature Sensor
    ↓
Electrical Signal
    ↓
Signal Conditioning
    ↓
ADC
    ↓
Computer / Display
```

Therefore, transducers provide the interface between the **physical world** and the **measurement system**.

---

# 2.3 Classification of Transducers

Transducers can be classified in several ways.

The important classifications are:

1. Primary and Secondary Transducers
2. Active and Passive Transducers
3. Analog and Digital Transducers
4. Electrical and Non-electrical Transducers
5. Transducers based on the operating principle

Let's understand each one.

---

# 2.4 Primary and Secondary Transducers

## Primary Transducer

A **primary transducer** directly senses the physical quantity and produces a corresponding output.

### Example

A **Bourdon tube** used for pressure measurement.

```text
Pressure
   ↓
Bourdon Tube
   ↓
Mechanical displacement
```

The Bourdon tube directly responds to pressure.

---

## Secondary Transducer

A **secondary transducer** receives the output of a primary transducer and converts it into another useful form, generally an electrical signal.

For example:

```text
Pressure
   ↓
Bourdon Tube
   ↓
Displacement
   ↓
LVDT
   ↓
Electrical Signal
```

Here:

- Bourdon tube → Primary transducer
- LVDT → Secondary transducer

### Important point

The output of the primary transducer becomes the input to the secondary transducer.

---

# 2.5 Active and Passive Transducers

This is one of the **most important classifications for examinations**.

---

## A. Active Transducers

An **active transducer** generates its own electrical output without requiring an external excitation source.

They are also called **self-generating transducers**.

### Examples

- Thermocouple
- Piezoelectric transducer
- Photovoltaic cell

### Example: Thermocouple

When two dissimilar metals are joined and their junctions are maintained at different temperatures, a voltage is generated.

```text
Temperature Difference
        ↓
    Thermocouple
        ↓
      Voltage
```

No external power supply is required to generate the basic output.

---

## B. Passive Transducers

A **passive transducer** requires an external source of excitation.

The physical quantity changes some electrical parameter such as:

- Resistance
- Inductance
- Capacitance

### Examples

| Transducer | Parameter changed |
|---|---|
| Strain gauge | Resistance |
| RTD | Resistance |
| LVDT | Inductance |
| Capacitive transducer | Capacitance |

For example:

```text
External Excitation
       ↓
   Strain Gauge
       ↑
     Strain
       ↓
Change in Resistance
```

---

## Active vs Passive

| Active | Passive |
|---|---|
| Self-generating | Requires external excitation |
| Produces electrical output directly | Modifies an electrical parameter |
| Usually does not require external power for sensing | Requires external power |
| Thermocouple | Strain gauge |
| Piezoelectric sensor | RTD |
| Photovoltaic cell | LVDT |

### Memory trick

> **Active → produces output**  
> **Passive → needs power**

---

# 2.6 Analog and Digital Transducers

## Analog Transducer

An analog transducer produces an output that varies **continuously** with the input quantity.

Example:

```text
Temperature
    ↓
   RTD
    ↓
Resistance
```

As temperature changes continuously, resistance also changes continuously.

---

## Digital Transducer

A digital transducer produces an output in **discrete or digital form**.

Examples include:

- Optical encoders
- Digital position sensors
- Digital temperature sensors

Example:

```text
Rotational Position
       ↓
 Optical Encoder
       ↓
Digital Pulse Output
```

---

## Analog vs Digital

| Analog | Digital |
|---|---|
| Continuous output | Discrete/digital output |
| Output can have continuously varying values | Output represented by discrete states |
| More susceptible to noise | Generally better suited for digital processing |
| RTD | Optical encoder |
| LVDT | Digital position sensor |

---

# 2.7 Electrical and Non-Electrical Transducers

## Electrical Transducer

An electrical transducer produces an **electrical output** corresponding to the measured quantity.

Examples:

- Thermocouple → voltage
- Strain gauge → resistance change
- LVDT → voltage
- Photodiode → current

---

## Non-Electrical Transducer

A non-electrical transducer produces a **non-electrical output**, such as:

- Displacement
- Mechanical movement
- Pressure
- Force

Example:

```text
Pressure
   ↓
Bourdon Tube
   ↓
Mechanical Displacement
```

The output is mechanical rather than electrical.

---

# 2.8 Classification Based on Transduction Principle

Transducers can also be classified according to the electrical property affected.

### 1. Resistive Transducers

The resistance changes with the measurand.

Examples:

- Strain gauge
- RTD
- Thermistor

```text
Physical Quantity
       ↓
Change in Resistance
```

---

### 2. Inductive Transducers

The inductance or related magnetic quantity changes.

Example:

- LVDT

```text
Displacement
     ↓
LVDT
     ↓
Change in Inductive Output
```

---

### 3. Capacitive Transducers

The capacitance changes due to variation in:

- Distance between plates
- Area of overlap
- Dielectric material

Example:

```text
Displacement
     ↓
Change in Capacitance
```

---

### 4. Piezoelectric Transducers

Mechanical stress produces an electrical charge/voltage.

Example:

```text
Force / Pressure
       ↓
Piezoelectric Material
       ↓
Electrical Charge / Voltage
```

---

### 5. Photoelectric Transducers

Light energy is converted into an electrical output.

Examples:

- Photodiode
- Phototransistor
- Photovoltaic cell

These become particularly important in **Module III**, which covers photoelectric sensors. 0_SM_syllabus

---

# 2.9 Important Classification – Summary

```text
                    TRANSDUCERS
                         │
        ┌────────────────┼─────────────────┐
        │                │                 │
     Primary          Active/           Analog/
    /Secondary        Passive           Digital
        │                │                 │
        │          ┌─────┴─────┐           │
        │          │           │           │
        │        Active      Passive       │
        │          │           │           │
        │      Thermocouple  RTD           │
        │      Piezoelectric Strain Gauge  │
        │
        └────────────────────────────────────
                         │
                 Based on Principle
                         │
       ┌─────────┬────────┬─────────┬─────────┐
       ↓         ↓        ↓         ↓
   Resistive  Inductive Capacitive Piezoelectric
```

---

# 2.10 Worked Example: Temperature Measurement

Let's identify the classification of some temperature sensors.

### Thermocouple

- Active
- Analog
- Electrical output
- Principle: thermoelectric effect

### RTD

- Passive
- Analog
- Electrical output
- Principle: change in resistance

### Thermistor

- Passive
- Analog
- Electrical output
- Principle: change in resistance

This gives us a useful comparison:

| Sensor | Active/Passive | Output principle |
|---|---|---|
| Thermocouple | Active | Voltage generation |
| RTD | Passive | Resistance change |
| Thermistor | Passive | Resistance change |

---

# 2.11 Exam-Oriented Definitions

### Transducer
> A transducer is a device that converts a physical quantity into a corresponding signal, generally an electrical signal, suitable for measurement and processing.

### Active Transducer
> A transducer that generates its own electrical output without requiring external excitation is called an active transducer.

### Passive Transducer
> A transducer that requires external excitation and changes an electrical parameter such as resistance, inductance, or capacitance is called a passive transducer.

### Primary Transducer
> A transducer that directly senses the measurand and produces an output corresponding to it is called a primary transducer.

### Secondary Transducer
> A transducer that receives the output of a primary transducer and converts it into a suitable measurable signal is called a secondary transducer.

---

# Important Exam Questions

### 2-Mark Questions

1. Define a transducer.
2. What is an active transducer?
3. What is a passive transducer?
4. Give two examples of active transducers.
5. Give two examples of passive transducers.
6. Differentiate between primary and secondary transducers.
7. What is an analog transducer?
8. What is a digital transducer?

### 5-Mark Questions

1. Explain the classification of transducers.
2. Explain active and passive transducers with examples.
3. Differentiate between active and passive transducers.
4. Explain primary and secondary transducers with an example.
5. Explain analog and digital transducers.

### Very Important

**Q. Explain the classification of transducers with suitable examples.**

For this question, remember these four major bases:

> **Primary/Secondary → Active/Passive → Analog/Digital → Operating Principle**

---

## Next Step

**Step 3 will be: _Characteristics of Transducers – Static Characteristics_**

We'll cover the important characteristics one by one:

**Accuracy → Precision → Sensitivity → Linearity → Resolution → Threshold → Hysteresis → Repeatability → Reproducibility → Range → Span → Dead Zone → Drift**

This is an important section because many of these terms will appear again when we study **errors, uncertainty, accuracy and precision**.
