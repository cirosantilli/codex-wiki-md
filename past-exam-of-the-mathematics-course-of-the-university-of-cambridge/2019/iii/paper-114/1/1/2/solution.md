<h1 id="1/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [cellular chain complex](../../../../../../../cellular-chain-complex.md) for either space has one cell in dimensions $0,2,3,4$, with the only nonzero differential equal to multiplication by $p$ from degree three to degree two. The [universal coefficient theorem for cohomology](../../../../../../../universal-coefficient-theorem-for-cohomology.md) therefore gives, for both $X$ and $Y$,

$$
H^j(-;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&j=0,4,\\
\mathbb Z/p,&j=3,\\
0,&\text{otherwise}.
\end{cases}
$$

Every product of positive-degree classes vanishes for dimensional reasons, so

$$
\boxed{H^*(X;\mathbb Z)\cong H^*(Y;\mathbb Z)\text{ as graded rings}.}
$$

Their modulo-$p$ [cohomology rings](../../../../../../../cohomology-ring.md) distinguish them. Let $u\in H^2(X;\mathbb F_p)$ be the class restricting to the standard generator on $\mathbb{CP}^2$. The attaching map has degree $p$, so its cellular coboundary vanishes modulo $p$; the classes in degrees two and four restrict isomorphically to those of $\mathbb{CP}^2$. Hence $u^2\ne0$ in $H^4(X;\mathbb F_p)$. In $Y=M(\mathbb Z/p,2)\vee S^4$, the degree-two class comes from the three-dimensional [Moore space](../../../../../../../moore-space-algebraic-topology.md), so its square is zero; products between distinct wedge summands also vanish. The [mod-p cup-square obstruction to a homotopy equivalence](../../../../../../../mod-p-cup-square-obstruction-to-a-homotopy-equivalence.md) now proves

$$
\boxed{X\not\simeq Y.}
$$

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 114](../../../../paper-114-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
