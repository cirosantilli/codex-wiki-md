# Log-sum-exp function

↑ **Parent:** [Convex optimization](convex-optimization-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Log-sum-exp_function)

For $z\in\mathbb R^m$ and $\beta>0$, the scaled log-sum-exp function is

$$
\operatorname{LSE}_\beta(z)
=\frac1\beta\log\sum_{i=1}^m e^{\beta z_i}.
$$

It is a smooth [convex function](convex-function.md) satisfying

$$
\max_i z_i\leq\operatorname{LSE}_\beta(z)
\leq\max_i z_i+\frac{\log m}{\beta}.
$$

**Table of contents**

- [Smooth maximum](smooth-maximum.md)

## ↑ Ancestors (5)

1. [Convex optimization](convex-optimization-split.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/5/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/6/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-339/1/c/solution.md)
- [Smooth maximum](smooth-maximum.md)
