<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\mathcal W_n$ for the deterministic [set](../../../../../../set-split.md) of $n$-step [self-avoiding walks](../../../../../../self-avoiding-walk.md) from $0$. Each uses $n$ distinct [edges](../../../../../../edge-of-a-graph.md), so [independence](../../../../../../independent-random-variables.md) gives

$$
\kappa_n=\sum_{w\in\mathcal W_n}\mathbf1_{\{w\text{ open}\}},\qquad\mathbb E_p\kappa_n=c_np^n.
$$

For $n\geq1$, the function $t\mapsto t^{1/n}$ on $[0,\infty)$ is a [concave function](../../../../../../concave-function.md). The [Jensen inequality](../../../../../../jensen-s-inequality.md) gives the [root-moment bound for open self-avoiding walks](../../../../../../root-moment-bound-for-open-self-avoiding-walks.md)

$$
\mathbb E_p(\kappa_n^{1/n})\leq(\mathbb E_p\kappa_n)^{1/n}=p c_n^{1/n}.
$$

Equivalently, the [Lyapunov moment inequality](../../../../../../lyapunov-moment-inequality.md) compares exponents $1/n$ and $1$, both strictly positive. Taking the [limit superior](../../../../../../limit-superior.md) and the [connective constant](../../../../../../connective-constant.md) limit proves

$$
\boxed{\limsup_{n\to\infty}\mathbb E_p(\kappa_n^{1/n})\leq p\mu}.
$$

This includes $p=0$ and $n=1$. No [independence](../../../../../../independent-random-variables.md) between the different [self-avoiding walk](../../../../../../self-avoiding-walk.md) indicators is asserted or needed.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
