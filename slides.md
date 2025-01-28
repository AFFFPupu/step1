---
theme: frankfurt
infoLine: true
author: 拓课堂
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# some information about your slides (markdown enabled)
title: STEP课程 Lesson 1 Differentiation
date: 2025
info: |
  STEP Lesson 2: Calculus: Integration

# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
---

# 拓课堂 STEP 课程 
## Lesson 1

Calculus: Differentiation


---
section: 'STEP 介绍'
---

# STEP 1/2/3 分别是什么

<div v-click>

- <span class="text-red-500 font-bold">**STEP（第六学期考试）**</span> 是一种数学资格考试，旨在测试数学知识和技能，通常用于大学入学。

</div>

<div v-click>

- <span class="text-gray-500">**STEP 数学 1** 自 2021 年 6 月起不再提供。</span>
- <span class="text-green-500 font-bold">**STEP 数学 2 和 3** 仍然可用，其性质和风格在 2025 年保持不变。</span>

</div>

<div v-click>

- 规范假定考生具备先前的知识：
  <div v-click>
  
  - <span class="text-blue-500">STEP 2 假定考生已掌握数学 1 的内容。</span>
  - <span class="text-blue-500">STEP 3 假定考生已掌握数学 1 和 STEP 2 的内容。</span>
  
  </div>
</div>

---
transition: slide-up
---

# 考试规范

<div v-click>

- <span class="text-orange-500 font-bold">**基于 A Level 数学**</span>：遵循教育部 A Level 数学以及 AS 和 A Level 进阶数学规范的纯数学内容，但删除了一些主题并添加了一些主题。

</div>

<div v-click>

- **附加主题**：在规范中以粗体斜体标示，包括 STEP 2 和 3 中力学和概率/统计的所有附加主题。

</div>

<div v-click>

- **考试形式**：
  - **STEP 2 和 3**：<span class="text-purple-500 font-bold">3 小时的试卷</span>，分为三个部分：
    <div v-click>
    
    - <span class="text-blue-600">A 部分：纯数学（8 道题）</span>
    - <span class="text-green-600">B 部分：力学（2 道题）</span>
    - <span class="text-red-600">C 部分：概率/统计（2 道题）</span>
    
    </div>
</div>

---
transition: fade-out
---

# 评估与准备

<div v-click>

- <span class="text-purple-500 font-bold">**评估**</span>：基于得分最高的<span class="text-red-500 font-bold">六道题</span>进行评估，对于从任何部分尝试的题目数量没有限制。每道题的最高分均为<span class="text-green-500 font-bold">20 分</span>。

</div>

<div v-click>

- <span class="text-blue-500 font-bold">**重要提醒**</span>：
  - <span class="text-red-500">不提供公式</span>
  - <span class="text-red-500">不允许使用计算器和双语词典</span>

</div>

<div v-click>

- **知识测试**：题目可能会以不熟悉的方式测试考生应用数学知识的能力，需要洞察力、创造力和毅力。题目还可能涉及高年级 GCSE 数学的主题。

</div>

<div v-click>

- **规范包括符号部分，和卷面书写**。

</div>



---
section: 'Limits'
layout: center
class: text-center
---

# Let's Start with Calculus
## <span v-mark.red="1">Differentiation</span> - A Common Topic in STEP

<div class="mt-8" v-click>

STEP often tests <span v-mark.circle.orange="2">calculus concepts</span> in depth, particularly differentiation.

</div>

<div class="mt-4" v-click>

Understanding the <span v-mark.red="3">limits</span> and <span v-mark.circle="4">first principles</span> is crucial for:
- <span v-mark.red="5">STEP 2 Pure Mathematics</span> section
- Many mechanics questions
- Real-world application problems

</div>

---
layout: center
class: text-center
---

#  Limits
## Fundamental Theorems and Properties

---

# Theorem 1: Basic Limit Rules

<div class="grid grid-cols-2 gap-4">
<div class="text-lg">

If $\lim _{x \rightarrow c} f(x)$ and $\lim _{x \rightarrow c} g(x)$ both exist, then:

<v-clicks>

1. **Sum/Difference Rule**
   $$\lim _{x \rightarrow c}[f(x) \pm g(x)]=\lim _{x \rightarrow c} f(x) \pm \lim _{x \rightarrow c} g(x)$$

