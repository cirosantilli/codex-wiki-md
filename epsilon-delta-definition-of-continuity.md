# Epsilon-delta definition of continuity

↑ **Parent:** [Continuous function](continuous-function.md)

A [function](function-split.md) $f:D\to\mathbb R$ is [continuous](continuous-function.md) at $a\in D$ when

$$
\text{for every }\varepsilon>0\text{ there is a }\delta>0\text{ such that}
\quad x\in D,\ |x-a|<\delta\ \Longrightarrow\ |f(x)-f(a)|<\varepsilon.
$$

First choose the required output tolerance $\varepsilon$; then choose an input tolerance $\delta$ that works for every allowed [function input](function-input.md) in that window. Picking a different $\delta$ separately after seeing each $x$ would reverse the [quantifiers](quantifier.md) and lose this guarantee. There is no need to exclude $x=a$, because the output difference is then zero.

At an isolated point of the [domain of a function](domain-of-a-function.md), choose a small enough window that its only allowed [function input](function-input.md) is $a$. This proves [continuity](continuous-function.md) there directly. At a point with arbitrarily close other inputs, the same definition is the [limit of a function](limit-of-a-function.md) condition $f(x)\to f(a)$. For [metric spaces](metric-space.md), replace the two [absolute values](absolute-value.md) by their [distance functions](metric.md); for arbitrary [topological spaces](topological-space.md), the corresponding definition is a [continuous map](continuous-map.md).

The input tolerance may depend on $a$. A single choice valid everywhere on the [domain of a function](domain-of-a-function.md) is the stronger requirement of [uniform continuity](uniform-continuity.md). The [continuous function](continuous-function.md) $x\mapsto x^2$ on $\mathbb R$ shows the difference: for any proposed $\delta>0$, the points $a=1/\delta$ and $b=a+\delta/2$ have $|b-a|<\delta$, yet $b^2-a^2=1+\delta^2/4>1$. Thus the fixed output tolerance $\varepsilon=1$ admits no global input tolerance on the [real line](real-line.md).

**Table of contents**

- [Continuity bounds for the square function](continuity-bounds-for-the-square-function.md)

## ↑ Ancestors (8)

1. [Continuous function](continuous-function.md)
2. [Limit of a function](limit-of-a-function.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Continuity and differentiability thresholds for a damped oscillation](continuity-and-differentiability-thresholds-for-a-damped-oscillation.md)
- [Continuous function](continuous-function.md)
- [Continuous functions preserve convergent sequences](continuous-functions-preserve-convergent-sequences.md)
- [Discontinuity of a function](discontinuity-of-a-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/19/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1/19/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/19/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/19/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/19/a/i/solution.md)
- [Uniformly continuous function](uniformly-continuous-function.md)
