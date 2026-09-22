<h1 id="14e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The nonzero poles are

$$
t=\pm ia_n,\qquad a_n=\frac\pi2(2n+1),\qquad n\geq0.
$$

Their paired residues sum to

$$
-(-1)^na_n^{s-1}\cos\frac{\pi s}{2}.
$$

The paired [series](../../../../../../series-mathematics.md) converges for $\operatorname{Re}s<1$ by the alternating-series test, and absolutely for $\operatorname{Re}s<0$. Therefore

$$
\sum\operatorname{Res}=-\cos\frac{\pi s}{2}
\left(\frac\pi2\right)^{s-1}\beta(1-s).
$$

Using the stated contour closure, the Hankel [integral](../../../../../../integral.md) is $-2\pi i$ times this sum. Substitution into part (a) gives

$$
\beta(s)=\Gamma(1-s)\cos\frac{\pi s}{2}
\left(\frac\pi2\right)^{s-1}\beta(1-s).
$$

Now $1/\Gamma(1-s)=\Gamma(s)\sin(\pi s)/\pi$ and $\sin(\pi s)=2\sin(\pi s/2)\cos(\pi s/2)$, so

$$
\boxed{\beta(1-s)=\Gamma(s)\left(\frac\pi2\right)^{-s}
\sin\frac{\pi s}{2}\,\beta(s)}.
$$

It was derived on a nonempty half-plane. Both sides have analytic continuations, with the apparent gamma poles cancelled by the sine factor or the trivial zeros from part (b); the [identity theorem](../../../../../../identity-theorem.md) therefore extends it to every $s\in\mathbb C$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
