<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [group action](../../../../../group-action.md) of $G$ on $X$, the [orbit of a group action](../../../../../orbit-of-a-group-action.md) through $x$ is $Gx=\{gx:g\in G\}$, and its [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is $H_x=\{g:gx=x\}$. A [transitive group action](../../../../../transitive-group-action.md) has one orbit. A [simply transitive group action](../../../../../simply-transitive-group-action.md) has exactly one element carrying any given point to any other; equivalently it is transitive and every [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is trivial.

In the modern terminology, a [multiply transitive group action](../../../../../multiply-transitive-group-action.md) is transitive on ordered $k$-tuples of distinct points for some $k\ge2$. In older geometric usage, the phrase can instead mean transitive but not simply transitive, so that there are several elements carrying one point to another. Under either interpretation the action is transitive, and that alone is what the following argument needs. These meanings should not be confused: a transitive action with nontrivial stabilizers need not be two-transitive.

Fix $x_0\in X$ and put $H=H_{x_0}$. Define

$$
F:G/H\longrightarrow X,\qquad F(gH)=gx_0.
$$

This is well-defined because every element of $H$ fixes $x_0$. It is surjective by transitivity, and $gx_0=g'x_0$ is equivalent to $g'^{-1}g\in H$, proving injectivity. For a smooth [Lie group](../../../../../lie-group.md) action, $H$ is closed, since it is the inverse image of $x_0$ under the [orbit map](../../../../../orbit-map.md). The orbit map has constant rank: translations in $G$ and the action diffeomorphisms of $X$ intertwine its differentials. Transitivity makes this rank $\dim X$; otherwise every point would be a critical value, contradicting [Sard theorem](../../../../../sard-s-theorem.md). Its local submersion charts give smooth local sections and hence a smooth inverse for $F$. Therefore

$$
\boxed{X\cong G/H.}
$$

Choosing $x_1=ax_0$ replaces $H$ by $aHa^{-1}$. Thus the [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is determined by the base point, and intrinsically only up to conjugacy. A [simply transitive group action](../../../../../simply-transitive-group-action.md) gives $H=\{e\}$.

For a finite quantum system with [Hilbert space](../../../../../hilbert-space-split.md) $\mathcal H=\mathbb C^{n+1}$, a [pure state](../../../../../pure-state.md) is a nonzero vector modulo multiplication by a nonzero complex number. Equivalently, it is a unit vector modulo its physically irrelevant phase. Consequently the space of [pure states](../../../../../pure-state.md) is the space of complex lines,

$$
\boxed{\mathbb{CP}^{n}=(\mathbb C^{n+1}\setminus\{0\})/\mathbb C^*.}
$$

The qualification “pure” is essential: arbitrary [quantum states](../../../../../quantum-state.md) include mixed [density matrices](../../../../../density-matrix.md) and do not form [Complex projective space](../../../../../complex-projective-space.md).

The [unitary group](../../../../../unitary-group.md) $U(n+1)$ acts transitively on these lines: choose unit vectors in two given lines, complete each to an [orthonormal basis](../../../../../orthonormal-basis.md), and map one basis to the other by a [unitary transformation](../../../../../unitary-operator.md). The stabilizer of the line $\mathbb C e_0$ consists exactly of block matrices $\operatorname{diag}(z,V)$ with $z\in U(1)$ and $V\in U(n)$. Indeed a [unitary transformation](../../../../../unitary-operator.md) preserving the line also preserves its orthogonal complement. The [homogeneous space](../../../../../homogeneous-space.md) description is therefore

$$
\boxed{\mathbb{CP}^n\cong U(n+1)/(U(1)\times U(n)).}
$$

Its real dimension is $(n+1)^2-1-n^2=2n$. This action is generally not two-transitive: the absolute inner product between unit representatives of two lines is invariant.

The [Hopf fibration](../../../../../hopf-fibration.md) is the projection $\pi:S^{2n+1}\to\mathbb{CP}^n$, $z\mapsto[z]$. The right action $z\cdot\lambda=z\lambda$, $\lambda\in S^1$, is free, and its orbits are exactly the fibres. On the chart $U_i$ where $z_i\ne0$, write $w_j=z_j/z_i$ for $j\ne i$. A smooth local section is

$$
\sigma_i(w)=\frac{(w_0,\ldots,w_{i-1},1,w_{i+1},\ldots,w_n)}{\sqrt{1+\sum_{j\ne i}|w_j|^2}}.
$$

Every unit vector over this chart has the unique expression $z=\sigma_i([z])\lambda$, where $\lambda=z_i/|z_i|$. These formulas provide local trivializations $\pi^{-1}(U_i)\cong U_i\times S^1$, proving that this is a [principal bundle](../../../../../principal-bundle.md) with fibre $S^1$. For $n\ge1$ it has no global section: a global section would give $S^{2n+1}\cong\mathbb{CP}^n\times S^1$, contradicting their [fundamental groups](../../../../../fundamental-group.md). For $n=0$ the base is a point and the bundle is trivial.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
