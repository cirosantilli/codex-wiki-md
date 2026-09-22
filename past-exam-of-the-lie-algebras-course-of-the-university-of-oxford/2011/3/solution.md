<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Equip the finite-dimensional real vector space $V$ with a positive-definite [inner product](../../../inner-product-split.md). A reduced crystallographic [root system](../../../root-system.md) is a finite set $R\subset V\setminus\{0\}$ spanning $V$ such that, for every $\alpha\in R$,

$$
R\cap\mathbb R\alpha=\{\alpha,-\alpha\},\qquad
s_\alpha(R)=R,\qquad
\frac{2(\beta,\alpha)}{(\alpha,\alpha)}\in\mathbb Z\quad(\beta\in R),
$$

where $s_\alpha(v)=v-2(v,\alpha)\alpha/(\alpha,\alpha)$ is the [orthogonal reflection](../../../reflection-in-a-hyperplane.md) in $\alpha^\perp$. The [Weyl group](../../../weyl-group.md) is $W(R)=\langle s_\alpha:\alpha\in R\rangle$. It permutes the finite set $R$. Its action is faithful because $R$ spans $V$: an element fixing every [root](../../../root-of-a-root-system.md) fixes every vector. Hence it embeds in the finite [symmetric group](../../../symmetric-group.md) of $R$ and **is finite**.

A [Cartan subalgebra](../../../cartan-subalgebra.md) is a nilpotent self-normalizing [Lie subalgebra](../../../lie-subalgebra.md). For a finite-dimensional complex [semisimple Lie algebra](../../../semisimple-lie-algebra-split.md) it is equivalently a maximal toral subalgebra: a maximal abelian subalgebra whose elements have [diagonalizable](../../../diagonalizable-matrix.md) adjoint actions. The commuting semisimple operators $\operatorname{ad}(h)$ give the [root-space decomposition](../../../root-space-decomposition.md)

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in R}\mathfrak g_\alpha,\qquad
\mathfrak g_\alpha=\{x:[h,x]=\alpha(h)x\text{ for every }h\in\mathfrak h\}.
$$

The nonzero weights $\alpha$ are the roots. Their real span inside the complex dual $\mathfrak h^*$, with the positive-definite real [inner product](../../../inner-product-split.md) induced by the [Killing form](../../../killing-form.md), is the Euclidean space in which they form a reduced crystallographic [root system](../../../root-system.md). In particular one uses this real span, rather than treating all of $\mathfrak h^*$ as a real vector space of twice the [rank](../../../rank-one-quadratic-form.md).

For the specified [Special orthogonal Lie algebra](../../../special-orthogonal-lie-algebra.md), put $\bar i=7-i$. The [matrix](../../../matrix.md) relation is $x_{ij}=-x_{\bar j,\bar i}$. Thus its diagonal [Cartan subalgebra](../../../cartan-subalgebra.md) consists of

$$
H(t)=\operatorname{diag}(t_1,t_2,t_3,-t_3,-t_2,-t_1).
$$

Let $\varepsilon_i(H(t))=t_i$. The [matrix](../../../matrix.md) units satisfy $[H,E_{ij}]=(d_i-d_j)E_{ij}$, where $d=(t_1,t_2,t_3,-t_3,-t_2,-t_1)$. A [basis](../../../basis.md) of [root](../../../root-of-a-root-system.md) vectors is supplied, for $1\le i<j\le3$, by

$$
\begin{array}{c|c}
\text{root}&\text{root vector}\\\hline
\varepsilon_i-\varepsilon_j&E_{ij}-E_{\bar j,\bar i}\\
-\varepsilon_i+\varepsilon_j&E_{ji}-E_{\bar i,\bar j}\\
\varepsilon_i+\varepsilon_j&E_{i,\bar j}-E_{j,\bar i}\\
-\varepsilon_i-\varepsilon_j&E_{\bar j,i}-E_{\bar i,j}
\end{array}
$$

These are twelve independent off-diagonal matrices. Together with the three diagonal generators, they account for the full [dimension](../../../dimension-vector-space.md) $6\cdot5/2=15$, so no further roots occur. Consequently

$$
\boxed{R=\{\pm\varepsilon_i\pm\varepsilon_j:1\le i<j\le3\},\qquad R\text{ has type }D_3.}
$$

Choose the simple roots

$$
\alpha_1=\varepsilon_1-\varepsilon_2,\qquad
\alpha_2=\varepsilon_2-\varepsilon_3,\qquad
\alpha_3=\varepsilon_2+\varepsilon_3.
$$

The six positive roots are $\alpha_1,\alpha_2,\alpha_3,\alpha_1+\alpha_2,\alpha_1+\alpha_3,\alpha_1+\alpha_2+\alpha_3$, and every other [root](../../../root-of-a-root-system.md) is their negative. In the standard orthonormal coordinates all roots have squared length $2$, and their [Cartan matrix](../../../cartan-matrix.md) is

$$
\begin{pmatrix}2&-1&-1\\-1&2&0\\-1&0&2\end{pmatrix}.
$$

Its [Dynkin diagram](../../../dynkin-diagram.md) is the connected chain $\alpha_2-\alpha_1-\alpha_3$. A decomposition into mutually orthogonal nonempty [root](../../../root-of-a-root-system.md) systems would separate this connected set of simple roots, which is impossible. Thus the [root system](../../../root-system.md) is irreducible. The chain is also the diagram $A_3$, which is the [root system](../../../root-system.md) of $\mathfrak{sl}_4(\mathbb C)$. The classification of complex semisimple Lie algebras by their [root](../../../root-of-a-root-system.md) systems yields the [Lie algebra isomorphism](../../../lie-algebra-isomorphism.md)

$$
\boxed{\mathfrak{so}_6(\mathbb C)\cong\mathfrak{sl}_4(\mathbb C).}
$$

An explicit explanation of this coincidence uses the [exterior-power Lie algebra representation](../../../exterior-power-lie-algebra-representation.md) of $\mathfrak{sl}_4$ on $\bigwedge^2\mathbb C^4$, a six-dimensional space. After choosing a volume form, $u\wedge v$ defines a nondegenerate [symmetric bilinear form](../../../symmetric-bilinear-form.md) on that [exterior square](../../../exterior-square.md). The induced action preserves it because a traceless [endomorphism](../../../endomorphism.md) acts trivially on the top exterior power. This gives a nonzero homomorphism $\mathfrak{sl}_4\to\mathfrak{so}_6$. Its [kernel](../../../kernel-of-a-linear-map-split.md) is an ideal in the simple algebra $\mathfrak{sl}_4$, so it is zero; equal dimensions $15$ then make it an isomorphism. Over $\mathbb C$ all nondegenerate symmetric forms in [dimension](../../../dimension-vector-space.md) six are equivalent, including the form with [matrix](../../../matrix.md) $J$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2011](../../2011-split.md)
3. [Past exam of the Lie algebras course of the University of Oxford](../../split.md)
4. [Lie algebras course of the University of Oxford](../../../lie-algebras-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
