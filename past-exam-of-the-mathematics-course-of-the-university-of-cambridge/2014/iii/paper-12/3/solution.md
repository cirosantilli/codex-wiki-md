<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [complex tautological line bundle](../../../../../complex-tautological-line-bundle.md) over [Complex projective space](../../../../../complex-projective-space.md) is

$$
\lambda=\{(\ell,v):\ell\in\mathbb{CP}^n,\ v\in\ell\}\longrightarrow\mathbb{CP}^n,\qquad(\ell,v)\longmapsto\ell.
$$

On the standard chart $U_i=\{[z_0:\cdots:z_n]:z_i\ne0\}$, the vector $v_i([z])=z/z_i$ is independent of the chosen representative and gives a continuous nonzero frame. The map

$$
U_i\times\mathbb C\longrightarrow\lambda|_{U_i},\qquad(\ell,w)\longmapsto(\ell,wv_i(\ell))
$$

is a [local trivialization](../../../../../local-trivialization.md); its inverse takes the $i$th coordinate of the vector in the fibre. Hence $\lambda$ is a locally trivial [complex line bundle](../../../../../complex-line-bundle.md).

Its unit [sphere bundle](../../../../../sphere-bundle.md) is $S^{2n+1}$: a unit vector $v\in\mathbb C^{n+1}$ corresponds to $([v],v)$. The projection is the [Hopf fibration](../../../../../hopf-fibration.md). Regard $\lambda$ as an oriented real rank-two [vector bundle](../../../../../vector-bundle.md) using its complex orientation, and put $t=e(\lambda)\in H^2(\mathbb{CP}^n;\mathbb Z)$. The [Gysin sequence of a sphere bundle](../../../../../gysin-sequence-of-a-sphere-bundle.md) gives, for $2\leq q\leq2n$,

$$
H^{q-2}(\mathbb{CP}^n;\mathbb Z)\overset{\smile t}{\longrightarrow}H^q(\mathbb{CP}^n;\mathbb Z)
$$

as an isomorphism, since the intervening cohomology groups of $S^{2n+1}$ vanish. It also gives $H^1(\mathbb{CP}^n)=0$. The [CW complex](../../../../../cw-complex.md) structure has one cell in dimensions $0,2,\ldots,2n$ and none above $2n$, so these groups and products give

$$
\boxed{H^*(\mathbb{CP}^n;\mathbb Z)\cong\mathbb Z[t]/(t^{n+1}),\qquad |t|=2.}
$$

The [Euler class](../../../../../euler-class-of-a-vector-bundle.md) of $\lambda$ is the negative of the usual hyperplane generator; replacing $t$ by $-t$ gives the same ring presentation. For $n=0$ the formula reads $\mathbb Z$.

Now let $\alpha$ generate $H^2(S^2;\mathbb Z)$ and let $u_i$ be its pullback from the $i$th factor of $(S^2)^n$. The [Künneth theorem](../../../../../kunneth-theorem.md) gives $H^2((S^2)^n;\mathbb Z)=\bigoplus_i\mathbb Z u_i$. If a map $f$ were invariant under all factor permutations, write $f^*\alpha=\sum_i a_i u_i$; naturality under a transposition forces every $a_i$ to have the same integer value $a$. Let $\Delta:S^2\to(S^2)^n$ be the diagonal. Then

$$
\Delta^*f^*\alpha=na\alpha.
$$

The second condition is $f\circ\Delta=\mathrm{id}$, so this must equal $\alpha$, giving $na=1$. **For $n>1$ this is impossible in $\mathbb Z$, and $\boxed{\text{no such continuous map exists}.}$** This is the [diagonal-degree obstruction to a symmetric sphere retraction](../../../../../diagonal-degree-obstruction-to-a-symmetric-sphere-retraction.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
