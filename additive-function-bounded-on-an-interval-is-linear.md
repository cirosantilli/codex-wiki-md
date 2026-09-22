# Additive function bounded on an interval is linear

↑ **Parent:** [Additive function](additive-function.md)

Let $f:\mathbb R\to\mathbb R$ be an [additive function](additive-function.md). Suppose $|f(x)|\leq M$ for all $x$ in a nondegenerate [interval](interval-mathematics.md) $(a,b)$, meaning $a<b$. Then $f$ is [continuous](continuous-function.md) everywhere and $f(x)=xf(1)$. A finite bound on even one such [interval](interval-mathematics.md) is enough; a bound at one isolated point is not.

Here is a proof outline that turns a finite bound into arbitrarily small outputs. Set $z=(a+b)/2$ and $\delta=(b-a)/2$. If $|h|<\delta$, then both $z$ and $z+h$ lie in $(a,b)$, so [Cauchy's functional equation](cauchy-s-functional-equation.md) gives

$$
|f(h)|=|f(z+h)-f(z)|\leq2M.
$$

Given $\varepsilon>0$, choose a positive [integer](integer-split.md) $N$ with $2M/N<\varepsilon$. For $|h|<\delta/N$, the argument $Nh$ lies in $(-\delta,\delta)$, and [rational homogeneity of an additive function](rational-homogeneity-of-an-additive-function.md) gives

$$
|f(h)|=\frac{|f(Nh)|}{N}\leq\frac{2M}{N}<\varepsilon.
$$

This proves [continuity](continuous-function.md) at zero. Now [additive function continuous at one point is linear](additive-function-continuous-at-one-point-is-linear.md) completes the proof. The key mechanism is that repeated [addition](addition.md) magnifies a tiny input without escaping the bounded region, forcing the original output to be small.

## ↑ Ancestors (7)

1. [Additive function](additive-function.md)
2. [Cauchy's functional equation](cauchy-s-functional-equation.md)
3. [Functional equation](functional-equation.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Discontinuous additive function](discontinuous-additive-function.md)
