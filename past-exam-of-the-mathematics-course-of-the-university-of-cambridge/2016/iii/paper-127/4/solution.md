<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [quaternionic projective space](../../../../../quaternionic-projective-space.md) $\mathbb{HP}^n$ is the space of one-dimensional right [quaternion](../../../../../quaternion.md) subspaces of $\mathbb H^{n+1}$. Equivalently it is the quotient of the unit sphere $S^{4n+3}$ by simultaneous right multiplication by unit quaternions. Its coordinate filtration has one open cell $\mathbb H^k\cong\mathbb R^{4k}$ in each dimension $4k$, for $0\le k\le n$. Hence its [cellular cohomology](../../../../../cellular-cohomology.md) is $\mathbb Z$ in those dimensions and zero otherwise.

Let $\mathcal H$ be the [quaternionic tautological line bundle](../../../../../quaternionic-tautological-line-bundle.md). Its unit [sphere bundle](../../../../../sphere-bundle.md) is $S^{4n+3}\to\mathbb{HP}^n$, with fibre $S^3$. The [Gysin sequence of a sphere bundle](../../../../../gysin-sequence-of-a-sphere-bundle.md) shows that multiplication by its [Euler class](../../../../../euler-class-of-a-vector-bundle.md) $e\in H^4$ is an isomorphism from $H^{4k}$ to $H^{4k+4}$ for $k<n$. Choose the generator $u=-e$. Its powers generate every nonzero positive degree, giving the [cohomology ring of quaternionic projective space](../../../../../cohomology-ring-of-quaternionic-projective-space.md)

$$
\boxed{H^*(\mathbb{HP}^n;\mathbb Z)=\mathbb Z[u]/(u^{n+1}),\qquad |u|=4}.
$$

This also accounts for $n=0$.

First take $n=2$. Under the coordinate inclusion $i:\mathbb{CP}^2\to\mathbb{HP}^2$, the pulled-back quaternionic line is the quaternionic extension of the complex tautological line $L$. As a complex rank-two bundle it is $L\oplus\overline L$: a transition scalar $c\in\mathbb C$ acts on the two complex coordinates of a quaternion by $c$ and $\overline c$. Put $x=c_1(L^*)$, the degree-two generator of the [cohomology ring of complex projective space](../../../../../cohomology-ring-of-complex-projective-space.md). The [Whitney sum formula for Chern classes](../../../../../whitney-sum-formula-for-chern-classes.md) gives

$$
i^*e=c_2(L\oplus\overline L)=(-x)x=-x^2,
\qquad \boxed{i^*u=x^2}.
$$

Here the [Euler class of a complex vector bundle](../../../../../euler-class-of-a-complex-vector-bundle.md) is its top [Chern class](../../../../../chern-class.md), using the complex orientation. In particular this degree-four pullback has coefficient one; it is not a multiple of larger absolute value. The compatible tautological bundles on the projective filtrations give the same equality for every $n$, and multiplicativity then determines the whole ring map:

$$
\boxed{i^*(u^k)=x^{2k},\qquad x^{n+1}=0}.
$$

It is zero whenever $2k>n$. These facts are the [complex inclusion into quaternionic projective space](../../../../../complex-inclusion-into-quaternionic-projective-space.md).

For an odd prime $p$, the [Steenrod reduced powers](../../../../../steenrod-reduced-power.md) are natural [stable cohomology operations](../../../../../stable-cohomology-operation.md)

$$
P^i:H^q(-;\mathbb F_p)\longrightarrow H^{q+2i(p-1)}(-;\mathbb F_p).
$$

They satisfy $P^0=1$, the [Cartan formula](../../../../../cartan-formula-algebraic-topology.md), $P^i a=0$ when $2i>|a|$, and $P^i a=a^p$ when $|a|=2i$. In particular, on $\mathbb{CP}^\infty$ one has $P^1x=x^p$ and $P^i x=0$ for $i>1$. The [Cartan formula](../../../../../cartan-formula-algebraic-topology.md) and the [binomial theorem](../../../../../binomial-theorem.md) give

$$
P^i(x^{2k})=\binom{2k}{i}x^{2k+i(p-1)}.
$$

Pass to the infinite projective spaces, where $i^*:H^*(\mathbb{HP}^\infty;\mathbb F_p)\to H^*(\mathbb{CP}^\infty;\mathbb F_p)$, $u\mapsto x^2$, is injective. The equality just obtained determines the [Steenrod powers on quaternionic projective space](../../../../../steenrod-powers-on-quaternionic-projective-space.md); restricting to the finite spaces gives

$$
\boxed{P^i(u^k)=\binom{2k}{i}u^{k+i(p-1)/2}}
$$

with coefficients modulo $p$ and powers above $n$ set to zero. In particular $P^1u=2u^{(p+1)/2}$, $P^2u=u^p$, and $P^i u=0$ for $i>2$. The infinite-space argument matters: the finite inclusion cannot detect those degrees for which $x^{2k}=0$.

Finally put $Q=\mathbb{HP}^{15}/\mathbb{HP}^{12}$ and $S=\Sigma^{48}\mathbb{HP}^3$. Both have [reduced cohomology](../../../../../reduced-cohomology.md) $\mathbb Z$ in degrees $52,56,60$ and zero otherwise. Choose integral generators $a_{13},a_{14},a_{15}$ for $Q$ whose pullbacks under the quotient map are $u^{13},u^{14},u^{15}$, and suspended integral generators $b_1,b_2,b_3$ for $S$ from $u,u^2,u^3$.

Use $p=5$. Naturality for the quotient and the formula above give

$$
P^1a_{13}=\binom{26}{1}a_{15}=a_{15}\quad\text{modulo }5.
$$

Stability under the [suspension isomorphism](../../../../../suspension-isomorphism.md) instead gives

$$
P^1b_1=\Sigma^{48}(P^1u)=2b_3\quad\text{modulo }5.
$$

Any [homotopy equivalence](../../../../../homotopy-equivalence.md) $h:Q\to S$ would induce isomorphisms on the rank-one integral groups, so $h^*b_1=\varepsilon a_{13}$ and $h^*b_3=\delta a_{15}$ with $\varepsilon,\delta\in\{1,-1\}$. Reducing modulo five and commuting $h^*$ with $P^1$ would require $\varepsilon=2\delta$ in $\mathbb F_5$. Neither $1$ nor $-1$ equals $2$ or $-2$ modulo five. Therefore

$$
\boxed{\mathbb{HP}^{15}/\mathbb{HP}^{12}\not\simeq\Sigma^{48}\mathbb{HP}^3}.
$$

The essential point is that [integral generator signs constrain Steenrod comparisons](../../../../../integral-generator-signs-constrain-steenrod-comparisons.md). Arbitrary changes of basis over $\mathbb F_5$ could rescale these two nonzero coefficients into agreement; a genuine equivalence must also preserve the integral lattices, where only the two signs are available.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 127](../../paper-127-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
