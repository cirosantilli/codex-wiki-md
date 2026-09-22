<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [flat torus](../../../../../flat-torus.md) is the quotient $\mathbb R^d/\Lambda$, where $\Lambda$ is a full-rank [Euclidean lattice](../../../../../euclidean-lattice.md), with the [Riemannian metric](../../../../../riemannian-metric.md) induced from the [Euclidean metric](../../../../../euclidean-metric.md). Translation by a lattice vector is a [Riemannian isometry](../../../../../riemannian-isometry.md), so this metric is well defined and has zero curvature. Its volume is the covolume of $\Lambda$.

The [dual lattice](../../../../../dual-lattice.md) is $\Lambda^\vee=\{w:\langle w,v\rangle\in\mathbb Z\text{ for all }v\in\Lambda\}$. For $w\in\Lambda^\vee$, the function $e_w(x)=\exp(2\pi i\langle w,x\rangle)$ descends to the [flat torus](../../../../../flat-torus.md), and direct differentiation gives

$$
\Delta e_w=4\pi^2|w|^2e_w.
$$

Conversely, write $\Lambda=B\mathbb Z^d$ and $x=By$. Ordinary [Fourier series](../../../../../fourier-series-split.md) on $\mathbb R^d/\mathbb Z^d$ have frequencies $n\in\mathbb Z^d$, corresponding to $w=B^{-\mathsf T}n\in\Lambda^\vee$. After normalization they form a complete [orthonormal basis](../../../../../orthonormal-basis.md) in $L^2$, and the [Fourier coefficients](../../../../../fourier-coefficient.md) of a smooth function decay rapidly. Applying the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) term by term shows that a smooth [eigenfunction](../../../../../eigenfunction.md) with [eigenvalue](../../../../../eigenvalue.md) $\lambda$ has nonzero coefficients only where $4\pi^2|w|^2=\lambda$. Thus the [spectrum of a flat torus](../../../../../spectrum-of-a-flat-torus.md) is

$$
\boxed{\operatorname{Spec}(\mathbb R^d/\Lambda)=\{4\pi^2|w|^2:w\in\Lambda^\vee\},\qquad
m(\lambda)=\#\{w\in\Lambda^\vee:4\pi^2|w|^2=\lambda\}.}
$$

The formula counts multiplicity over either the real or complex numbers: the two frequencies $w,-w$ give the real sine and cosine functions.

For the rigidity assertion in dimension two, it suffices to reconstruct a rank-two [Euclidean lattice](../../../../../euclidean-lattice.md) $L=\Lambda^\vee$ from its vector-length multiset. The multiset first determines its covolume $A$. Indeed, a bounded fundamental parallelogram, and comparison of the cells meeting a disk with slightly larger and smaller disks, give the [lattice-point asymptotics by fundamental cells](../../../../../lattice-point-asymptotics-by-fundamental-cells.md)

$$
N_L(R)=\#\{v\in L:|v|\leq R\}=\frac{\pi R^2}{A}+O(R).
$$

The [spectrum](../../../../../spectrum-functional-analysis.md) determines $N_L(R)$, including multiplicities, so it determines $A$.

Let $a$ be the smallest nonzero vector length, and choose $v\in L$ with $|v|=a$. This vector is primitive: $v=ku$ with $|k|>1$ would contradict minimality. From the length multiset subtract the two vectors $kv,-kv$ at every positive length $ka$, for $k=1,2,\ldots$. The shortest remaining length $b$ is exactly the length of a shortest vector $w\notin\mathbb Zv$. This subtraction is legitimate even if several directions have length $a$: it subtracts just two copies, and then $b=a$. It also proves that $b$ is independent of our choice of shortest direction. Replace $w$ by $w-kv$ to arrange

$$
|v\cdot w|\leq a^2/2.
$$

The replacement stays outside $\mathbb Zv$ and cannot be shorter than $b$, so a reduced choice still has length $b$.

The [shortest-independent-vector basis lemma](../../../../../shortest-independent-vector-basis-lemma.md) says that $v,w$ are a basis of $L$. To prove it, choose coordinates with $v=(a,0)$. Because $v$ is primitive, $L/\mathbb Zv\cong\mathbb Z$; let $h>0$ be the smallest positive vertical coordinate in $L$. Write $w=(x,mh)$, with $m\geq1$ after changing its sign. If $m\geq2$, a vector $u$ of vertical coordinate $h$, reduced horizontally modulo $v$, has

$$
|u|^2\leq a^2/4+h^2\leq(a^2+m^2h^2)/4\leq(a^2+b^2)/4\leq b^2/2<b^2.
$$

This contradicts the definition of $b$, since $u\notin\mathbb Zv$. Hence $m=1$ and $v,w$ generate $L$.

The [Gram matrix](../../../../../gram-matrix.md) of this basis is $\left(\begin{smallmatrix}a^2&c\\c&b^2\end{smallmatrix}\right)$, with $c=v\cdot w$, and its determinant is $A^2$. Therefore

$$
c^2=a^2b^2-A^2.
$$

Changing the sign of one basis vector allows $c\geq0$. The numbers $a,b,A$, all audible from the [spectrum](../../../../../spectrum-functional-analysis.md), consequently determine the [Gram matrix](../../../../../gram-matrix.md), and hence $L$, up to an [orthogonal transformation](../../../../../orthogonal-transformation.md). Taking [dual lattices](../../../../../dual-lattice.md) gives the same conclusion for $\Lambda$. **Isospectral flat two-dimensional tori are isometric.** The argument uses the special basis property of rank-two [Euclidean lattices](../../../../../euclidean-lattice.md), so it does not claim higher-dimensional rigidity.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 117](../../paper-117-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