2. **Product Rule**
   $$\lim _{x \rightarrow c}[f(x) g(x)]=\lim _{x \rightarrow c} f(x) \cdot \lim _{x \rightarrow c} g(x)$$

3. **Quotient Rule**
   $$\lim _{x \rightarrow c}\left[\frac{f(x)}{g(x)}\right]=\frac{\lim _{x \rightarrow c} f(x)}{\lim _{x \rightarrow c} g(x)}$$
   (when denominator limit ≠ 0)

</v-clicks>

</div>
<div>

<div v-click class="mt-4 border-l-4 border-blue-500 pl-4 text-lg">

### Important Notes:
- "Exist" means:
  1. Definite value
  2. Not infinity
- c can be any number or ∞
- Rules apply for one-sided limits too

</div>

<div v-click class="mt-8 bg-green-50 p-4 rounded text-lg">

### Example:
$\lim _{x \rightarrow 2} (x^2 + 3x)$
= $\lim _{x \rightarrow 2} x^2 + \lim _{x \rightarrow 2} 3x$
= $4 + 6 = 10$

</div>

</div>
</div>

<style>
.katex {
  font: normal 1.21em KaTeX_Main, 'Times New Roman', serif;
}
</style>

---

# Theorem 2 & 3: Composition and Squeeze

<div class="grid grid-cols-2 gap-4">
<div>

### Composition Rule (Theorem 2)
<v-clicks>

If:
1. $$\lim_{x \rightarrow c} f(x) = A$$
2. $$\lim_{y \rightarrow A} g(y) = B$$
3. $$\text{Range of } f \subseteq \text{domain of } g$$

Then:
$$\lim_{x \rightarrow c} g(f(x)) = B$$

</v-clicks>

<div v-click class="mt-4 bg-yellow-50 p-4 rounded">

### Example:
$\lim_{x \rightarrow 0} \sin(\sin x)$
= $\sin(\lim_{x \rightarrow 0} \sin x)$
= $\sin(0) = 0$

</div>

</div>
<div>

### Squeeze Theorem (Theorem 3)
<v-clicks>

If on interval (a,b):
1. $$f(x) \leq h(x) \leq g(x)$$
2. $\lim_{x \rightarrow c} f(x) = A$ and  $\lim_{x \rightarrow c} g(x) = A$

Then:
$$\lim_{x \rightarrow c} h(x) = A$$

</v-clicks>

<div v-click class="mt-4 border-l-4 border-green-500 pl-4">

### Key Application:
Proving $\lim_{x \rightarrow 0} \frac{\sin x}{x} = 1$
- Uses geometric argument
- Crucial for calculus foundations

</div>

</div>
</div>

---

# Important Limits & Applications

<div class="grid grid-cols-2 gap-4">
<div>

### Fundamental Limits
<v-clicks>

1. $\lim_{n \rightarrow \infty}\left(1+\frac{1}{n}\right)^n = e$

2. $\lim_{x \rightarrow 0} \frac{\sin x}{x} = 1$

</v-clicks>

<div v-click class="mt-4 bg-blue-50 p-4 rounded">

### Applications:
- Euler's number definition
- Derivative of sin(x)
- Small angle approximations
- Taylor series expansions

</div>

</div>
<div>

### Proving $\lim_{x \rightarrow 0} \frac{\sin x}{x} = 1$
<v-clicks>

1. Use Squeeze Theorem
2. Geometric argument:
   - Area comparisons of:
     - Triangle
     - Sector
     - Inscribed angle

3. Key inequalities:
   $\cos x \leq \frac{\sin x}{x} \leq 1$
   for x → 0

</v-clicks>

</div>
</div>


---
section: 'Defn and 1st Principle'
---

# Differentiation

## Definition & Concept

<v-clicks>

- Differentiation measures how sensitive a function's output value is to changes in its input value
- It is a fundamental tool of calculus
- Example: The derivative of position with respect to time is velocity, measuring how quickly position changes

</v-clicks>

<div class="mt-8" v-click>

### Key Applications

- Rate of change problems
- Optimization (finding maximum/minimum values)
- Motion problems (velocity, acceleration)
- Tangent line calculations

</div>



---

# First Principle of Differentiation

<div class="grid grid-cols-2 gap-8">
<div v-click>

<Item title="Mathematical Definition">
<div class="text-center my-4">

$f^{\prime}(x)=\lim _{h \rightarrow 0} \frac{f(x+h)-f(x)}{h}$

</div>

