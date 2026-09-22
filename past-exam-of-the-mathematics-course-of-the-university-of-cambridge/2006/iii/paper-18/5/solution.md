<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Torelli theorem](../../../../../torelli-theorem.md) concerns a connected [smooth projective curve](../../../../../smooth-projective-curve.md) over $\mathbb C$ and its canonical principal [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md). Its conclusion is

$$
\boxed{(\operatorname{Jac}(X),[\Theta_X])\cong(\operatorname{Jac}(Y),[\Theta_Y])\quad\Longrightarrow\quad X\cong Y.}
$$

The [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md) is part of the hypothesis. We will reconstruct the curve intrinsically from the [Jacobian variety](../../../../../jacobian-variety.md) and the [theta divisor](../../../../../theta-divisor.md), using the [Gauss map of a theta divisor](../../../../../gauss-map-of-a-theta-divisor.md), and prove the reconstruction in both the nonhyperelliptic and [hyperelliptic curve](../../../../../hyperelliptic-curve.md) cases. The needed biduality and ordinary-tangency facts about [projective dual varieties](../../../../../projective-dual-variety.md) are the general projective-duality results permitted here.

First explain why the polarized data determine the [theta divisor](../../../../../theta-divisor.md) up to translation. On $J=\operatorname{Jac}(X)$, take integral one-form classes $\alpha_i,\beta_i$ dual to the symplectic cycle [basis](../../../../../basis.md). Pullback by the degree-one [Abelian sum map](../../../../../abel-map-of-an-algebraic-curve.md) identifies them with the corresponding classes on $X$; the [Riemann bilinear relations](../../../../../riemann-bilinear-relations-for-a-compact-surface.md) give

$$
\int_X\alpha_i\wedge\beta_j=\delta_{ij},\qquad
\int_X\alpha_i\wedge\alpha_j=\int_X\beta_i\wedge\beta_j=0.
$$

On $X^{g-1}$, the sum map pulls each one-form back to the sum of its pullbacks from the factors. It has generic degree $(g-1)!$ onto $W_{g-1}$: the [Abel theorem for divisors](../../../../../abel-theorem-for-divisors.md) and the existence of classes with $h^0=1$ give a unique effective unordered representative, and ordering gives the factorial. Integrating a wedge of $2g-2$ [basis](../../../../../basis.md) one-forms over the product, only terms assigning a matching pair $\alpha_i,\beta_i$ to each factor survive. Dividing by $(g-1)!$ gives integral one when precisely one matching pair is omitted, and zero for all other [basis](../../../../../basis.md) wedges. Hence the Poincaré dual class of $W_{g-1}$ is

$$
c_1(\mathcal O_J(\Theta))=\sum_{i=1}^g\alpha_i\wedge\beta_i.
$$

This is exactly the integral form of the canonical principal [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md) constructed by periods.

Its associated [line bundle](../../../../../line-bundle.md) has one-dimensional section space. One can check this without any theta multiplicity assumption: in normalized period coordinates a representative has sections satisfying

$$
F(z+m)=F(z),\qquad
F(z+\tau n)=e^{-\pi i n^t\tau n-2\pi i n^tz}F(z).
$$

Expand the first periodicity in a [Fourier series](../../../../../fourier-series-split.md) $F(z)=\sum_{k\in\mathbb Z^g}c_ke^{2\pi i k^tz}$. The second periodicity forces $c_k=c_0e^{\pi i k^t\tau k}$. Positive definiteness of $\operatorname{Im}\tau$ makes this series normally convergent, so the section space has dimension exactly one. Other [line bundles](../../../../../line-bundle.md) giving the same [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md) differ by a degree-zero [line bundle](../../../../../line-bundle.md). The map $x\mapsto T_x^*L\otimes L^{-1}$ is an isomorphism from $J$ to its [dual abelian variety](../../../../../dual-abelian-variety.md) for a principal [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md): on lattices it is the unimodular alternating form. Thus all these [line bundles](../../../../../line-bundle.md) are translates, and so are their unique zero [divisors](../../../../../divisor.md). In particular the given polarized data recover the reduced [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $W_{g-1}$ up to translation. Translation does not change tangent hyperplanes after identifying tangent spaces with $T_0J$.

Put $V=T_0J=H^0(K_X)^*$ and $P=\mathbb P(V^*)$. At a smooth class $L=\mathcal O_X(D)\in\Theta$, the [Riemann singularity theorem](../../../../../riemann-singularity-theorem.md) says $h^0(D)=1$. The [derivative of the Abelian sum map](../../../../../derivative-of-the-abelian-sum-map.md) identifies the translated tangent hyperplane with $H^0(K_X(-D))^\perp$. Thus the intrinsic [Gauss map of a theta divisor](../../../../../gauss-map-of-a-theta-divisor.md) is

$$
\Gamma:\Theta_{\mathrm{sm}}\longrightarrow P,
\qquad \Gamma(L)=[\omega],\quad H^0(K_X(-D))=\mathbb C\omega.
$$

In particular

$$
D\le\operatorname{div}(\omega).
$$

We will see that this map is dominant and generically finite. Its function-field extension therefore determines an intrinsic finite cover: normalize $P$ in $\mathbb C(\Theta)$, obtaining $Z\to P$. Normalization in a finite extension is finite here. Let $B\subset P$ be its reduced codimension-one branch locus. Using this finite cover avoids counting omitted points of the rational [Gauss map of a theta divisor](../../../../../gauss-map-of-a-theta-divisor.md) as ramification. Everything in this construction is determined by the polarized [Jacobian variety](../../../../../jacobian-variety.md).

Suppose first that $g\ge3$ and $X$ is nonhyperelliptic. Its [canonical map](../../../../../canonical-map.md) embeds it as a nondegenerate curve $C\subset\mathbb P(V)$. For clarity, this follows directly from the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md): $h^0(p)=1$ on a positive-genus curve, so $K_X$ has no base point. If a length-two effective [divisor](../../../../../divisor.md) $E$ had $h^0(E)\ge2$, a nonconstant [meromorphic function](../../../../../meromorphic-function.md) with poles bounded by $E$ would give a map of degree at most two to $\mathbb P^1$. Degree one forces genus zero, and degree two is the [hyperelliptic curve](../../../../../hyperelliptic-curve.md) case. Hence $h^0(E)=1$, and the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(K_X(-E))=g-2$. The canonical sections therefore separate every pair of points and every tangent direction, proving the embedding.

