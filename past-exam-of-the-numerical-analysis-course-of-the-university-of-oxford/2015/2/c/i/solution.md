<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $f\in C^{n+1}[a,b]$ and reorder the [interpolation nodes](../../../../../interpolation-node.md) increasingly as $x_0<\cdots<x_n$. The [polynomial interpolation error](../../../../../polynomial-interpolation-error.md) $e=f-p_n$ vanishes at all of them. [Rolle's theorem](../../../../../rolle-theorem.md) supplies

$$
\eta_i\in(x_{i-1},x_i),\qquad e'(\eta_i)=0,\qquad i=1,\ldots,n.
$$

These $n$ points are distinct because their containing [intervals](../../../../../interval-mathematics.md) are disjoint. Thus $q=p_n'$ is a [polynomial](../../../../../polynomial-split.md) of [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $n-1$ that interpolates the [function](../../../../../function-split.md) $f'$ at the [interpolation nodes](../../../../../interpolation-node.md) $\eta_1,\ldots,\eta_n$.

Apply the [polynomial interpolation error](../../../../../polynomial-interpolation-error.md) theorem to $f'$ with these $n$ [interpolation nodes](../../../../../interpolation-node.md). Since the $n$th [derivative](../../../../../derivative.md) of $f'$ is $f^{(n+1)}$, for every $x\in[a,b]$ there is a $\xi_x\in(a,b)$ with

$$
\boxed{f'(x)-q(x)=\frac{f^{(n+1)}(\xi_x)}{n!}\widehat\pi_n(x),\qquad
\widehat\pi_n(x)=\prod_{i=1}^n(x-\eta_i).}
$$

For $x=\eta_i$ the equality is zero on both sides; otherwise the same auxiliary-[function](../../../../../function-split.md) and repeated-[Rolle's theorem](../../../../../rolle-theorem.md) proof applies. This also covers $n=1$, where $q$ is a [constant polynomial](../../../../../constant-polynomial.md) and the proof is the ordinary [mean value theorem](../../../../../mean-value-theorem.md) for $f'$.

Writing $M=\max_{[a,b]}|f^{(n+1)}|$ gives the genuine error bound

$$
\boxed{|f'(x)-q(x)|\leq\frac M{n!}\prod_{i=1}^n|x-\eta_i|
\leq\frac M{n!}(b-a)^n.}
$$

The first formula is sharper, but its intermediate [interpolation nodes](../../../../../interpolation-node.md) depend on $f$; the last bound eliminates those unknown locations. This is [derivative interpolation error from Rolle points](../../../../../derivative-interpolation-error-from-rolle-points.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
