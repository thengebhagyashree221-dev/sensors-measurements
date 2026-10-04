# MODULE I – FUNDAMENTALS OF MEASUREMENTS
## Step 6: Statistical Analysis of Measurement

The syllabus places **statistical analysis of measurement** under errors in measurement and methods of error analysis. 0_SM_syllabus

> **Important:** The uploaded syllabus names this topic but does not specify the individual statistical formulas. So the treatment below is the standard statistical approach used for repeated measurements.

---

# 6.1 Why Statistical Analysis is Needed

Suppose we measure the same voltage five times:

$$
10.2,\quad 10.1,\quad 10.3,\quad 9.9,\quad 10.0\ V
$$

Why aren't all the readings exactly the same?

Because of **random errors**.

A single measurement may not represent the best estimate of the quantity.

Therefore, we take several measurements and use statistical methods to obtain:

- Best estimate of the measured value
- Variation in measurements
- Standard deviation
- Uncertainty associated with the measurements

The basic idea is:

```text
Repeated Measurements
          ↓
   Statistical Analysis
          ↓
Best Estimate + Variation
```

---

# 6.2 Arithmetic Mean

The most basic statistical quantity is the **arithmetic mean**.

If the measured values are:

$$
x_1,x_2,x_3,\ldots,x_n
$$

then the arithmetic mean is:

$$
\boxed{
\bar{x}=\frac{x_1+x_2+x_3+\cdots+x_n}{n}
}
$$

or

$$
\boxed{
\bar{x}=\frac{1}{n}\sum_{i=1}^{n}x_i
}
$$

where:

- \(\bar{x}\) = arithmetic mean
- \(x_i\) = individual measurement
- \(n\) = number of measurements

---

# 6.3 Example – Arithmetic Mean

Suppose a voltage is measured five times:

| Measurement | Voltage |
|---|---:|
| \(x_1\) | 10.2 V |
| \(x_2\) | 10.1 V |
| \(x_3\) | 10.3 V |
| \(x_4\) | 9.9 V |
| \(x_5\) | 10.0 V |

Then:

$$
\bar{x}=
\frac{10.2+10.1+10.3+9.9+10.0}{5}
$$

$$
\bar{x}=\frac{50.5}{5}
$$

$$
\boxed{\bar{x}=10.1V}
$$

Therefore, **10.1 V** is the arithmetic mean.

---

# 6.4 Deviation from the Mean

To understand how much each measurement differs from the mean, we calculate the **deviation**.

For an individual measurement:

$$
\boxed{
d_i=x_i-\bar{x}
}
$$

where:

- \(x_i\) = individual measurement
- \(\bar{x}\) = mean
- \(d_i\) = deviation

Using the previous example:

$$
\bar{x}=10.1V
$$

For \(x_1=10.2V\):

$$
d_1=10.2-10.1
$$

$$
d_1=+0.1V
$$

For \(x_2=10.1V\):

$$
d_2=10.1-10.1=0
$$

For \(x_3=10.3V\):

$$
d_3=+0.2V
$$

---

# 6.5 Deviation Table

For our five readings:

| \(x_i\) | \(d_i=x_i-\bar{x}\) |
|---:|---:|
| 10.2 | +0.1 |
| 10.1 | 0 |
| 10.3 | +0.2 |
| 9.9 | −0.2 |
| 10.0 | −0.1 |

Notice:

$$
\sum d_i=0
$$

This is an important property of the arithmetic mean.

$$
\boxed{\sum_{i=1}^{n}(x_i-\bar{x})=0}
$$

---

# 6.6 Average Deviation

The **average deviation** can be calculated using the absolute values of the deviations:

$$
\boxed{
D=\frac{\sum |d_i|}{n}
}
$$

For our example:

$$
|d_i|:
0.1,\ 0,\ 0.2,\ 0.2,\ 0.1
$$

Therefore:

$$
D=\frac{0.1+0+0.2+0.2+0.1}{5}
$$

