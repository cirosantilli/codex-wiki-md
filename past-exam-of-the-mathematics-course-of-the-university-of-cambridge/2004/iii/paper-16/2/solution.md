<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [CW complex](../../../../../cw-complex.md) is built by attaching q-dimensional discs to the $(q-1)$-skeleton along maps of their boundary [spheres](../../../../../sphere.md), with the closure-finite and weak-topology conditions. Write $X^q$ for its q-skeleton and $X^{-1}=\varnothing$. The [cellular chain group](../../../../../cellular-chain-group.md) is

$$
C_q^{\mathrm{cell}}(X)=H_q(X^q,X^{q-1})\cong\bigoplus_{\text{q-cells}}\mathbb Z.
$$

The [cellular boundary](../../../../../cellular-boundary.md) is the composite of the connecting map and the relative quotient map:

$$
H_q(X^q,X^{q-1})\xrightarrow{\delta}H_{q-1}(X^{q-1})\longrightarrow H_{q-1}(X^{q-1},X^{q-2}).
$$

Consecutive maps in the relevant exact sequences compose to zero, so these maps make a [cellular chain complex](../../../../../cellular-chain-complex.md). Equivalently, a boundary coefficient is the degree of the attaching [sphere](../../../../../sphere.md) followed by collapse onto the [sphere](../../../../../sphere.md) of a selected lower cell. Its [cellular homology](../../../../../cellular-chain-complex.md) is $\ker d_q/\operatorname{im}d_{q+1}$. The relative groups of successive skeleta vanish off their cell dimension; their exact sequences identify this [homology](../../../../../homology-split.md) with [singular homology](../../../../../singular-homology.md), the [cellular homology theorem](../../../../../cellular-homology-theorem.md).

For $k\ge1$, the [sphere](../../../../../sphere.md) $S^k$ has a zero-cell and a k-cell with zero boundary. The [Complex projective space](../../../../../complex-projective-space.md) $\mathbb{CP}^n$ has one cell in each dimension $0,2,\ldots,2n$ and no odd cells, so all cellular boundaries vanish. Consequently

$$
\boxed{H_q(S^k)=\begin{cases}\mathbb Z,&q=0,k,\\0,&\text{otherwise},\end{cases}\qquad
H_q(\mathbb{CP}^n)=\begin{cases}\mathbb Z,&q\in\{0,2,\ldots,2n\},\\0,&\text{otherwise}.\end{cases}}
$$

At $k=0$, the [sphere](../../../../../sphere.md) consists of two points and $H_0(S^0)=\mathbb Z^2$; at $n=0$, projective space is a point.

Put $a=2n-2$ and $Z=S^a\times S^3$. Its product [CW complex](../../../../../cw-complex.md) has cells in dimensions $0,3,a,a+3=2n+1$. For $n>3$, these positive dimensions are distinct and never consecutive, so all [cellular boundaries](../../../../../cellular-boundary.md) vanish. Thus

$$
\boxed{H_q(Z)=\begin{cases}\mathbb Z,&q\in\{0,3,2n-2,2n+1\},\\0,&\text{otherwise}.\end{cases}}
$$

Its $2n$-skeleton is $S^a\vee S^3$. Collapsing it gives the quotient

$$
q:Z\longrightarrow S^a\wedge S^3\cong S^{2n+1}.
$$

It induces an isomorphism on top [homology](../../../../../homology-split.md), with degree $+1$ after choosing the quotient [orientation](../../../../../orientation-of-a-simplex.md). Let $p:S^{2n+1}\to\mathbb{CP}^n$ be the [Hopf fibration](../../../../../hopf-fibration.md) and set $\phi=pq$, the [Hopf projection of a product smash quotient](../../../../../hopf-projection-of-a-product-smash-quotient.md).

On [reduced homology](../../../../../reduced-homology.md), the collapse kills the two lower-dimensional classes, and the remaining top class maps to zero because projective space has no odd-dimensional [homology](../../../../../homology-split.md). Therefore $\phi_*=0$ in every reduced degree. On [homotopy groups](../../../../../homotopy-group.md), $\pi_j(Z)\cong\pi_j(S^a)\oplus\pi_j(S^3)$ for $j\ge2$, with summands induced by the two factor inclusions. Both inclusions are collapsed by $q$, so $q_*$ and hence $\phi_*$ vanish on both summands. The domain is [simply connected](../../../../../simply-connected-space.md) and connected, which also handles the lower groups.

It remains to prove that $\phi$ is not [null-homotopic](../../../../../null-homotopic-map.md). The [Hopf fibration](../../../../../hopf-fibration.md) has fibre $S^1$ and has the [homotopy lifting property](../../../../../homotopy-lifting-property.md) for the CW domain $Z$: a [homotopy](../../../../../homotopy.md) downstairs and a lift of its initial map have a lift with that specified initial value. If $\phi$ were homotopic to a constant, lift this [homotopy](../../../../../homotopy.md) starting at $q$. The ending map would land in the single fibre $S^1$. Every map $Z\to S^1$ is [null-homotopic](../../../../../null-homotopic-map.md), since the [simply connected](../../../../../simply-connected-space.md) domain permits its lift to the contractible [universal cover](../../../../../universal-cover.md) $\mathbb R\to S^1$. Thus $q$ would be [null-homotopic](../../../../../null-homotopic-map.md) in $S^{2n+1}$, contradicting its nonzero top [homology](../../../../../homology-split.md) map. Hence

$$
\boxed{\phi_*\text{ vanishes on all homotopy groups and reduced homology, but }\phi\not\simeq *.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
