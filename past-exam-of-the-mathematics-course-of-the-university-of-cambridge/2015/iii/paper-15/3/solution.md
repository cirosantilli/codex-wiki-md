<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Integral groups for $M_4$.** Put $r=n-1$. The space $M_n$ is the [inversion mapping torus of a torus](../../../../../inversion-mapping-torus-of-a-torus.md), fibred over $S^1$ with fiber $T^r$. The [cohomology ring of a torus](../../../../../cohomology-ring-of-a-torus.md) is the [exterior algebra](../../../../../exterior-algebra.md) on $r$ degree-one generators. Inversion acts as $-1$ on each such generator, hence as $(-1)^q$ on $H^q(T^r;\mathbb Z)\cong\mathbb Z^{\binom rq}$.

The [Wang sequence](../../../../../wang-sequence.md) therefore gives

$$
0\longrightarrow
\operatorname{coker}(F^*-1:H^{q-1}(T^r;\mathbb Z)\to H^{q-1}(T^r;\mathbb Z))
\longrightarrow H^q(M_n;\mathbb Z)
\longrightarrow
\ker(F^*-1:H^q(T^r;\mathbb Z)\to H^q(T^r;\mathbb Z))
\longrightarrow0.
$$

The right-hand term is free, so this [short exact sequence](../../../../../short-exact-sequence.md) splits as a sequence of groups. In even fiber degree, $F^*-1=0$; in odd fiber degree it is multiplication by $-2$. For $r=3$ this computes the [integral cohomology of an inversion mapping torus](../../../../../integral-cohomology-of-an-inversion-mapping-torus.md):