$$
D=\frac{0.6}{5}
$$

$$
\boxed{D=0.12V}
$$

---

# 6.7 Variance

Variance gives a measure of how widely the measurements are distributed around their mean.

For a set of \(n\) measurements, the **sample variance** is:

$$
\boxed{
s^2=
\frac{\sum (x_i-\bar{x})^2}{n-1}
}
$$

For a complete population, the corresponding expression is:

$$
\boxed{
\sigma^2=
\frac{\sum (x_i-\mu)^2}{n}
}
$$

where:

- \(s^2\) = sample variance
- \(\sigma^2\) = population variance
- \(\bar{x}\) = sample mean
- \(\mu\) = population mean

For typical measurement experiments involving a limited number of repeated observations, the **sample formula** is commonly used.

---

# 6.8 Standard Deviation

Standard deviation is the square root of variance.

For a sample:

$$
\boxed{
s=
\sqrt{
\frac{\sum (x_i-\bar{x})^2}{n-1}
}
}
$$

It indicates the spread of measurements around the mean.

### Interpretation

- Small standard deviation → measurements are close together
- Large standard deviation → measurements are widely scattered

Therefore:

> **Standard deviation is a measure of the dispersion of repeated measurements.**

---

# 6.9 Example – Standard Deviation

Consider:

$$
10.2,\quad10.1,\quad10.3,\quad9.9,\quad10.0
$$

We already found:

$$
\bar{x}=10.1
$$

### Step 1: Calculate deviations

$$
+0.1,\quad0,\quad+0.2,\quad-0.2,\quad-0.1
$$

### Step 2: Square the deviations

$$
0.01,\quad0,\quad0.04,\quad0.04,\quad0.01
$$

Therefore:

$$
\sum d_i^2=0.10
$$

### Step 3: Calculate sample variance

$$
s^2=\frac{0.10}{5-1}
$$

$$
s^2=0.025
$$

### Step 4: Standard deviation

$$
s=\sqrt{0.025}
$$

$$
\boxed{s\approx0.158V}
$$

So the measurements have a standard deviation of approximately:

$$
\boxed{0.158V}
$$

---

# 6.10 Variance vs Standard Deviation

| Variance | Standard Deviation |
|---|---|
| Average squared deviation | Square root of variance |
| Unit is squared | Same unit as measurement |
| \(V^2\), for example | \(V\), for example |
| \(s^2\) | \(s\) |

Because standard deviation has the **same unit as the measurement**, it is often easier to interpret.

---

# 6.11 Standard Error of the Mean

When several measurements are averaged, we are interested in the uncertainty associated with the **mean**.

The standard error of the mean is:

$$
\boxed{
SE=\frac{s}{\sqrt{n}}
}
$$

where:

- \(s\) = sample standard deviation
- \(n\) = number of observations

### Important observation

As \(n\) increases:

$$
SE\downarrow
$$

Therefore, taking more independent measurements can improve the statistical estimate of the mean.

---

# 6.12 Example – Standard Error

From our previous example:

$$
s=0.158V
$$

and:

$$
n=5
$$

Therefore:

$$
SE=\frac{0.158}{\sqrt{5}}
$$

$$
\boxed{SE\approx0.071V}
$$

So the mean has a standard error of approximately:

$$
\boxed{0.071V}
$$

---

# 6.13 Normal Distribution of Random Errors

Random measurement errors often approximately follow a **normal (Gaussian) distribution** when many independent effects contribute to the measurement.

The familiar shape is:

```text
Frequency
   │
   │             /\
   │           /    \
   │         /        \
   │       /            \
   │_____/________________\_____ Error
                 0
```

The distribution is centered around the mean.

For an ideal normal distribution:

- Mean = central value
- Most observations occur near the mean
- Large deviations are less frequent

---

# 6.14 Mean and Random Error

Suppose repeated measurements are:

$$
9.8,\ 9.9,\ 10.0,\ 10.1,\ 10.2
$$