This is the formal definition of the derivative, derived from the concept of instantaneous rate of change.
</Item>

</div>
<div v-click>

<Item title="Key Interpretations">

- **Rate of Change**: This limit represents the instantaneous rate of change of the function
- **Geometric Meaning**: The slope of the tangent line at a point
- **Physical Applications**: 
  - Velocity (derivative of position)
  - Acceleration (derivative of velocity)
  - Rate of growth/decay

</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
</style>


---

# Your Turn: Power Function Differentiation

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Problem">

Try to find $\frac{d}{dx}(x^2)$ using first principle:

<div class="text-center my-4">

$\begin{aligned}
f(x) &= x^2 \\[1ex]
f'(x) &= \lim_{h \to 0}\frac{f(x+h)-f(x)}{h} \\[1ex]
&= \lim_{h \to 0}\frac{(x+h)^2-x^2}{h}
\end{aligned}$

</div>



</Item>

</div>
<div>

<v-clicks>

<Item title="Hints">

1. Expand $(x+h)^2 = x^2 + 2xh + h^2$
2. Subtract $x^2$ from numerator
3. Factor out $h$ from numerator
4. What happens to terms with $h$ as $h \to 0$?

</Item>

<div class="mt-4">
<Item title="Solution">

<div class="text-center my-4">

$\begin{aligned}
&= \lim_{h \to 0}\frac{x^2 + 2xh + h^2-x^2}{h} \\[1ex]
&= \lim_{h \to 0}\frac{2xh + h^2}{h} \\[1ex]
&= \lim_{h \to 0}(2x + h) \\[1ex]
&= 2x
\end{aligned}$

</div>

</Item>
</div>

</v-clicks>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>



---

# First Principle: Power Functions

<div class="grid grid-cols-2 gap-4">
<div v-click>

<Item title="Step-by-Step Derivation">

For $f(x)=x^n$, let's find $f'(x)$ using first principle:

$\begin{aligned}
f'(x) &= \lim_{h \to 0}\frac{f(x+h)-f(x)}{h} \\[1ex]
&= \lim_{h \to 0}\frac{(x+h)^n-x^n}{h} \\[1ex]
&= \lim_{h \to 0}\frac{\sum_{r=0}^n \binom{n}{r}x^{n-r}h^r-x^n}{h} \\[1ex]
&= \lim_{h \to 0}\left(\binom{n}{1}x^{n-1} + \binom{n}{2}x^{n-2}h + \cdots\right) \\[1ex]
&= nx^{n-1}
\end{aligned}$

</Item>

</div>
<div v-click>

<Item title="Key Points">

- Uses binomial expansion of $(x+h)^n$
- All terms with $h^1$ or higher → 0 as $h \to 0$
- Only term with $h^1$ survives in limit
- $\binom{n}{1} = n$ gives final coefficient

</Item>

<div class="mt-4">
<Item title="Examples">

- If $n=2$: $\frac{d}{dx}(x^2) = 2x$
- If $n=3$: $\frac{d}{dx}(x^3) = 3x^2$
- If $n=\frac{1}{2}$: $\frac{d}{dx}(\sqrt{x}) = \frac{1}{2}x^{-\frac{1}{2}}$

</Item>
</div>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
</style>




---

# Your Turn: Exponential & Natural Log

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Exponential Function">

Try to find $\frac{d}{dx}(e^x)$ using first principle:

<div class="text-center my-4">

$\begin{aligned}
f'(x) &= \lim_{h \to 0}\frac{e^{x+h}-e^x}{h} \\[1ex]
&= \lim_{h \to 0}\frac{e^x(e^h-1)}{h} \\[1ex]
&= e^x\lim_{h \to 0}\frac{e^h-1}{h}
\end{aligned}$

<div v-click class="mt-2 text-blue-500">
Can you show that:
<div class="text-center my-2">

$\displaystyle\lim_{h \to 0}\frac{e^h-1}{h} = 1$?

</div>
</div>

</div>
</Item>

</div>
<div>

<Item title="Natural Logarithm">

Try to find $\frac{d}{dx}(\ln x)$ using first principle:

<div class="text-center my-4">

$\begin{aligned}
f'(x) &= \lim_{h \to 0}\frac{\ln(x+h)-\ln x}{h} \\[1ex]
&= \lim_{h \to 0}\frac{\ln(1+\frac{h}{x})}{h} \\[1ex]
&= \frac{1}{x}\lim_{h \to 0}\frac{\ln(1+h)}{h}
\end{aligned}$

