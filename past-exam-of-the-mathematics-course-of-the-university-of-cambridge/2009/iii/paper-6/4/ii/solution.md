<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Number the [simple roots](../../../../../../simple-root.md) so that $\alpha_1$ is short and $\alpha_2$ is long. In a Euclidean plane take

$$
\alpha_1=(1,0),\qquad \alpha_2=(-3/2,\sqrt3/2).
$$

Their squared lengths are $1,3$, and their angle is $150^\circ$. The positive [roots of a root system](../../../../../../root-of-a-root-system.md) are

$$
\alpha_1,\quad\alpha_2,\quad\alpha_1+\alpha_2,\quad2\alpha_1+\alpha_2,\quad3\alpha_1+\alpha_2,\quad3\alpha_1+2\alpha_2;
$$

their negatives give the remaining six roots of the [G2 root system](../../../../../../g2-root-system.md). The three short positive [roots of a root system](../../../../../../root-of-a-root-system.md) are $\alpha_1$, $\alpha_1+\alpha_2$, and $2\alpha_1+\alpha_2$.

Solving $\langle\omega_j,\alpha_i^\vee\rangle=\delta_{ij}$ gives the [fundamental weights](../../../../../../fundamental-weight.md)

$$
\boxed{\omega_1=2\alpha_1+\alpha_2=(1/2,\sqrt3/2),\qquad \omega_2=3\alpha_1+2\alpha_2=(0,\sqrt3).}
$$

In this case both [fundamental weights](../../../../../../fundamental-weight.md) are themselves roots; the diagram marks their locations on the two hexagons.

<a id="4/ii/image-the-twelve-g2-roots-with-short-first-simple-roots-and-fundamental-weights-marked-on-the-short-and-long-hexagons"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-6-g2-roots.png)

**[Figure 3](#4/ii/image-the-twelve-g2-roots-with-short-first-simple-roots-and-fundamental-weights-marked-on-the-short-and-long-hexagons). The twelve G2 roots with short-first simple roots and fundamental weights marked on the short and long hexagons**.

Let $a=n_1$ and $b=n_2$. Relative to the [simple coroots](../../../../../../simple-coroot.md), the six positive [coroots](../../../../../../coroot.md), in the root order above, have coordinates

$$
(1,0),\quad(0,1),\quad(1,3),\quad(2,3),\quad(1,1),\quad(1,2).
$$

For example, $\alpha_1+\alpha_2$ has squared length one, so its [coroot](../../../../../../coroot.md) is $2\alpha_1+2\alpha_2=\alpha_1^\vee+3\alpha_2^\vee$; the analogous length computation gives each other entry. Since $\rho=\omega_1+\omega_2$, the pairings of $\lambda+\rho$ with these [coroots](../../../../../../coroot.md) are $a+1$, $b+1$, $a+3b+4$, $2a+3b+5$, $a+b+2$, and $a+2b+3$. Their values at $a=b=0$ multiply to $1\cdot1\cdot4\cdot5\cdot2\cdot3=120$. The [Weyl dimension formula](../../../../../../weyl-dimension-formula.md) therefore yields the [G2 dimension polynomial](../../../../../../g2-dimension-polynomial.md)

$$
\boxed{\dim L(a\omega_1+b\omega_2)=\frac{(a+1)(b+1)(a+b+2)(a+2b+3)(a+3b+4)(2a+3b+5)}{120}.}
$$

This holds for all nonnegative [integers](../../../../../../integer.md) $a,b$. In particular it gives [dimensions](../../../../../../dimension-vector-space.md) $7$ and $14$ for $L(\omega_1)$ and $L(\omega_2)$, and $27$ for $L(2\omega_1)$. Reversing the numbering of the [simple roots](../../../../../../simple-root.md) would interchange $a,b$ in the [polynomial](../../../../../../polynomial-split.md), so the short-first convention matters.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
