<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Give the real root span an [inner product](../../../../../../inner-product.md) with $\varepsilon_1,\varepsilon_2$ orthonormal. The [B2 root system](../../../../../../b2-root-system.md) consists of four short roots on the coordinate axes and four long roots on the diagonals. Choose the long-first [simple roots](../../../../../../simple-root.md)

$$
\boxed{\alpha_1=\varepsilon_1-\varepsilon_2,\qquad\alpha_2=\varepsilon_2.}
$$

The [positive roots](../../../../../../positive-root.md) are $\alpha_1,\alpha_2,\alpha_1+\alpha_2=\varepsilon_1$, and $\alpha_1+2\alpha_2=\varepsilon_1+\varepsilon_2$. The corresponding simple reflections are

$$
s_1(x,y)=(y,x),\qquad s_2(x,y)=(x,-y).
$$

They generate every signed permutation of the two coordinates. Thus the [Weyl group](../../../../../../weyl-group.md) has order eight and is the symmetry group of a square; every element sends $(x,y)$ to $(\pm x,\pm y)$ or $(\pm y,\pm x)$, with independent signs.

<a id="2/b/image-the-b2-root-system-with-long-first-simple-roots-and-all-four-positive-roots"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-5-b2-roots.png)

**[Figure 1](#2/b/image-the-b2-root-system-with-long-first-simple-roots-and-all-four-positive-roots). The B2 root system with long-first simple roots and all four positive roots**.

Since $\alpha_1,\alpha_2$ form an integral basis of $\mathbb Z^2$, the [root lattice](../../../../../../root-lattice.md) is $Q=\mathbb Z\varepsilon_1\oplus\mathbb Z\varepsilon_2$. The [simple coroots](../../../../../../simple-coroot.md) are $\alpha_1^\vee=\varepsilon_1-\varepsilon_2$ and $\alpha_2^\vee=2\varepsilon_2$. Therefore the [weight lattice](../../../../../../weight-lattice.md) is

$$
\boxed{P=\{(x,y):x-y\in\mathbb Z,\ 2y\in\mathbb Z\}
=\mathbb Z^2\ \cup\ \big((\mathbb Z+\tfrac12)\times(\mathbb Z+\tfrac12)\big).}
$$

Solving $\langle\Lambda_i,\alpha_j^\vee\rangle=\delta_{ij}$ gives the [fundamental weights](../../../../../../fundamental-weight.md)

$$
\boxed{\Lambda_1=\varepsilon_1,\qquad\Lambda_2=\tfrac12(\varepsilon_1+\varepsilon_2).}
$$

The cone of [dominant weights](../../../../../../dominant-weight.md) is

$$
\boxed{P^+=\{a\Lambda_1+b\Lambda_2:a,b\in\mathbb Z_{\ge0}\}
=\{(x,y)\in P:x\ge y\ge0\}.}
$$

Indeed $a=x-y$ and $b=2y$ are exactly the two simple-coroot pairings. This describes representations of the Lie algebra, or of its simply connected [Spin group](../../../../../../spin-group.md); half-integral weights are allowed. For representations descending to $\operatorname{SO}(5)$ itself, the weight must lie in $\mathbb Z^2$, equivalently $b$ must be even.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
