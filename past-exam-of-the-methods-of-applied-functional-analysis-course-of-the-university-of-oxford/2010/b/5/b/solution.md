<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [weak solution](../../../../../weak-solution.md) is $u\in H_0^1(\Omega)$ such that

$$
\int_\Omega\nabla u\cdot\nabla\varphi=\int_\Omega f(u)\varphi\qquad(\varphi\in H_0^1(\Omega)).
$$

Let $M_f=\|f\|_\infty$ and define the [Nemytskii operator](../../../../../nemytskii-operator.md) $N(v)=f\circ v$ on $L^2(\Omega)$. It satisfies $\|N(v)\|_2\leq M_f|\Omega|^{1/2}$. It is continuous in $L^2$: from any sequence $v_j\to v$ in $L^2$, every subsequence has a further subsequence converging [almost everywhere](../../../../../almost-everywhere.md); continuity and boundedness of $f$, followed by the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md), give convergence of the corresponding $N(v_j)$ in $L^2$. This subsequence criterion proves continuity of the whole sequence.

For $h\in L^2$, the [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) defines the inverse Dirichlet solution map $Sh\in H_0^1$ by $\int\nabla(Sh)\cdot\nabla\varphi=\int h\varphi$. Testing with $Sh$ and using the [Poincaré inequality](../../../../../poincare-inequality.md) yields

$$
\|\nabla Sh\|_2\leq C_P\|h\|_2,\qquad\|Sh\|_2\leq C_P^2\|h\|_2.
$$

The [Rellich-Kondrachov compactness theorem](../../../../../rellich-kondrachov-theorem.md) makes $S:L^2\to L^2$ compact. Therefore $T=S\circ N$ is a [nonlinear compact operator](../../../../../nonlinear-compact-operator.md) and its image lies in the closed $L^2$ ball of radius $R=1+C_P^2M_f|\Omega|^{1/2}$. This ball is nonempty, closed, bounded and convex. The [Schauder fixed-point theorem](../../../../../schauder-fixed-point-theorem.md) gives $u=Tu$. Since $Tu\in H_0^1$, its defining identity is exactly the required [weak formulation](../../../../../weak-formulation.md). Thus **a weak solution exists**. This is the [bounded semilinear Dirichlet existence theorem](../../../../../bounded-semilinear-dirichlet-existence-theorem.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
