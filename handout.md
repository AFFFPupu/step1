
# STEP Lesson 1: Calculus – Differentiation

**Handout for Students**

*(Feel free to write your name here and take notes throughout.)*

---

## Table of Contents

1. [Overview of STEP 2/3](#overview-of-step-23)
2. [Exam Format & Preparation](#exam-format--preparation)
3. [Limits](#limits)
   - [Theorem 1: Basic Limit Rules](#theorem-1-basic-limit-rules)
   - [Theorem 2: Composition Rule](#theorem-2-composition-rule)
   - [Theorem 3: Squeeze Theorem](#theorem-3-squeeze-theorem)
   - [Important Limits & Applications](#important-limits--applications)
4. [Differentiation](#differentiation)
   - [First Principle of Differentiation](#first-principle-of-differentiation)
   - [Power Functions via First Principle](#power-functions-via-first-principle)
   - [Exponential & Logarithmic Derivatives](#exponential--logarithmic-derivatives)
   - [Homework: Trigonometric Derivatives](#homework-trigonometric-derivatives)
5. [Real STEP Example: Osculating Circle (2010 P2 Q1)](#real-step-example-osculating-circle-2010-p2-q1)
6. [Basic Derivatives (Reference)](#basic-derivatives-reference)
7. [Differentiation Rules](#differentiation-rules)
8. [Real STEP Example: Function Analysis (2000 P1 Q7)](#real-step-example-function-analysis-2000-p1-q7)

Throughout this handout, **blank spaces** are provided for you to take notes and work out solutions.

---

## Overview of STEP 2/3

- **STEP（Sixth Term Examination Paper）** is a mathematics examination, often used for university admissions in the UK.
- **STEP Mathematics 1** is no longer offered since June 2021.
- **STEP Mathematics 2 and 3** remain with the same structure in 2025.
- **Content Assumptions**:
  - STEP 2 assumes knowledge of A-level Mathematics (and what was in STEP 1).
  - STEP 3 assumes knowledge of A-level Mathematics and Further Mathematics (and what was in STEP 2).

**Notes:**
```





```


## Exam Format & Preparation

- Based on **A Level Mathematics** content (some topics removed, some added).
- **STEP 2 & 3** each is a 3-hour paper, split into:
  - **Section A:** Pure Mathematics (8 questions)
  - **Section B:** Mechanics (2 questions)
  - **Section C:** Probability/Statistics (2 questions)
- Grading is based on the best 6 answers (each worth up to 20 marks).
- **Important**:
  - No formula booklet provided.
  - No calculators or bilingual dictionaries allowed.
- Questions may test familiar knowledge in unfamiliar ways, requiring insight and creativity.

**Notes:**
```



```

---

## Limits

### Theorem 1: Basic Limit Rules

If \(\lim_{x \to c} f(x)\) and \(\lim_{x \to c} g(x)\) both exist, then:

1. **Sum/Difference Rule**  
   \[
   \lim_{x \to c} [f(x) \pm g(x)] 
   = \lim_{x \to c} f(x) 
   \pm \lim_{x \to c} g(x)
   \]

2. **Product Rule**  
   \[
   \lim_{x \to c} [f(x) g(x)] 
   = \left(\lim_{x \to c} f(x)\right) 
     \cdot \left(\lim_{x \to c} g(x)\right)
   \]

3. **Quotient Rule**  
   \[
   \lim_{x \to c} \frac{f(x)}{g(x)} 
   = \frac{\lim_{x \to c} f(x)}{\lim_{x \to c} g(x)}
   \]
   (assuming the denominator limit \(\neq 0\))

**Notes:**
```



```

---

### Theorem 2: Composition Rule

If:
1. \(\lim_{x \to c} f(x) = A\)
2. \(\lim_{y \to A} g(y) = B\)
3. Range of \(f\) is in the domain of \(g\)

Then:
\[
\lim_{x \to c} g(f(x)) = B.
\]

**Example**:  
\(\lim_{x \to 0} \sin(\sin x)\)  
\(= \sin\bigl(\lim_{x \to 0} \sin x \bigr)\)  
\(= \sin(0) = 0.\)

---

### Theorem 3: Squeeze Theorem

If, on an interval, we have
\[
f(x) \leq h(x) \leq g(x)
\]
and
\[
\lim_{x \to c} f(x) = \lim_{x \to c} g(x) = A,
\]
then
\[
\lim_{x \to c} h(x) = A.
\]

**Key Application**: \(\lim_{x \to 0} \frac{\sin x}{x} = 1\).

**Notes:**
```



```

---

### Important Limits & Applications

- \(\displaystyle \lim_{n \to \infty}\left(1+\frac{1}{n}\right)^n = e.\)
- \(\displaystyle \lim_{x \to 0} \frac{\sin x}{x} = 1.\)

These are crucial for defining \(e\), finding the derivative of \(\sin x\), small-angle approximations, and Taylor expansions.

**Notes:**
```




```

---

## Differentiation

**Differentiation** measures how a function changes as its input changes.  

- **Physical Interpretation**: Rate of change, slope of tangent, velocity, acceleration, etc.
- **Mathematical Definition** (First Principle):
  \[
  f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}.
  \]

**Key Applications**:
- Rate of change problems
- Optimization
- Motion (velocity, acceleration)
- Tangent lines

**Notes:**
```





```

---

### First Principle of Differentiation

\[
f'(x)=\lim _{h \rightarrow 0} \frac{f(x+h)-f(x)}{h}.
\]

- **Interpretation**: Instantaneous rate of change or slope of the tangent line at a point.
- **Examples**:
  - Velocity = derivative of position.
  - Acceleration = derivative of velocity.

**Notes:**
```





```

---

### Power Functions via First Principle

**Example**: \(\frac{d}{dx}(x^2)\)

\[
\begin{aligned}
f'(x) &= \lim_{h \to 0}\frac{(x+h)^2 - x^2}{h} \\
      &= \lim_{h \to 0}\frac{x^2 + 2xh + h^2 - x^2}{h} \\
      &= \lim_{h \to 0}(2x + h) \\
      &= 2x.
\end{aligned}
\]

General result for \(f(x) = x^n\):
\[
\frac{d}{dx} x^n = nx^{n-1}.
\]

**Notes:**
```








```

---

### Exponential & Logarithmic Derivatives

1. \(\frac{d}{dx}(e^x)\)

   Using first principle:
   \[
   \frac{d}{dx}(e^x) = e^x.
   \]
   Key limit used:
   \(\displaystyle \lim_{h \to 0}\frac{e^h - 1}{h} = 1.\)

2. \(\frac{d}{dx}(\ln x)\)

   Using first principle:
   \[
   \frac{d}{dx}(\ln x) = \frac{1}{x}.
   \]
   Key limit used:
   \(\displaystyle \lim_{h \to 0}\frac{\ln(1+h)}{h} = 1.\)

**Notes:**
```







```

---

### Homework: Trigonometric Derivatives

**Problem 1**: Prove from first principles that
\[
\frac{d}{dx}\sin x = \cos x.
\]

**Hints**:
1. \(\sin(x+h) = \sin x \cos h + \cos x \sin h\).
2. Use the limits \(\lim_{h\to 0} \frac{\sin h}{h} = 1\) and \(\lim_{h\to 0} \frac{\cos h - 1}{h} = 0\).

---

**Problem 2**: Prove from first principles that
\[
\frac{d}{dx}\cos x = -\sin x.
\]

**Hints**:
1. \(\cos(x+h) = \cos x \cos h - \sin x \sin h\).
2. Similar limit usage as above.

**Space for your working/notes**:
```

















```

---

## Real STEP Example: Osculating Circle (STEP 2010, Paper 2 Q1)

**Question**:

A curve \(C\) is given by \(y = 1 - x + \tan x\). Let \(P\) be the point on this curve with \(x\)-coordinate \(\frac{\pi}{4}\). The **osculating circle** at \(P\) is the circle that:
1. Touches \(C\) at \(P\).
2. Has the same rate of change of gradient as \(C\) at \(P\).

**Task**: Find the centre and radius of the osculating circle at \(P\).

**Space for your working/notes**:
```
























```

*(The detailed solution typically involves matching coordinates, first derivative, and second derivative with that of a general circle. You might also use the radius of curvature formula \(R = \frac{[1+(y')^2]^{3/2}}{|y''|}\).)*

---

## Basic Derivatives (Reference)

1. **Power Functions**  
   \(\frac{d}{dx} x^a = a x^{a-1}\).

2. **Trigonometric Functions**  
   \[
   \frac{d}{dx}\sin x = \cos x, \quad
   \frac{d}{dx}\cos x = -\sin x, \quad
   \frac{d}{dx}\tan x = \sec^2 x.
   \]

3. **Inverse Trigonometric Functions**  
   \[
   \frac{d}{dx}\arcsin x = \frac{1}{\sqrt{1-x^2}}, \quad
   \frac{d}{dx}\arccos x = -\frac{1}{\sqrt{1-x^2}}, \quad
   \frac{d}{dx}\arctan x = \frac{1}{1+x^2}.
   \]

4. **Exponential & Logarithm**  
   \[
   \frac{d}{dx} e^x = e^x, \quad
   \frac{d}{dx}\ln x = \frac{1}{x}.
   \]

---

## Differentiation Rules

### Chain Rule

For \(h(x) = g(f(x))\):
\[
h'(x) = g'(f(x)) \cdot f'(x).
\]

**Example**: \(\frac{d}{dx}[\sin(x^2)] = \cos(x^2) \cdot 2x.\)

---

### Product Rule

\[
\frac{d}{dx}[u \cdot v] = u \frac{dv}{dx} + v \frac{du}{dx}.
\]

**Example**: \(\frac{d}{dx}[x \sin x] = \sin x + x \cos x.\)

---

### Quotient Rule

\[
\frac{d}{dx}\left(\frac{u}{v}\right) 
= \frac{v\,\frac{du}{dx} - u\,\frac{dv}{dx}}{v^2}.
\]

**Example**: \(\frac{d}{dx}\left[\frac{x}{\sin x}\right] 
= \frac{\sin x \cdot 1 - x \cdot \cos x}{(\sin x)^2}.\)

**Notes:**
```

```

---

## Real STEP Example: Function Analysis (STEP 2000, Paper 1 Q7)

**Question**:  
Let \(f(x) = a x - \frac{x^3}{1 + x^2}\), where \(a\) is a constant. Show that if \(a \ge \frac{9}{8}\), then \(f'(x) \ge 0\) for all \(x\).

**Outline**:
1. Differentiate \(f(x)\) using the quotient rule.
2. Show that the resulting expression is non-negative for \(a \ge \frac{9}{8}\).

**Space for your working/notes**:
```














```

---

# End of Handout

**Remember**: Practice questions from past STEP papers often involve applying these derivative rules in non-standard ways. Focus on mastering first principles, the chain/product/quotient rules, and practicing problems under exam conditions.

**Good Luck!**