Their mean is:

$$
10.0
$$

Some values are above the mean and some below it.

Random errors may be positive or negative.

This is why averaging repeated measurements is useful.

---

# 6.15 Important Concept: More Measurements

Suppose we measure a quantity:

### Case A

5 readings

### Case B

50 readings

Generally, increasing the number of independent observations makes the estimate of the mean more stable.

The standard error follows:

$$
SE=\frac{s}{\sqrt{n}}
$$

Therefore:

$$
\boxed{\text{More observations} \Rightarrow \text{smaller standard error of the mean}}
$$

However, repeated measurements do **not automatically eliminate systematic errors**.

For example, if an instrument consistently reads 2 V high, taking 100 readings does not remove that offset.

---

# 6.16 Statistical Analysis – Complete Flow

```text
Repeated Measurements
          ↓
Calculate Mean
          ↓
Calculate Deviations
          ↓
Calculate Variance
          ↓
Calculate Standard Deviation
          ↓
Calculate Standard Error
          ↓
Estimate Reliability / Spread
```

---

# 6.17 Important Formulas

### Arithmetic Mean

$$
\boxed{
\bar{x}=\frac{\sum x_i}{n}
}
$$

### Deviation

$$
\boxed{
d_i=x_i-\bar{x}
}
$$

### Average Deviation

$$
\boxed{
D=\frac{\sum|d_i|}{n}
}
$$

### Sample Variance

$$
\boxed{
s^2=
\frac{\sum(x_i-\bar{x})^2}{n-1}
}
$$

### Sample Standard Deviation

$$
\boxed{
s=
\sqrt{
\frac{\sum(x_i-\bar{x})^2}{n-1}
}
}
$$

### Standard Error

$$
\boxed{
SE=\frac{s}{\sqrt n}
}
$$

---

# 6.18 Quick Worked Problem

Five measurements of resistance are:

$$
100.2,\quad99.8,\quad100.1,\quad99.9,\quad100.0\ \Omega
$$

### Mean

$$
\bar{x}
=
\frac{100.2+99.8+100.1+99.9+100.0}{5}
$$

$$
\boxed{\bar{x}=100.0\Omega}
$$

### Deviations

$$
+0.2,\ -0.2,\ +0.1,\ -0.1,\ 0
$$

### Squared deviations

$$
0.04,\ 0.04,\ 0.01,\ 0.01,\ 0
$$

Therefore:

$$
\sum d_i^2=0.10
$$

### Sample standard deviation

$$
s=\sqrt{\frac{0.10}{4}}
$$

$$
\boxed{s\approx0.158\Omega}
$$

### Standard error

$$
SE=\frac{0.158}{\sqrt5}
$$

$$
\boxed{SE\approx0.071\Omega}
$$

---

# ⭐ Exam Focus

### 2-Mark Questions

1. What is statistical analysis of measurement?
2. Define arithmetic mean.
3. Define deviation.
4. What is variance?
5. Define standard deviation.
6. What is standard error?
7. What is the significance of standard deviation?
8. Why are repeated measurements taken?

### 5-Mark Questions

1. Explain statistical analysis of repeated measurements.
2. Explain mean, deviation, variance and standard deviation.
3. Explain the significance of standard deviation in measurement.
4. Explain normal distribution of random errors.

### Numerical Questions ⭐

Be prepared to calculate:

1. Arithmetic mean
2. Deviation from mean
3. Average deviation
4. Variance
5. Standard deviation
6. Standard error

---

## One Important Distinction

Do not confuse:

$$
\boxed{\text{Standard Deviation}}
$$

with

$$
\boxed{\text{Standard Error}}
$$

**Standard deviation** → spread of individual measurements.

**Standard error** → uncertainty/variability associated with the estimated mean.

---

**Next → Step 7: Methods of Error Analysis**, where we'll distinguish **absolute/relative/percentage/limiting errors and systematic/random error treatment**, and work through numerical problems.
