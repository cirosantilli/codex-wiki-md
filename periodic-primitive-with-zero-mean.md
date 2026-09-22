# Periodic primitive with zero mean

↑ **Parent:** [Periodic extension](periodic-extension.md)

For $h\in L^1(0,1)$ with integral zero, $Ph$ is the unique [absolutely continuous function](absolutely-continuous-function.md) with $(Ph)'=-h$, equal endpoint values, and integral zero. The first formula gives the [derivative](derivative.md); zero integral of $h$ gives equal endpoint values, while the added constant makes the mean zero. Uniqueness follows because the difference of two such primitives has zero [weak derivative](weak-derivative.md) and therefore is constant, then its mean is zero. Its [periodic extension](periodic-extension.md) has [distributional derivative](distributional-derivative.md) $-\overline h$, with no endpoint [Dirac delta distribution](dirac-delta-function.md).

Writing $Rh(x)=x\int_0^1h-\int_0^xh$, the same operator on zero-mean inputs is $Ph=Rh-\int_0^1Rh$. For arbitrary $h\in L^1(0,1)$,

$$
\|Rh\|_{L^1}\leq\frac12\|h\|_{L^1},\qquad
\left\|Rh-\int_0^1Rh\right\|_{L^1}\leq\|h\|_{L^1}.
$$

The first inequality follows from the integral kernel $x-\mathbf1_{\{t<x\}}$, whose absolute value has integral $(t^2+(1-t)^2)/2\leq1/2$ in $x$. The second follows by the [triangle inequality](triangle-inequality.md). This bound permits arbitrarily many iterations without increasing the [L1 space](l1-space.md) norm.

```
Target: Rapid distributional decay of periodic oscillations. Parent: Weak convergence of distributions. Intended file: distribution-theory.bigb.
```

## ↑ Ancestors (8)

1. [Periodic extension](periodic-extension.md)
2. [Periodic function](periodic-function.md)
3. [Function](function-split.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
