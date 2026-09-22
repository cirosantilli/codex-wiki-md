<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the convention $A_{ij}=\langle\alpha_j,\alpha_i^\vee\rangle=2(\alpha_i,\alpha_j)/(\alpha_i,\alpha_i)$. For a finite reduced crystallographic [root system](../../../../root-system.md), diagonal entries are two and off-diagonal entries belong to $\{0,-1,-2,-3\}$, with $A_{ij}A_{ji}\in\{0,1,2,3\}$. Transposing this convention merely transposes the [Cartan matrix](../../../../cartan-matrix.md).

The $\alpha$-string through $\beta$ has the consecutive [roots](../../../../root-of-a-root-system.md) $\beta-p\alpha,\ldots,\beta+q\alpha$, where $p,q\ge0$ and $p-q=\langle\beta,\alpha^\vee\rangle$. For distinct [simple roots](../../../../simple-root.md) $\alpha_i,\alpha_j$, the negative step is absent, so $p=0$ and $q=-A_{ij}$.

The [matrix](../../../../matrix.md) determines each simple [reflection](../../../../reflection-mathematics.md) on the simple-[root](../../../../root-of-a-root-system.md) [basis](../../../../basis.md):

$$
s_i(\alpha_j)=\alpha_j-A_{ij}\alpha_i.
$$

It therefore determines their generated [Weyl group](../../../../weyl-group.md) as linear transformations. Every [root](../../../../root-of-a-root-system.md) is in the Weyl orbit of a [simple root](../../../../simple-root.md). For a positive nonsimple [root](../../../../root-of-a-root-system.md) $\beta=\sum c_i\alpha_i$, some $(\beta,\alpha_i)$ is positive because $\sum c_i(\beta,\alpha_i)=(\beta,\beta)>0$. Its [reflection](../../../../reflection-mathematics.md) subtracts a positive integer multiple of $\alpha_i$ and lowers height. It stays positive unless the [root](../../../../root-of-a-root-system.md) is simple, since the other simple-[root](../../../../root-of-a-root-system.md) coefficients are unchanged and at least one is positive. Induction on height reaches a [simple root](../../../../simple-root.md); negative [roots](../../../../root-of-a-root-system.md) follow by sign. Hence $\Phi=W\Delta$, which is completely reconstructed by those [reflection](../../../../reflection-mathematics.md) [matrices](../../../../matrix.md). This determines the system up to [root](../../../../root-of-a-root-system.md)-system isomorphism, rather than fixing an absolute length scale; irreducible components may be rescaled.

For [positive roots for a chain Cartan matrix](../../../../positive-roots-for-a-chain-cartan-matrix.md), symmetry and adjacency imply all [simple roots](../../../../simple-root.md) have equal length; normalize their squared lengths to two. Adjacent inner products are minus one and all others zero. Since every [root](../../../../root-of-a-root-system.md) is Weyl-conjugate to a [simple root](../../../../simple-root.md), every [root](../../../../root-of-a-root-system.md) also has squared length two. Write a [positive root](../../../../positive-root.md) as $\beta=\sum_{i=1}^lc_i\omega_i$ with nonnegative integers $c_i$, and set $c_0=c_{l+1}=0$. Then

$$
2=(\beta,\beta)=2\sum_{i=1}^lc_i^2-2\sum_{i=1}^{l-1}c_ic_{i+1}=\sum_{i=0}^l(c_{i+1}-c_i)^2.
$$

There must be exactly two nonzero integer differences, one $+1$ and one $-1$. Nonnegativity and the two zero endpoint values imply that the coefficients are one on one consecutive interval and zero elsewhere.

Conversely a single [simple root](../../../../simple-root.md) is a [root](../../../../root-of-a-root-system.md). If $\omega_i+\cdots+\omega_j$ is a [root](../../../../root-of-a-root-system.md) and $j<l$, its pairing with $\omega_{j+1}^\vee$ is minus one. Reflecting in $\omega_{j+1}$ therefore adds that [simple root](../../../../simple-root.md), making the next longer interval a [root](../../../../root-of-a-root-system.md). Induction constructs every interval. Thus

$$
\boxed{\Phi^+=\left\{\sum_{k=i}^j\omega_k:1\le i\le j\le l\right\}.}
$$

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