Let $U\subset P$ be the open set of hyperplanes transverse to $C$. A hyperplane in $U$ cuts out $n=2g-2$ distinct points. These points span the hyperplane: if a second independent canonical section vanished at all of them, its zero [divisor](../../../../../divisor.md) would have to equal the same degree-$2g-2$ [divisor](../../../../../divisor.md), and the ratio of the two sections would be a constant. Consequently some $g-1$ of the intersection points are independent. For the [divisor](../../../../../divisor.md) $D$ formed by such a subset, $h^0(K_X(-D))=1$ and $h^0(D)=1$.

We need to know that every $(g-1)$-subset of a general hyperplane section has this property. Here is the [monodromy](../../../../../monodromy.md) argument, with its essential steps. The incidence space choosing one intersection point is a [projective bundle](../../../../../projective-bundle.md) over $C$ before restricting to $U$, so it is irreducible. The incidence space choosing two distinct ordered intersection points is likewise a [projective bundle](../../../../../projective-bundle.md) over $C\times C$ minus its diagonal, with fibre $\mathbb P^{g-3}$; it too is irreducible. Restricting to transverse sections preserves irreducibility and hence connectedness of these covers. Thus the [monodromy action of a covering space](../../../../../monodromy-action-of-a-covering-space.md) on the $n$ intersection points is two-transitive. A general tangent hyperplane has just one contact of order two, by characteristic-zero [projective biduality theorem](../../../../../projective-biduality-theorem.md); locally its intersection equation is $z^2=t$ together with the other simple points. A small loop in $t$ exchanges exactly those two points. Two-transitivity conjugates this transposition to every transposition, so the [monodromy](../../../../../monodromy.md) is the full [symmetric group](../../../../../symmetric-group.md) $\mathfrak S_n$.

It follows that the finite étale cover of $U$ choosing a $(g-1)$-subset is connected and irreducible. The condition of dependent evaluations is closed on that cover. It is proper because we have exhibited an independent subset; its image under the finite map is therefore a proper closed subset of $U$. Outside that image every subset is independent. By the [Abel theorem for divisors](../../../../../abel-theorem-for-divisors.md), distinct such subsets have distinct Abelian sums: $h^0(D)=1$ means there is only one effective representative of its class. Thus the subset cover is birational to $\Theta$ with its [Gauss map of a theta divisor](../../../../../gauss-map-of-a-theta-divisor.md), and

$$
\deg\Gamma=\binom{2g-2}{g-1}.
$$

More precisely it is exactly the restriction of $Z\to P$ over $U$, since this étale cover is normal and has the same [function field](../../../../../function-field-of-an-algebraic-variety.md).

There can consequently be no branch component over $U$. Its complement is the irreducible hypersurface $C^*$ of tangent hyperplanes, the [projective dual variety](../../../../../projective-dual-variety.md) of $C$. Around a general point of $C^*$, the transposition of two roots acts nontrivially on $(g-1)$-subsets: choose a subset containing exactly one of those two roots. Hence the finite cover is ramified there. This proves the exact identity

$$
\boxed{B=C^*.}
$$

The quoted biduality theorem now recovers $C=(C^*)^*=B^*$ as an embedded curve, and the [canonical map](../../../../../canonical-map.md) identifies $X$ with $C$. This proves reconstruction in the nonhyperelliptic case, including special curves rather than only a general curve in moduli.

Now suppose that $X$ is a [hyperelliptic curve](../../../../../hyperelliptic-curve.md) of genus $g\ge3$. Let $\pi:X\to\mathbb P^1$ be its degree-two map. The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) gives $2g+2$ branch points $b_1,\ldots,b_{2g+2}$. Choose an affine coordinate with no branch at infinity and write