$$
\boxed{
H^q(M_4;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&q=0,1,\\
\mathbb Z^3\oplus(\mathbb Z/2)^3,&q=2,\\
\mathbb Z^3,&q=3,\\
\mathbb Z/2,&q=4,\\
0,&\text{otherwise}.
\end{cases}}
$$

The top torsion group is consistent with $M_4$ being nonorientable: inversion of its three-dimensional fiber reverses orientation.

**Mod-two groups.** Over $\mathbb F_2$, inversion acts as the identity on the fiber [cohomology](../../../../../cohomology-split.md). The [Wang sequence](../../../../../wang-sequence.md) gives

$$
0\to H^{q-1}(T^r;\mathbb F_2)\to H^q(M_n;\mathbb F_2)
\to H^q(T^r;\mathbb F_2)\to0.
$$

Thus

$$
\boxed{\dim_{\mathbb F_2}H^q(M_n;\mathbb F_2)
=\binom rq+\binom r{q-1}=\binom nq,}
$$

with out-of-range binomial coefficients interpreted as zero. These are exactly the dimensions of the graded groups $H^*(T^n;\mathbb F_2)$.

**The intersection pairing for $M_2$.** The [mapping torus](../../../../../mapping-torus.md) of reflection of the circle is the [Klein bottle](../../../../../klein-bottle.md). Let $a$ be the section loop through a fixed point of the reflection and $b$ a fiber circle. They form a basis of $H_1(M_2;\mathbb F_2)$. The section has a normal neighborhood homeomorphic to a [Möbius band](../../../../../mobius-band.md), so it is one-sided and a transverse displacement meets it once modulo two. The fiber is two-sided and can be displaced disjointly. The two loops meet once. The [mod-two intersection pairing of the Klein bottle](../../../../../mod-two-intersection-pairing-of-the-klein-bottle.md) therefore has matrix

$$
Q=\begin{pmatrix}a\cdot a&a\cdot b\\b\cdot a&b\cdot b\end{pmatrix}
=\boxed{\begin{pmatrix}1&1\\1&0\end{pmatrix}}.
$$

Take the evaluation-dual basis $t,x\in H^1(M_2;\mathbb F_2)$, with $t(a)=1,t(b)=0$ and $x(a)=0,x(b)=1$. By [Poincare duality](../../../../../poincare-duality.md), the [cup product](../../../../../cup-product.md) matrix in this dual basis is $Q^{-1}$, not $Q$:

$$
Q^{-1}=\begin{pmatrix}0&1\\1&1\end{pmatrix}.
$$

Writing $w$ for the nonzero top class gives $t^2=0$, $tx=w$ and $x^2=w$. Hence the [cohomology ring](../../../../../cohomology-ring.md) is

$$
\boxed{H^*(M_2;\mathbb F_2)
\cong\mathbb F_2[t,x]/(t^2,x^2+tx),\qquad |t|=|x|=1.}
$$

These relations already force all degrees above two to vanish.

**The ring for general $n$.** For each of the $r$ fiber coordinates, projection induces $M_n\to M_2$. Pull back the classes above, calling the common base class $t$ and the fiber-coordinate classes $x_1,\ldots,x_r$. Naturality of the [cup product](../../../../../cup-product.md) gives $t^2=0$ and $x_i^2=t x_i$. The square-free products $x_I=\prod_{i\in I}x_i$ restrict to the [exterior algebra](../../../../../exterior-algebra.md) basis of the fiber [cohomology](../../../../../cohomology-split.md). The [Leray-Hirsch theorem](../../../../../leray-hirsch-theorem.md) then says that $x_I$ and $t x_I$ form an additive basis. This proves the full [mod-two cohomology ring of an inversion mapping torus](../../../../../mod-two-cohomology-ring-of-an-inversion-mapping-torus.md):

$$
\boxed{H^*(M_n;\mathbb F_2)\cong
\mathbb F_2[t,x_1,\ldots,x_{n-1}]
/(t^2,\ x_i^2+t x_i\ (1\leq i\leq n-1)).}
$$

For $n\geq2$, $x_i^2=t x_i$ is nonzero by this basis description. In the [cohomology ring of a torus](../../../../../cohomology-ring-of-a-torus.md) every degree-one class squares to zero: the generators square to zero and the cross terms occur twice in characteristic two. The [degree-one cup-square obstruction to ring isomorphism](../../../../../degree-one-cup-square-obstruction-to-ring-isomorphism.md) therefore proves that **the rings are not isomorphic for any $n\geq2$**, despite their isomorphic graded groups. For $n=1$, both spaces are circles and the rings are isomorphic. Even if grading is forgotten, the rings differ for $n\geq2$: every element of the torus ring has square either zero or one, whereas $x_i^2=t x_i$ is nonzero and is not the unit.

**Integral cup products in $M_4$.** To specify $H^*(M_4;\mathbb Z)$ also as a ring, let $a\in H^1$ be the pullback of the positive generator of $H^1(S^1;\mathbb Z)$. Let $\rho$ denote reduction modulo two and set $\tau_i=\widehat\beta(x_i)$ using the [integral Bockstein homomorphism](../../../../../integral-bockstein-homomorphism.md). The [degree-one Bockstein square identity](../../../../../degree-one-bockstein-square-identity.md) gives $\rho\tau_i=x_i^2=t x_i$, so the $\tau_i$ are the three independent order-two classes in degree two. Choose free classes $b_{12},b_{13},b_{23}\in H^2$ which restrict to the corresponding two-fold fiber products and have reductions $\rho b_{ij}=x_i x_j$. Such choices exist: reduction in degree two is surjective because $H^3(M_4;\mathbb Z)$ is free, and adding the $\tau_i$ removes any $t x_i$ terms from an initial lift.

The [Wang sequence](../../../../../wang-sequence.md) identifies $a b_{12},a b_{13},a b_{23}$ as a free basis of $H^3$. Let $\kappa$ generate $H^4\cong\mathbb Z/2$, with $\rho\kappa=t x_1x_2x_3$. Reduction in degree four is an isomorphism. The [integral cup products in the four-dimensional inversion mapping torus](../../../../../integral-cup-products-in-the-four-dimensional-inversion-mapping-torus.md) are consequently determined by

$$
\begin{aligned}
&a^2=0,\quad a\tau_i=0,\quad \tau_i\tau_j=0,\quad b_{ij}^2=0,\\
&\boxed{b_{12}b_{13}=b_{12}b_{23}=b_{13}b_{23}=\kappa},\\
&\boxed{b_{ij}\tau_k=
\begin{cases}\kappa,&\{i,j,k\}=\{1,2,3\},\\0,&\text{otherwise},\end{cases}}\\
&2\tau_i=2\kappa=0.
\end{aligned}
$$

Together with the unit, graded commutativity and vanishing above degree four, these give every product. For example, $\rho(b_{12}b_{13})=x_1^2x_2x_3=t x_1x_2x_3$, whereas $\rho(b_{12}^2)=t^2x_1x_2=0$. The products $a\tau_i$ vanish because they are torsion in the free group $H^3$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
