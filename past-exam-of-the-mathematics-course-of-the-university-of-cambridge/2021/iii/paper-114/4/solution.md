<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an oriented real rank-$r$ vector bundle $\pi:E\to X$, let $u_E\in H^r(D(E),S(E);\mathbb Z)$ be its [Thom class](../../../../../thom-class.md). If $s:X\to D(E)$ is the zero section, the [Euler class of a vector bundle](../../../../../euler-class-of-a-vector-bundle.md) is

$$
e(E)=s^*u_E\in H^r(X;\mathbb Z).
$$

Let $u$ generate $H^{2k}(S^{2k};\mathbb Z)$. The [Poincaré-Hopf theorem](../../../../../poincare-hopf-theorem.md) gives

$$
e(TS^{2k})=\chi(S^{2k})u=2u.
$$

For every integer $m$, choose a map $f_m:S^{2k}\to S^{2k}$ of degree $m$. Naturality of the [Euler class](../../../../../euler-class-of-a-vector-bundle.md) gives

$$
e(f_m^*TS^{2k})=f_m^*e(TS^{2k})=2m,u.
$$

Thus every even class belongs to $\mathcal E_{2k}(S^{2k})$.

More generally, every class $a\in H^{2k}(M;\mathbb Z)$ on a closed $2k$-manifold is $f^*u$ for some map $f:M\to S^{2k}$, by the [realization of top-dimensional cohomology by a sphere map](../../../../../realization-of-top-dimensional-cohomology-by-a-sphere-map.md). Pulling back $TS^{2k}$ gives

$$
2a=e(f^*TS^{2k}),
$$

so $2H^{2k}(M;\mathbb Z)\subseteq\mathcal E_{2k}(M)$. The inclusion can be strict: every [complex line bundle](../../../../../complex-line-bundle.md) on $S^2$ has an underlying oriented real two-plane bundle, and these bundles realize every integral Euler class. Hence

$$
2H^2(S^2;\mathbb Z)\subsetneq\mathcal E_2(S^2)=H^2(S^2;\mathbb Z).
$$

The odd-dimensional analogue fails. The [Euler class of an oriented odd-rank vector bundle is two-torsion](../../../../../euler-class-of-an-oriented-odd-rank-vector-bundle-is-two-torsion.md), whereas $H^{2k+1}(S^{2k+1};\mathbb Z)\cong\mathbb Z$ is torsion-free. Thus every oriented rank-$(2k+1)$ bundle on $S^{2k+1}$ has zero Euler class, and the nonzero subgroup $2\mathbb Z$ cannot lie in $\mathcal E_{2k+1}(S^{2k+1})$.

Finally, if $E$ and $F$ are oriented bundles of ranks $k$ and $l$, orient $E\oplus F$ by the ordered sum. The [Whitney product formula for Euler classes](../../../../../whitney-product-formula-for-euler-classes.md) states

$$
e(E\oplus F)=e(E)\smile e(F).
$$

Therefore cup product restricts to the asserted map $\mathcal E_k(X)\otimes\mathcal E_l(X)\to\mathcal E_{k+l}(X)$.

It need not be injective. For $X=S^2$ and $k=l=2$, one has $\mathcal E_2(S^2)=\mathbb Z$, so the source contains $\mathbb Z\otimes\mathbb Z\cong\mathbb Z$, but $H^4(S^2)=0$ and the map is zero. It need not be surjective either. For $X=S^2$ and $k=l=1$, every oriented real line bundle is trivial, so both degree-one Euler-class sets vanish, while $\mathcal E_2(S^2)=\mathbb Z$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
