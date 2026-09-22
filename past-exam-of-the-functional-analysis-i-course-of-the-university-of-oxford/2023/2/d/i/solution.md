<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $D=C([-1,1])$, restricted to $(-1,1)$ and regarded as a [linear subspace](../../../../../vector-subspace.md) of $L^p((-1,1))$. The [density of continuous functions in Lp on an interval](../../../../../density-of-continuous-functions-in-lp-on-an-interval.md) says that $D$ is a [dense subspace](../../../../../dense-subspace.md) whenever $1\leq p<\infty$.

For $g\in D$, the [supremum norm](../../../../../supremum-norm.md) gives

$$
|T_hg|\leq h^{-1/p'}\int_{-h}^h|g(x)|\,dx
\leq2\|g\|_\infty h^{1-1/p'}=2\|g\|_\infty h^{1/p}\longrightarrow0.
$$

In particular $D\subseteq Y$, with zero limit. Part (c), together with $D$ being a [dense subspace](../../../../../dense-subspace.md), implies $Y=X$. To identify the limit throughout $X$, for $f\in X$ and $g\in D$ use

$$
|T_hf|\leq M\|f-g\|_p+2\|g\|_\infty h^{1/p},\qquad M=2^{1/p'}.
$$

First choose $g$ in the [dense subspace](../../../../../dense-subspace.md) to make the first term arbitrarily small, then let $h\to0^+$. This is [convergence on a dense subspace under a uniform operator bound](../../../../../convergence-on-a-dense-subspace-under-a-uniform-operator-bound.md), and proves

$$
\boxed{Tf=\lim_{h\to0^+}T_hf=0\quad(f\in L^p((-1,1))),\qquad\|T\|=0.}
$$

The zero [linear functional](../../../../../linear-functional.md) belongs to the [continuous dual space](../../../../../continuous-dual-space-split.md) $X^*$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis I course of the University of Oxford](../../../../split.md)
6. [Functional analysis I course of the University of Oxford](../../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
