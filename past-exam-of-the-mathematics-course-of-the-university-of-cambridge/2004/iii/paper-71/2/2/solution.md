<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $n\ge1$ and $1<p<\infty$. The [Lp space](../../../../../../lp-space.md) is strictly convex because $z\mapsto|z|^p$ is strictly convex: for distinct unit functions its pointwise midpoint inequality is strict on a set of positive measure, hence integration gives [norm](../../../../../../norm.md) strictly below one. The finite-dimensional [linear subspace](../../../../../../vector-subspace.md) $\mathcal T_{n-1}$ has a best approximant: any minimizing sequence is bounded by $\|t\|_p\le\|f-t\|_p+\|f\|_p$, and finite-dimensional [compactness](../../../../../../compact-space.md) gives a convergent subsequence whose limit minimizes the continuous error. Uniqueness follows from part 1.

Write that unique minimizer as $t^*$ and its residual as $F=f-t^*$. Translation on the circle preserves the [Lp norm](../../../../../../lp-norm.md). Since $f(x+2\pi/n)=f(x)$, the translated [polynomial](../../../../../../polynomial-split.md) $t^*(x+2\pi/n)$ is another minimizer. Uniqueness forces

$$
t^*(x+2\pi/n)=t^*(x),\qquad F(x+2\pi/n)=F(x).
$$

Also $f(x+\pi/n)=-f(x)$. Therefore the [polynomial](../../../../../../polynomial-split.md) $-t^*(x+\pi/n)$ has residual $-F(x+\pi/n)$, with the same [norm](../../../../../../norm.md) as $F$, and is again a minimizer. Hence

$$
t^*(x)=-t^*(x+\pi/n),\qquad F(x)=-F(x+\pi/n).
$$

To extract the consequence, write the [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) as $t^*(x)=\sum_{|\ell|\le n-1}c_\ell e^{i\ell x}$. The first identity gives $(e^{2\pi i\ell/n}-1)c_\ell=0$. Only $\ell=0$ in the indicated frequency range is a multiple of $n$, so $t^*$ is constant. The second identity makes this constant its own negative and therefore zero. Thus the [lower-frequency Lp approximation to a single harmonic](../../../../../../lower-frequency-lp-approximation-to-a-single-harmonic.md) is

$$
\boxed{t^*_{n-1}\equiv0,\qquad E_{n-1,p}(f)=\|a\cos nx+b\sin nx\|_p.}
$$

For $n=1$ the space already consists only of constants, and the negative-translation argument gives the same result.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
