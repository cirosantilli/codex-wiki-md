# Secant method

↑ **Parent:** [Root finding](root-finding.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Secant_method)

The [secant method](secant-method.md) approximates a [zero of a function](zero-of-a-function.md) by repeatedly taking the zero of a [secant line](secant-line.md) through the two most recent sampled points. The formula follows by setting the line $f(x_k)+(x-x_k)(f(x_k)-f(x_{k-1}))/(x_k-x_{k-1})$ equal to zero. It requires distinct sampled positions and a nonzero difference of sampled values, unless a [root](root-of-a-root-system.md) has already been found. After initialization it needs one new [function](function-split.md) evaluation per step. Unlike [bisection](bisection-method.md), it need not retain a bracket. For a sufficiently smooth [function](function-split.md) near a simple [root](root-of-a-root-system.md), its usual local [order of convergence](order-of-convergence.md) is $(1+\sqrt5)/2$.[§3.8(iii), Secant Method, following equation 3.8.6](nist-digital-library-of-mathematical-functions/3-8-nonlinear-equations.md)

## ↑ Ancestors (6)

1. [Root finding](root-finding.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [3.8 Nonlinear Equations](nist-digital-library-of-mathematical-functions/3-8-nonlinear-equations.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/5/a/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/5/a/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/5/a/iii/solution.md)
- [Secant method](secant-method.md)
