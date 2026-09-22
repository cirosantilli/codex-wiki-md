# Paper 159

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_159.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_159.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 159](paper-159.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Picard group](../../../ringed-space.md#picard-group) $\operatorname{Pic}(X)$ is the set of isomorphism classes of [line bundles](../../../ringed-space.md#line-bundle) on $X$, with tensor product as addition, the trivial bundle as zero and the dual bundle as inverse. On a smooth projective surface, line bundles can be represented by divisors. The [intersection pairing on the Picard group of a surface](../../../algebraic-geometry.md#intersection-pairing-on-the-picard-group-of-a-surface) is the symmetric bilinear map

$$
\operatorname{Pic}(X)\times\operatorname{Pic}(X)\longrightarrow\mathbb Z,
\qquad ([D],[E])\longmapsto D\cdot E,
$$

obtained by moving the divisors into proper position and counting their intersections with multiplicity.

The surface

$$
\mathbb P_{\mathbb P^1}(\mathcal O\oplus\mathcal O(1))
$$

is the first [Hirzebruch surface](../../../toric-geometry.md#hirzebruch-surface) $\mathbb F_1$. If $S$ is its [negative section](../../../toric-geometry.md#negative-section-of-a-hirzebruch-surface) and $F$ a fiber of the ruling, its [Picard lattice of a Hirzebruch surface](../../../algebraic-geometry.md#picard-lattice-of-a-hirzebruch-surface) is

$$
\operatorname{Pic}(\mathbb F_1)=\mathbb ZS\oplus\mathbb ZF,
\qquad
S^2=-1,quad S\cdot F=1,quad F^2=0.
$$

Now let $\pi:X\to\mathbb P^2$ be the given nonisomorphic [birational](../../../algebraic-geometry.md#birational-variety) morphism. A birational morphism between smooth projective surfaces factors as a nonempty sequence of point blowups. Let $H=\pi^*[\text{line}]$, and take the total transform $E$ on $X$ of the exceptional curve of the first blowup. The [intersection formula for blowing up a surface](../../../algebraic-geometry.md#intersection-formula-for-blowing-up-a-surface) gives

$$
H^2=1,qquad E^2=-1,qquad H\cdot E=0.
$$

Therefore the nonzero [Picard group](../../../ringed-space.md#picard-group) element $H+E$ satisfies

$$
(H+E)^2=1-1=0.
$$

This is the [isotropic divisor from a nontrivial birational morphism to the projective plane](../../../algebraic-geometry.md#isotropic-divisor-from-a-nontrivial-birational-morphism-to-the-projective-plane).

For a morphism $\phi:\mathbb P^2\to\mathbb P^n$, the pullback of the hyperplane bundle has the form

$$
\phi^*\mathcal O_{\mathbb P^n}(1)\cong\mathcal O_{\mathbb P^2}(d)
$$

for an integer $d\geq0$. If a line $\ell$ is contracted to a point, this bundle restricts trivially to $\ell$, whereas

$$
\mathcal O_{\mathbb P^2}(d)|_\ell\cong\mathcal O_{\mathbb P^1}(d).
$$

Its [degree](../../../algebraic-geometry.md#degree-of-a-divisor) is therefore zero, so $d=0$. The homogeneous sections defining $\phi$ are then constants, and $\phi$ is constant. This proves the [morphism from the projective plane contracting a line](../../../algebraic-geometry.md#morphism-from-the-projective-plane-contracting-a-line) criterion.

Finally choose an integer $r>C^2$ and blow up $r$ distinct points of the smooth curve $C$. For the resulting morphism $\pi:X'\to X$, let $E_1,\ldots,E_r$ be the [exceptional curves](../../../complex-geometry.md#exceptional-divisor). The [strict transform](../../../complex-geometry.md#strict-transform) is

$$
C'=\pi^*C-\sum_{i=1}^rE_i,
$$

and the [self-intersection after blowing up points on a smooth curve](../../../algebraic-geometry.md#self-intersection-after-blowing-up-points-on-a-smooth-curve) formula gives

$$
(C')^2=C^2-r<0.
$$

Blowing up a smooth point of a smooth curve does not change that curve itself, so $\pi|_{C'}:C'\to C$ is an isomorphism.

## 2

↑ **Parent:** [Paper 159](paper-159.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [minimal algebraic surface](../../../algebraic-geometry.md#minimal-algebraic-surface) is a smooth projective surface containing no [exceptional curve of the first kind](../../../algebraic-geometry.md#exceptional-curve-of-the-first-kind), namely no smooth rational curve of self-intersection $-1$. An [abelian surface](../../../algebraic-geometry.md#abelian-surface) contains no rational curve because every morphism from $\mathbb P^1$ to an [abelian variety](../../../abelian-variety.md) is constant. It therefore has no $(-1)$-curve and is minimal.

For every $n\geq2$, the [Minimal Hirzebruch surface](../../../algebraic-geometry.md#minimal-hirzebruch-surface) $\mathbb F_n$ is a rational minimal surface. These surfaces are pairwise nonisomorphic: the negative section is the unique irreducible curve of negative self-intersection and has square $-n$, so an isomorphism would recover $n$. Thus there are infinitely many nonisomorphic minimal rational surfaces.

A [K3 surface](../../../complex-geometry.md#k3-surface) is a smooth projective surface $X$ with $K_X\cong\mathcal O_X$ and $H^1(X,\mathcal O_X)=0$. For a smooth curve $C\subset X$ of [geometric genus](../../../normalization-of-an-algebraic-curve.md#geometric-genus) $g$, the [adjunction formula](../../../complex-geometry.md#adjunction-formula) gives

$$
2g-2=C\cdot(C+K_X)=C^2,
$$

and hence

$$
\boxed{C^2=2g-2}.
$$

An [elliptic surface](../../../algebraic-geometry.md#elliptic-surface) is a smooth projective surface with a morphism to a smooth curve whose generic fiber is a smooth genus-one curve. If $E$ is an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve), projection

$$
\mathbb P^1\times E\longrightarrow\mathbb P^1
$$

is an elliptic fibration. Its canonical bundle is pulled back from $K_{\mathbb P^1}$, so every positive pluricanonical space vanishes and the [Kodaira dimension](../../../algebraic-geometry.md#kodaira-dimension) is $-\infty$. This supplies the requested negative-Kodaira-dimension example.

For an elliptically fibered K3 surface, choose a smooth quartic $X\subseteq\mathbb P^3$ containing a line $L$. The [canonical bundle of a smooth projective hypersurface](../../../algebraic-topology.md#canonical-bundle-of-a-smooth-projective-hypersurface) formula makes $K_X$ trivial, and the standard cohomology sequence gives $H^1(X,\mathcal O_X)=0$, so $X$ is K3. The pencil of planes through $L$ cuts $X$ into $L$ plus a residual plane cubic. The residual linear system $|H-L|$ is basepoint-free, has square zero and defines a morphism $X\to\mathbb P^1$ whose generic fiber is a smooth plane cubic. This is the [Elliptic K3 surface from a quartic containing a line](../../../complex-geometry.md#elliptic-k3-surface-from-a-quartic-containing-a-line).

A [surface of general type](../../../algebraic-geometry.md#surface-of-general-type) is a smooth projective surface of [Kodaira dimension](../../../algebraic-geometry.md#kodaira-dimension) two. Let $B\subseteq\mathbb P^2$ be a smooth plane curve of degree eight and let

$$
\pi:X\longrightarrow\mathbb P^2
$$

be the degree-two cover branched along $B$. The branch-cover canonical-bundle formula gives

$$
K_X=\pi^*\left(K_{\mathbb P^2}+4H\right)=\pi^*H.
$$

This divisor is ample, so $X$ is a [double plane of general type](../../../algebraic-geometry.md#double-plane-of-general-type) and $\pi$ is the required finite morphism of degree two.

## 3

↑ **Parent:** [Paper 159](paper-159.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [irregularity of an algebraic surface](../../../algebraic-geometry.md#irregularity-of-an-algebraic-surface) and the [geometric genus of an algebraic surface](../../../algebraic-geometry.md#geometric-genus-of-an-algebraic-surface) are respectively

$$
q(X)=h^1(X,\mathcal O_X)=h^0(X,\Omega_X^1),
\qquad
p_g(X)=h^0(X,K_X)=h^2(X,\mathcal O_X).
$$

If $\pi:X'\to X$ is the blowup at a point with [exceptional divisor](../../../complex-geometry.md#exceptional-divisor) $E$, then

$$
K_{X'}=\pi^*K_X+E.
$$

A holomorphic two-form on $X$ pulls back to one on $X'$. Conversely, a holomorphic two-form on $X'$ descends across $E$: locally it is a form on the punctured smooth surface $X\setminus\{p\}$, and its coefficients extend over the codimension-two point $p$. Equivalently, $\pi_*K_{X'}=K_X$. Pullback is therefore an isomorphism

$$
H^0(X,K_X)\cong H^0(X',K_{X'}),
$$

which proves the [birational invariance of the geometric genus of a surface](../../../algebraic-geometry.md#birational-invariance-of-the-geometric-genus-of-a-surface) in this case.

Let $X=C\times D$, where both smooth projective curves have positive genus. The [Künneth theorem](../../../cohomology.md#kunneth-theorem) gives the [irregularity of a product of curves](../../../algebraic-geometry.md#irregularity-of-a-product-of-curves)

$$
q(X)=g(C)+g(D)>0.
$$

If a surface is a hypersurface in projective space, dimension forces it to be a smooth hypersurface $Y\subseteq\mathbb P^3$. From

$$
0\longrightarrow\mathcal O_{\mathbb P^3}(-d)
\longrightarrow\mathcal O_{\mathbb P^3}
\longrightarrow\mathcal O_Y
\longrightarrow0
$$

and the intermediate cohomology vanishing for line bundles on projective space, one obtains $H^1(Y,\mathcal O_Y)=0$. Thus every such hypersurface has irregularity zero, whereas $X$ has positive irregularity. Hence $C\times D$ is not isomorphic to a hypersurface. This is the [product of positive-genus curves is not a projective hypersurface](../../../algebraic-geometry.md#product-of-positive-genus-curves-is-not-a-projective-hypersurface) obstruction.

The [Albanese variety](../../../algebraic-geometry.md#albanese-variety) $\operatorname{Alb}(X)$ is the universal [abelian variety](../../../abelian-variety.md) receiving a pointed morphism from $X$, and

$$
\dim\operatorname{Alb}(X)=q(X).
$$

Let the smooth image curve of the Albanese morphism be $C$ of genus $g$. Pullback of holomorphic one-forms along the dominant map $X\to C$ is injective, giving $g\leq q(X)$. On the other hand, the universal property of the Jacobian extends $C\to\operatorname{Alb}(X)$ to a homomorphism

$$
\operatorname{Jac}(C)\longrightarrow\operatorname{Alb}(X).
$$

The Albanese image generates the entire Albanese variety, so this homomorphism is surjective and $q(X)\leq\dim\operatorname{Jac}(C)=g$. Therefore the [Irregularity from a smooth Albanese curve image](../../../algebraic-geometry.md#irregularity-from-a-smooth-albanese-curve-image) is

$$
\boxed{q(X)=g}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