<div v-click class="mt-2 text-blue-500">
Can you show that:
<div class="text-center my-2">

$\displaystyle\lim_{h \to 0}\frac{\ln(1+h)}{h} = 1$?

</div>
</div>

</div>
</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>




---

# Exponential Function: Detailed Derivation

<div class="grid grid-cols-2 gap-4">
<div v-click>

<Item title="Key Steps">

For $f(x)=e^x$, we showed:

<div class="text-center my-4">

$\begin{aligned}
f'(x) &= e^x\lim_{h \to 0}\frac{e^h-1}{h} \\[1ex]
&= e^x \cdot 1 \\[1ex]
&= e^x
\end{aligned}$

</div>

But why is $\displaystyle\lim_{h \to 0}\frac{e^h-1}{h} = 1$?

</Item>

</div>
<div>

<v-clicks>

<Item title="Proof Using the Definition of e">

Recall that $e$ is defined as:

$e = \lim_{n \to \infty}(1 + \frac{1}{n})^n$

Let $h = \frac{1}{n}$. Then as $n \to \infty$, $h \to 0$:

$\begin{aligned}
\lim_{h \to 0}\frac{e^h-1}{h} &= \lim_{h \to 0}\frac{(1+h)^{\frac{1}{h}}-1}{h} \\[1ex]
&= 1
\end{aligned}$

</Item>



</v-clicks>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>




---

# Natural Log: Detailed Derivation

<div class="grid grid-cols-2 gap-4">
<div v-click>

<Item title="Key Steps">

For $f(x)=\ln x$, we showed:

<div class="text-center my-4">

$\begin{aligned}
f'(x) &= \lim_{h \to 0}\frac{\ln(x+h)-\ln x}{h} \\[1ex]
&= \lim_{h \to 0}\frac{\ln(1+\frac{h}{x})}{h} \\[1ex]
&= \frac{1}{x}\lim_{h \to 0}\frac{\ln(1+h)}{h}
\end{aligned}$

</div>

But why is $\displaystyle\lim_{h \to 0}\frac{\ln(1+h)}{h} = 1$?

</Item>

</div>
<div>

<v-clicks>

<Item title="Proof Using Properties of ln">

Let $y = \lim_{h \to 0}\frac{\ln(1+h)}{h}$

Then $e^y = e^{\lim_{h \to 0}\frac{\ln(1+h)}{h}}$

$\begin{aligned}
e^y &= \lim_{h \to 0}(1+h)^{\frac{1}{h}} \\[1ex]
&= e
\end{aligned}$

Therefore, $y = 1$

</Item>



</v-clicks>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>




---

# Homework: Trigonometric Derivatives

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Problem 1: Sine Function">

Prove that $\frac{d}{dx}\sin x = \cos x$ using first principle.

<div class="text-center my-4">

$\begin{aligned}
f'(x) &= \lim_{h \to 0}\frac{\sin(x+h)-\sin x}{h}
\end{aligned}$

</div>

<div v-click class="mt-2">
<Item title="Hints">

1. Use addition formula: $\sin(A+B) = \sin A\cos B + \cos A\sin B$
2. Group terms with $\sin x$
3. You'll need these limits:
   - $\lim_{h \to 0}\frac{\sin h}{h} = 1$
   - $\lim_{h \to 0}\frac{\cos h-1}{h} = 0$

</Item>
</div>

</Item>

</div>
<div>

<Item title="Problem 2: Cosine Function">

Prove that $\frac{d}{dx}\cos x = -\sin x$ using first principle.

<div class="text-center my-4">

$\begin{aligned}
g'(x) &= \lim_{h \to 0}\frac{\cos(x+h)-\cos x}{h}
\end{aligned}$

</div>

<div v-click class="mt-2">
<Item title="Hints">

1. Use addition formula: $\cos(A+B) = \cos A\cos B - \sin A\sin B$
2. Group terms with $\cos x$
3. Use the same limits as Problem 1
4. Watch for the negative sign!

</Item>
</div>

</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>




---

# Real STEP Question: Osculating Circle

<div class="grid gap-4">
<div>

<Item title="STEP 2010 Paper 2, Q1">

Let $P$ be a given point on a given curve $C$. The osculating circle to $C$ at $P$ is defined to be the circle that satisfies the following two conditions at $P$:

