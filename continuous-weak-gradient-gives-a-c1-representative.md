# Continuous weak gradient gives a C1 representative

↑ **Parent:** [Weak derivative](weak-derivative.md)

If a locally integrable function has [weak derivatives](weak-derivative.md) represented by a continuous [vector field](vector-field.md) $g$, it has a representative $U\in C^1$ with $\nabla U=g$. The assertion is local, so work on a ball compactly contained in the domain and regularize using a [mollifier](mollifier.md). The regularizations satisfy the segment identity $u_\varepsilon(x)-u_\varepsilon(y)=\int_0^1\nabla u_\varepsilon(y+t(x-y))\cdot(x-y)\,dt$. Averaging over a smaller ball in $y$ fixes the additive constant through local $L^1$ convergence. The gradients converge uniformly on compact sets, so the averaged identity gives local uniform convergence to $U$. Passing to the limit on each segment then gives $U(x+h)-U(x)-g(x)\cdot h=o(|h|)$. Continuity of $g$ proves that $U$ is continuously [differentiable](differentiable-function.md).

## ↑ Ancestors (7)

1. [Weak derivative](weak-derivative.md)
2. [Distributional derivative](distributional-derivative.md)
3. [Distribution theory](distribution-theory-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-methods-of-applied-functional-analysis-course-of-the-university-of-oxford/2010/a/2/b/ii/solution.md)
