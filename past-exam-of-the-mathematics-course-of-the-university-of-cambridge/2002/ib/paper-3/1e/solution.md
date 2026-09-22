<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

For $t\ne0$, ordinary differentiation of the two smooth components gives

$$
\boxed{f'(t)=\bigl(2t\sin(1/t)-\cos(1/t),\ 2t\cos(1/t)+\sin(1/t)\bigr)}.
$$

At zero, use the definition of the [derivative](../../../../../derivative.md) in the [Euclidean norm](../../../../../euclidean-norm.md):

$$
\left\|\frac{f(h)-f(0)}h\right\|=\|h(\sin(1/h),\cos(1/h))\|=|h|\longrightarrow0.
$$

Thus $f$ has [differentiability](../../../../../differentiability.md) everywhere and $\boxed{f'(0)=(0,0)}$. The two vectors $(\sin(1/t),\cos(1/t))$ and $(-\cos(1/t),\sin(1/t))$ are orthogonal unit vectors, so the squared [norm](../../../../../norm.md) of the displayed derivative is $4t^2+1$. Consequently

$$
\boxed{\|f'(a)-f'(0)\|=\sqrt{1+4a^2}>1\qquad(a\ne0)}.
$$

This [discontinuous derivative of a differentiable plane curve](../../../../../discontinuous-derivative-of-a-differentiable-plane-curve.md) also shows why componentwise scalar [mean value theorem](../../../../../mean-value-theorem.md) conclusions do not supply a single intermediate point reproducing an entire vector-valued difference quotient.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
