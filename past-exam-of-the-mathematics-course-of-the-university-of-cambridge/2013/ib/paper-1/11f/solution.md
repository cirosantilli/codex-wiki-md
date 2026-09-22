<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

For [uniform convergence](../../../../../uniform-convergence.md) to $k$ on $A$, for every $\eta>0$ there is $N$ such that $|k_n(x)-k(x)|<\eta$ for all $n\ge N$ and all $x\in A$. The bound $|\sin(nx)/\sqrt n|\le1/\sqrt n$ proves [uniform convergence](../../../../../uniform-convergence.md) to zero, whereas its [derivative](../../../../../derivative.md) is $\sqrt n\cos(nx)$. On an interval containing zero these [derivatives](../../../../../derivative.md) diverge at zero, so they cannot converge uniformly. This supplies a counterexample to differentiating a uniformly convergent sequence without additional hypotheses.

For [uniform derivative convergence with an anchored value](../../../../../uniform-derivative-convergence-with-an-anchored-value.md), put $g=\lim k_n'$ and $a=\lim k_n(x_0)$. A uniform limit of continuous functions is continuous. The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) gives

$$
k_n(x)=k_n(x_0)+\int_{x_0}^x k_n'(t)\,dt.
$$

Thus $k_n(x)\to k(x)=a+\int_{x_0}^x g(t)\,dt$, with error bounded by

$$
|k_n(x_0)-a|+|x-x_0|\sup_A|k_n'-g|.
$$

This is uniform on bounded subintervals, and on all of $A$ if it is bounded. The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) now gives $k'=g$, so $k$ is continuously differentiable. For an unbounded $A$, no global [uniform convergence](../../../../../uniform-convergence.md) of $k_n$ follows merely from the displayed hypotheses, but local [uniform convergence](../../../../../uniform-convergence.md) and the claimed differentiability do.

For the series, use partial sums and differentiate their individual terms:

$$
\frac{d}{dx}\frac{x^n\sin(nx)}{n^3+1}
=\frac{n x^{n-1}\sin(nx)+n x^n\cos(nx)}{n^3+1}.
$$

For $|x|\le1$, their absolute values are at most $2n/(n^3+1)$, a summable bound. The [Weierstrass M-test](../../../../../weierstrass-m-test.md) makes the [derivative](../../../../../derivative.md) series uniformly convergent, while every partial sum is zero at $x=0$. The anchored-value result therefore proves **continuous differentiability on $(-1,1)$**, with [derivative](../../../../../derivative.md) equal to the displayed termwise [derivative](../../../../../derivative.md) series.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