1. It touches $C$
2. The rate of change of its gradient is equal to the rate of change of the gradient of $C$

Find the centre and radius of the osculating circle to the curve:

$y = 1-x+\tan x$

at the point on the curve with $x$-coordinate $\frac{1}{4}\pi$.

</Item>






</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>








---

# Solution: Osculating Circle (STEP 2010 P2 Q1)

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Key Concepts">

For a curve $C$ and its osculating circle at point $P$:

1. Same coordinates $(x,y)$
2. Same gradient $\frac{dy}{dx}$
3. Same rate of change of gradient $\frac{d^2y}{dx^2}$

<div class="mt-4">
<div class="text-center my-4">

For curve $y=1-x+\tan x$:
$\begin{aligned}
\frac{dy}{dx} &= -1+\sec^2 x \\[1ex]
\frac{d^2y}{dx^2} &= 2\sec^2 x\tan x
\end{aligned}$

</div>
</div>

</Item>

</div>
<div>

<Item title="Solution Method">

For circle $(x-a)^2+(y-b)^2=r^2$:

1. At $x=\frac{\pi}{4}$:
   - $y = 2-\frac{\pi}{4}$
   - $\frac{dy}{dx} = 1$
   - $\frac{d^2y}{dx^2} = 4$

2. Solve equations:
   - $(\frac{\pi}{4}-a)^2+(2-\frac{\pi}{4}-b)^2=r^2$
   - $\frac{dy}{dx}=-\frac{(x-a)}{(y-b)}=1$
   - $\frac{d^2y}{dx^2}=-\frac{4}{2(y-b)}=4$

</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>

---

# Answer & Verification

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Final Answer">

The osculating circle has:

<div class="text-center my-4">

$\begin{aligned}
\text{Centre} &= (\frac{\pi}{4}-\frac{1}{2}, \frac{5}{2}-\frac{\pi}{4}) \\[2ex]
\text{Radius} &= \frac{1}{\sqrt{2}}
\end{aligned}$

</div>

</Item>

</div>
<div>

<Item title="Verification">

You can verify by checking:

1. Point $P = (\frac{\pi}{4}, 2-\frac{\pi}{4})$ lies on both curves
2. Gradients match at $P$: $\frac{dy}{dx} = 1$
3. Second derivatives match at $P$: $\frac{d^2y}{dx^2} = 4$

<div v-click>

<div class="mt-4 text-blue-500">
Key insight: The radius of curvature formula confirms our answer:

$R = \frac{[1+(\frac{dy}{dx})^2]^{3/2}}{|\frac{d^2y}{dx^2}|} = \frac{1}{\sqrt{2}}$
</div>

</div>

</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>








---
section: Basics
---
# Basic Derivatives (1/2)

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Power Functions">

For any real number $a$:

<div class="text-center my-4">

$\frac{d}{dx}x^a = ax^{a-1}$

</div>

Special cases:
- $\frac{d}{dx}x = 1$
- $\frac{d}{dx}\sqrt{x} = \frac{1}{2\sqrt{x}}$
- $\frac{d}{dx}\frac{1}{x} = -\frac{1}{x^2}$

</Item>



</div>
<div>

<Item title="Trigonometric Functions">

<div class="text-center my-4">

$\begin{aligned}
\frac{d}{dx}\sin(x) &= \cos(x) \\[1ex]
\frac{d}{dx}\cos(x) &= -\sin(x) \\[1ex]
\frac{d}{dx}\tan(x) &= \sec^2(x) \\[1ex]
&= \frac{1}{\cos^2(x)} \\[1ex]
&= 1 + \tan^2(x)
\end{aligned}$

</div>

</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>

---

# Basic Derivatives (2/2)

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Inverse Trigonometric Functions">

<div class="text-center my-4">

$\begin{aligned}
\frac{d}{dx}\arcsin(x) &= \frac{1}{\sqrt{1-x^2}}, & -1 < x < 1 \\[2ex]
\frac{d}{dx}\arccos(x) &= -\frac{1}{\sqrt{1-x^2}}, & -1 < x < 1 \\[2ex]
\frac{d}{dx}\arctan(x) &= \frac{1}{1+x^2}
\end{aligned}$

</div>

</Item>

</div>
<div>

<Item title="Key Points to Remember">