$$
y^2=\prod_{i=1}^{2g+2}(x-b_i).
$$

The forms $dx/y,x\,dx/y,\ldots,x^{g-1}dx/y$ are holomorphic and independent; their orders at the two points at infinity show there are exactly $g$ of them. Thus the [canonical map](../../../../../canonical-map.md) factors as $\pi$ followed by the degree-$g-1$ [rational normal curve](../../../../../rational-normal-curve.md) embedding

$$
\nu:\mathbb P^1\longrightarrow\mathbb P(V),\qquad x\longmapsto[1:x:\cdots:x^{g-1}].
$$

Write $R=\nu(\mathbb P^1)$.

A general hyperplane section of $R$ consists of $g-1$ distinct points $x_1,\ldots,x_{g-1}$ avoiding the branch points. The corresponding canonical [divisor](../../../../../divisor.md) on $X$ consists of the $g-1$ pairs $\pi^{-1}(x_j)$. Choosing one lift from each pair gives an effective [divisor](../../../../../divisor.md) $D$ with $h^0(D)=1$: the evaluation [matrix](../../../../../matrix.md) of the canonical forms has Vandermonde rank $g-1$. If instead a degree-$g-1$ sub-divisor contains an entire pair, it has at least two sections, because that pair is a fibre of $\pi$ and moves in a pencil. Every choice not taking exactly one point from each pair contains an entire pair. Therefore the generic smooth theta points over the hyperplane are exactly the independent choices of one lift in each pair, and

$$
\deg\Gamma=2^{g-1}.
$$

The cover of these choices is again the restriction of $Z$ to the open set of transverse sections of $R$ avoiding the $b_i$: the identification on a dense open follows from the [Abel theorem for divisors](../../../../../abel-theorem-for-divisors.md), and the choice cover is finite étale and normal. Its components would correspond to components of the [function field](../../../../../function-field-of-an-algebraic-variety.md) of the irreducible [theta divisor](../../../../../theta-divisor.md), so it is connected.

There are precisely two types of codimension-one branching. If a simple root $x_j$ crosses a branch point $b_i$, its two lifts exchange, giving nontrivial [monodromy](../../../../../monodromy.md) on the choices. This yields the hyperplane

$$
H_i=\{H\in P:\nu(b_i)\in H\}.
$$

If two roots collide away from the $b_i$, a local transverse parameter gives roots $x_0\pm\sqrt t$. Trivialize the two sheets of $\pi$ near $x_0$. Choices selecting different sheets for the two roots are exchanged when the roots exchange; hence this also causes branching. Its locus is $R^*$, the hypersurface of tangent hyperplanes to $R$. Away from these two loci all roots and all their lifts vary locally without branching, so there are no other branch components. Consequently

$$
\boxed{B=R^*\ \cup\ \bigcup_{i=1}^{2g+2}H_i.}
$$

For $g\ge3$, $R^*$ is irreducible and nonlinear. Indeed, hyperplane sections of the degree-$g-1$ [rational normal curve](../../../../../rational-normal-curve.md) are binary forms of degree $g-1$, and the repeated-root hypersurface is their irreducible [discriminant](../../../../../discriminant.md) of degree $2g-4\ge2$. Thus $B$ intrinsically separates into its single nonlinear component $R^*$ and its $2g+2$ linear components. Biduality recovers $R$, while dualizing $H_i$ recovers the point $\nu(b_i)$ on $R$.

These data recover the double cover uniquely. Identify $R$ with $\mathbb P^1$ and move infinity away from the recovered branch set. Its [function field](../../../../../function-field-of-an-algebraic-variety.md) is

$$
\mathbb C(x)\left(\sqrt{\prod_i(x-b_i)}\right).
$$

Any other quadratic extension with the same simple branch points has a defining rational function whose ratio to this product has even valuation everywhere. On $\mathbb P^1$ such a rational function is a constant times a square, and every nonzero complex constant is a square. The quadratic extensions are therefore isomorphic; their smooth projective models are isomorphic. This proves the hyperelliptic reconstruction. The branch locus also distinguishes the two cases: the nonhyperelliptic locus has one irreducible branch hypersurface, whereas the hyperelliptic locus has the additional $2g+2$ linear components.

Finally handle the small genera. In genus two, the [theta divisor](../../../../../theta-divisor.md) is $W_1$, the image of $X$ itself. The [Abelian sum map](../../../../../abel-map-of-an-algebraic-curve.md) on $X$ is injective because a principal [divisor](../../../../../divisor.md) $p-q$ with $p\ne q$ would give a degree-one map to $\mathbb P^1$. Its derivative is nonzero since the [canonical bundle](../../../../../canonical-bundle.md) has no base point, so this compact injective immersion identifies $X$ with $W_1$. In genus one the same argument identifies $X$ with its [Jacobian variety](../../../../../jacobian-variety.md) after choosing an origin. In genus zero the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) supplies a function with one simple pole, giving $X\cong\mathbb P^1$. These cases complete the proof: **the canonically polarized Jacobian determines the curve in every genus**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
