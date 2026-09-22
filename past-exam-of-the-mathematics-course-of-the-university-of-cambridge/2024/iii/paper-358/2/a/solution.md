<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [projection-valued measure](../../../../../../projection-valued-measure.md) on the [Borel sets](../../../../../../borel-set.md) of $\mathbb C$ is a map $E$ into the [orthogonal projections](../../../../../../orthogonal-projection.md) on a [separable Hilbert space](../../../../../../separable-hilbert-space.md) $\mathcal H$ such that

$$
E(\varnothing)=0,\qquad E(\mathbb C)=I,\qquad
E(B\cap C)=E(B)E(C),
$$

and for pairwise disjoint $B_j$,

$$
E\!\left(\bigcup_jB_j\right)v=\sum_jE(B_j)v
$$

for every $v\in\mathcal H$, with convergence in norm.

The [spectral theorem for normal operators on a separable Hilbert space](../../../../../../spectral-theorem-for-normal-operators-on-a-separable-hilbert-space.md) states that a bounded [normal operator](../../../../../../normal-operator.md) $A$ has a unique projection-valued measure supported on $\operatorname{Sp}(A)$ for which

$$
\boxed{A=\int_{\operatorname{Sp}(A)}z\,dE(z).}
$$

More generally, the [Borel functional calculus for a normal operator](../../../../../../borel-functional-calculus-for-a-normal-operator.md) is

$$
f(A)=\int f(z)\,dE(z).
$$

For $v,w\in\mathcal H$, the [scalar spectral measures](../../../../../../scalar-spectral-measure.md) are

$$
\mu_{v,w}(B)=\langle E(B)v,w\rangle,
\qquad
\mu_v=\mu_{v,v}.
$$

If $A$ is [self-adjoint](../../../../../../self-adjoint-operator.md), its spectrum and hence the support of $E$ lie in $\mathbb R$. Moreover,

$$
\mu_v(B)=\langle E(B)v,v\rangle=\|E(B)v\|^2\geq0,
$$

so $\mu_v$ is a [positive measure](../../../../../../positive-measure.md), and

$$
\boxed{\mu_v(\mathbb R)=\langle Iv,v\rangle=\|v\|^2.}
$$

The paper prints total mass $\|v\|$; with the standard definition it is $\|v\|^2$, so the unsquared norm is a typographical error.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