- Domain restrictions are important
- These are building blocks for chain rule
- Memorize these for STEP efficiency
- Look for patterns:
  - $\arcsin$ and $\arccos$ are negatives
  - $\arctan$ connects to $1+x^2$
  - Power rule works for any real power

</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>








---
section: Rules
---

# Differentiation Rules

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Chain Rule">

For composite functions $h(x)=g(f(x))$:

<div class="text-center my-4">

$\begin{aligned}
h'(x) &= g'(f(x))f'(x) \\[2ex]
\frac{dy}{dx} &= \frac{dy}{du} \times \frac{du}{dx}
\end{aligned}$

where $y=g(u)$ and $u=f(x)$

</div>

<div v-click>

Example: If $y = \sin(x^2)$
$\frac{dy}{dx} = \cos(x^2) \cdot 2x$

</div>

</Item>

</div>
<div>

<Item title="Product Rule">

For product of functions:

<div class="text-center my-4">

$\begin{aligned}
(f(x)g(x))' &= f'(x)g(x) + f(x)g'(x) \\[2ex]
\frac{d}{dx}(uv) &= u\frac{dv}{dx} + v\frac{du}{dx}
\end{aligned}$

</div>

<div v-click>

Example: If $y = x\sin(x)$
$\frac{dy}{dx} = 1\cdot\sin(x) + x\cdot\cos(x)$

</div>

</Item>

</div>
</div>



<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>








---

# Differentiation Rules (continued)

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Quotient Rule">

For quotient of functions $\frac{f(x)}{g(x)}$ or $\frac{u}{v}$:

<div class="text-center my-4">

$\begin{aligned}
\left(\frac{f(x)}{g(x)}\right)' &= \frac{f'(x)g(x) - f(x)g'(x)}{(g(x))^2} \\[2ex]
\frac{d}{dx}\left(\frac{u}{v}\right) &= \frac{v\frac{du}{dx} - u\frac{dv}{dx}}{v^2}
\end{aligned}$

</div>

</Item>

</div>
<div>

<Item title="Memory Tips">

1. "Bottom times derivative of top minus top times derivative of bottom"
2. All over bottom squared
3. Remember the minus sign in the middle
4. Denominator must be non-zero

<div v-click>

Example: If $y = \frac{x}{\sin(x)}$

$\begin{aligned}
\frac{dy}{dx} &= \frac{\sin(x) \cdot 1 - x\cdot\cos(x)}{\sin^2(x)}
\end{aligned}$

</div>

</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>








---

# Real STEP Question: Function Analysis

<div class="grid gap-4">
<div>

<Item title="STEP 2000 Paper 1, Q7">

Let $f(x)$ be defined as:

<div class="text-center my-4">

$f(x)=ax-\frac{x^3}{1+x^2}$

</div>

where $a$ is a constant.

Show that, if $a \geqslant \frac{9}{8}$, then $f'(x) \geqslant 0$ for all $x$.

</Item>



</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>

---
# Solution: Function Analysis (STEP 2000 P1 Q7)

<div class="grid grid-cols-2 gap-4">
<div>

<Item title="Finding f'(x)">

Using quotient rule:

<div class="text-center my-4">

$\begin{aligned}
f'(x) &= a - \frac{(1+x^2)(3x^2) - x^3(2x)}{(1+x^2)^2} \\[1ex]
&= a - \frac{3x^2 + x^4}{(1+x^2)^2} \\[1ex]
&= \frac{a(1+x^2)^2 - (3x^2 + x^4)}{(1+x^2)^2} \\[1ex]
&= \frac{a + 2ax^2 + ax^4 - 3x^2 - x^4}{(1+x^2)^2}
\end{aligned}$

</div>

</Item>

</div>
<div>

<Item title="Proving Non-negativity">

For $f'(x) \geqslant 0$, numerator must be non-negative:

<div class="text-center my-4">

$a + (2a-3)x^2 + (a-1)x^4 \geqslant 0$

</div>

This quadratic in $x^2$ is minimized when:

<div class="text-center my-4">

$x^2 = \frac{3-2a}{2(1-a)}$

</div>

Minimum value is $a - \frac{9}{8}$

Therefore, if $a \geqslant \frac{9}{8}$, then $f'(x) \geqslant 0$ for all $x$.

</Item>

</div>
</div>

<style>
.katex {
  font: normal 1.1em KaTeX_Main, 'Times New Roman', serif;
}
.katex-display {
  overflow: hidden;
}
</style>

