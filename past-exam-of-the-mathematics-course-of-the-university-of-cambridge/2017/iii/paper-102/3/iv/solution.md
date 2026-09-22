<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The PDF uses $V=\mathbb C^{2n+1}$ for $\mathfrak{so}_{2n+1}$; the TeX incorrectly turns this into a power of two. The [crystal of the defining odd-orthogonal representation](../../../../../../crystal-of-the-defining-odd-orthogonal-representation.md) is the chain with weights $\varepsilon_1,\ldots,\varepsilon_n,0,-\varepsilon_n,\ldots,-\varepsilon_1$. Label its vertices $1,\ldots,n,0,\bar n,\ldots,\bar1$. Its directed edge colors are

$$
1,2,\ldots,n-1,n,n,n-1,\ldots,2,1.
$$

In particular the short-root string $n\to0\to\bar n$ has two edges of color $n$.

For a full drawing of the [tensor product of crystals](../../../../../../tensor-product-of-crystals.md) in any rank, take every ordered pair of chain vertices $(a,b)$. Let $\varepsilon_i(b)$ count incoming edges of color $i$ along its string, and let $\varphi_i(a)$ count outgoing ones. We use the convention

$$
\widetilde f_i(a\otimes b)=
\begin{cases}\widetilde f_i(a)\otimes b,&\varphi_i(a)>\varepsilon_i(b),\\
a\otimes\widetilde f_i(b),&\varphi_i(a)\leq\varepsilon_i(b),\end{cases}
$$

omitting an edge when the indicated operator vanishes. This [crystal tensor-product rule](../../../../../../crystal-tensor-product-rule.md) specifies every vertex and every edge; the raising rule uses $\geq$ for its first-factor branch. The picture shows the chain and all 25 tensor vertices for $n=2$, with connected components distinguished by node color.

<a id="3/iv/image-the-type-b2-defining-crystal-and-its-tensor-square"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102-b2-tensor-crystal.png)

**[Figure 2](#3/iv/image-the-type-b2-defining-crystal-and-its-tensor-square). The type-B2 defining crystal and its tensor square**.

For $n\geq2$, the three [highest-weight vectors](../../../../../../highest-weight-vector.md) of the tensor crystal are $1\otimes1$, $1\otimes2$ and $1\otimes\bar1$. They have weights $2\varepsilon_1$, $\varepsilon_1+\varepsilon_2$ and zero. There are no others: a highest tensor vertex must have highest first factor, and the string inequalities then restrict its second factor to these three vertices. Therefore

$$
\boxed{V\otimes V=L(2\varepsilon_1)\oplus L(\varepsilon_1+\varepsilon_2)\oplus L(0).}
$$

The summands are the traceless [symmetric square](../../../../../../symmetric-square.md), the [exterior square](../../../../../../exterior-square.md) (the [Adjoint representation](../../../../../../adjoint-representation-of-a-lie-algebra.md)), and the invariant scalar line. Their dimensions are $(2n+1)(n+1)-1$, $n(2n+1)$ and one, summing to $(2n+1)^2$. For $n\geq3$ the first two [highest weights](../../../../../../highest-weight-of-a-representation.md) are $2\omega_1,\omega_2$; for $n=2$ they are $2\omega_1,2\omega_2$. For $n=1$, the three tensor highest vertices are $1\otimes1,1\otimes0,1\otimes\bar1$, giving $L(4\omega_1)\oplus L(2\omega_1)\oplus L(0)$ of dimensions $5,3,1$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
