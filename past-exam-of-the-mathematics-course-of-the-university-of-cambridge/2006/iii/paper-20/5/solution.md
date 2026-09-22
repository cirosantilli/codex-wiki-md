<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [symplectic capacity](../../../../../symplectic-capacity.md) assigns $c(X,\omega)\in[0,\infty]$ to [symplectic manifolds](../../../../../symplectic-manifold.md) in a fixed dimension, is monotone under [symplectic embeddings](../../../../../symplectic-embedding.md), satisfies $c(X,a\omega)=a\,c(X,\omega)$ for $a>0$, and is nontrivial in the sense that

$$
0<c(B^{2n}(1))\leq c(B^2(1)\times\mathbb R^{2n-2})<\infty.
$$

The second domain is the standard [symplectic cylinder](../../../../../symplectic-cylinder.md). A [normalized symplectic capacity](../../../../../normalized-symplectic-capacity.md) assigns $\pi$ to both unit domains, hence $\pi R^2$ to both radius-$R$ domains. The general axioms already give invariance under [symplectomorphisms](../../../../../symplectomorphism.md) and quadratic scaling under coordinate dilation. For the rigidity argument, use the assumed existence of capacities in each dimension, including after adding a symplectic plane; normalization is not needed.

Let $\phi_j$ be [symplectomorphisms](../../../../../symplectomorphism.md) converging locally uniformly to a smooth [diffeomorphism](../../../../../diffeomorphism.md) $\phi$. Work in [Darboux charts](../../../../../darboux-chart.md). For a sufficiently small [solid ellipsoid](../../../../../solid-ellipsoid.md) $E$ centered at a chosen point and $0<a<1$, uniform convergence and [degree of a continuous mapping](../../../../../degree-of-a-continuous-mapping.md) give, for large $j$,

$$
\phi_j(aE)\subseteq\phi(E)\subseteq\phi_j(a^{-1}E).
$$

For the second inclusion, $\phi^{-1}\phi_j$ is uniformly close to the identity on the larger ellipsoid. Its boundary stays outside $\overline E$ and is homotopic there to the identity, so it has degree one about every point of $E$ and must cover $E$. Monotonicity and scaling now give $a^2c(E)\leq c(\phi(E))\leq a^{-2}c(E)$. Letting $a$ tend to one proves [capacity preservation under uniform limits](../../../../../capacity-preservation-under-uniform-limits.md).

At the chosen point, write $T=D\phi$. The rescaled maps $(\phi(tz)-\phi(0))/t$ preserve capacities of ellipsoids and converge uniformly on compact sets to $T$. Applying the same sandwich argument proves that $T$ preserves the capacities of all [solid ellipsoids](../../../../../solid-ellipsoid.md); so does $T^{-1}$.

We prove the required [linear capacity rigidity](../../../../../linear-capacity-rigidity.md) explicitly. Write the standard [symplectic form](../../../../../symplectic-form.md) as $\Omega$. Suppose $\Omega(u,v)=1$ and

$$
0<|\Omega(T^Tu,T^Tv)|=\lambda^2<1.
$$

Complete $u,v$ to a [symplectic basis](../../../../../symplectic-basis.md), and complete $T^Tu/\lambda$, with the appropriately signed $T^Tv/\lambda$, to another [symplectic basis](../../../../../symplectic-basis.md). If their basis matrices are $P,P'$, then $A=(P')^{-1}T^TP$ has first two columns $\lambda e_1,\pm\lambda f_1$. Hence $A^T$ sends the unit ball into the [symplectic cylinder](../../../../../symplectic-cylinder.md) of radius $\lambda$. This matrix differs from $T$ by symplectic linear maps, so it preserves capacities of ellipsoids. Its first coordinate pair is multiplied by $\lambda$, with a possible sign, and therefore $(A^T)^k$ sends the unit ball into the cylinder of radius $\lambda^k$. Monotonicity gives

$$
0<c(B^{2n}(1))\leq\lambda^{2k}c(Z^{2n}(1))
$$

for every $k$, contradicting finiteness of the right-hand unit-cylinder capacity as $k$ tends to infinity. For a normalized capacity, the first iterate already gives the contradiction.

A zero pairing is handled by a small perturbation of $u,v$. A pairing of absolute value greater than one gives the same contradiction for $T^{-1}$, after normalizing the transformed pair. Thus

$$
|\Omega(T^Tu,T^Tv)|=|\Omega(u,v)|
$$

for every pair. The squared bilinear forms agree, so their difference times their sum is the zero polynomial. The real polynomial ring is an [integral domain](../../../../../integral-domain.md); consequently one factor vanishes identically. Therefore $T$ is either symplectic or [anti-symplectic](../../../../../anti-symplectic-map.md).

To eliminate the negative sign, repeat the argument for $\phi_j\times\operatorname{id}_{\mathbb R^2}$, which are [symplectomorphisms](../../../../../symplectomorphism.md) for $\omega\oplus\omega_{\mathbb R^2}$. If $\phi^*\omega=-\omega$ at the chosen point, the limit pulls this product form back to $-\omega\oplus\omega_{\mathbb R^2}$, which is neither the product form nor its negative. This contradicts the preceding derivative classification. Thus $\phi^*\omega=\omega$ everywhere. We have proved the [Eliashberg–Gromov rigidity theorem](../../../../../eliashberg-gromov-rigidity-theorem.md): **the symplectomorphism group is closed in the $C^0$ topology on diffeomorphisms**.

Finally put $E=W^\perp$, with perpendicularity taken for the standard Euclidean [inner product](../../../../../inner-product.md). Its dimension is two, so being nonisotropic means that the restricted [symplectic form](../../../../../symplectic-form.md) is [nondegenerate](../../../../../nondegenerate-bilinear-form.md). For the standard compatible complex structure $J$, $W^\omega=JE$. If $Jv\in W\cap JE$, then $v\in E$ and $\omega(v,e)=0$ for every $e\in E$, forcing $v=0$. Thus $W$ is a [symplectic subspace](../../../../../symplectic-subspace.md) and admits a [symplectic basis](../../../../../symplectic-basis.md) extended to the whole space.

In the resulting linear symplectic coordinates, $W$ is $\{q_1=p_1=0\}$. The projection of the bounded set $U$ to the $(q_1,p_1)$ plane is bounded, so $U+W$ lies in a [symplectic cylinder](../../../../../symplectic-cylinder.md) of some finite radius $R$. As $U$ is nonempty and open, it contains a ball of some radius $r>0$, which is also contained in $U+W$. Monotonicity and scaling give

$$
\boxed{0<r^2c(B^{2n}(1))\leq c(U+W)\leq R^2c(Z^{2n}(1))<\infty},
$$

as in [capacity of a bounded set thickened by a symplectic subspace](../../../../../capacity-of-a-bounded-set-thickened-by-a-symplectic-subspace.md). For a [normalized symplectic capacity](../../../../../normalized-symplectic-capacity.md), the two bounds simplify to $\pi r^2$ and $\pi R^2$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
