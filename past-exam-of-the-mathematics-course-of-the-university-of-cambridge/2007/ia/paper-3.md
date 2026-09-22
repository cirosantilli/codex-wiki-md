# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2007/PaperIA_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2007/PaperIA_3.pdf)

**Table of contents**

- [1D](#1d)
  - [Solution](#1d/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3A](#3a)
  - [i](#3a/i)
    - [Solution](#3a/i/solution)
  - [ii](#3a/ii)
    - [Solution](#3a/ii/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
- [6D](#6d)
  - [Solution](#6d/solution)
  - [i](#6d/i)
    - [Solution](#6d/i/solution)
  - [ii](#6d/ii)
    - [Solution](#6d/ii/solution)
  - [iii](#6d/iii)
    - [Solution](#6d/iii/solution)
  - [iv](#6d/iv)
    - [Solution](#6d/iv/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
  - [i](#7d/i)
    - [Solution](#7d/i/solution)
  - [ii](#7d/ii)
    - [Solution](#7d/ii/solution)
  - [iii](#7d/iii)
    - [Solution](#7d/iii/solution)
  - [iv](#7d/iv)
    - [Solution](#7d/iv/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9A](#9a)
  - [i](#9a/i)
    - [Solution](#9a/i/solution)
  - [ii](#9a/ii)
    - [Solution](#9a/ii/solution)
- [10A](#10a)
  - [Solution](#10a/solution)
- [11A](#11a)
  - [Solution](#11a/solution)
  - [i](#11a/i)
    - [Solution](#11a/i/solution)
  - [ii](#11a/ii)
    - [Solution](#11a/ii/solution)
  - [iii](#11a/iii)
    - [Solution](#11a/iii/solution)
- [12A](#12a)
  - [Solution](#12a/solution)

## 1D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1d/solution">Solution</h3>

↑ **Parent:** [1D](#1d)

Let $p$ be a [permutation](../../../combinatorics.md#permutation) of the finite set. Starting from $a$, repeatedly apply $p$. Some iterate repeats; because $p$ is invertible, the first repeat closes the sequence at $a$. More explicitly, if $p^i(a)=p^j(a)$ with $0\le i<j$, applying $p^{-i}$ gives $p^{j-i}(a)=a$. If $r$ is the least positive return time, the elements $a,p(a),\ldots,p^{r-1}(a)$ are distinct and form one [permutation cycle](../../../finite-group-theory.md#permutation-cycle). If the set is not exhausted, start again at an unused element. Two such sets cannot overlap: an overlap lets an inverse iterate express either starting point as an iterate of the other, making the sets identical. Thus this process partitions the set into [disjoint permutation cycles](../../../finite-group-theory.md#disjoint-permutation-cycles). On each part its cycle acts exactly as $p$ and the other cycles fix the elements. Their product therefore equals $p$. This proves existence of the [cycle decomposition of a permutation](../../../mathematics.md#cycle-decomposition-of-a-permutation), including one-cycles for fixed points.

Use the composition convention that the rightmost [permutation](../../../combinatorics.md#permutation) acts first. For the specified product, the images are

$$
1\mapsto2\mapsto3\mapsto1,\qquad4\mapsto5\mapsto4,\qquad6\mapsto7\mapsto8\mapsto6.
$$

Hence

$$
\boxed{\sigma\tau=(123)(45)(678),\qquad\operatorname{ord}(\sigma\tau)=6.}
$$

The [order of a group element](../../../group-theory.md#order-of-a-group-element) here is the least positive exponent making every cycle return to the identity. It must be divisible by each cycle length, and any common multiple does make every cycle return. The [least common multiple](../../../number-theory.md#least-common-multiple) of $3,2,3$ is six.

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

A [group isomorphism](../../../algebra.md#group-isomorphism) $f:G\to H$ is a bijection satisfying $f(xy)=f(x)f(y)$ for all $x,y\in G$. It sends the identity to the identity and satisfies $f(x^k)=f(x)^k$. Applying its inverse shows that it preserves the [order of a group element](../../../group-theory.md#order-of-a-group-element) exactly.

The [cyclic group](../../../group.md#cyclic-group) $C_8$ has an element of order eight. Every element of the [direct product of groups](../../../group-theory.md#direct-product-of-groups) $C_4\times C_2$ has fourth power equal to the identity, and a generator of the first factor paired with the identity of the second has order four. Every nonidentity element of $C_2\times C_2\times C_2$ has order two. Thus their maximum element orders are respectively $8,4,2$, which an isomorphism would preserve. **The three groups are pairwise nonisomorphic.**

For a fourth example take the [dihedral group](../../../finite-group-theory.md#dihedral-group) of symmetries of a square. It consists of four rotations and four reflections, so has order eight. With $r$ a quarter-turn and $s$ a reflection, $srs=r^{-1}\ne r$, showing $sr\ne rs$. This [group](../../../group.md) is nonabelian, whereas all three displayed [direct products of groups](../../../group-theory.md#direct-product-of-groups) are [abelian groups](../../../group.md#abelian-group). Since a [group isomorphism](../../../algebra.md#group-isomorphism) preserves commutativity, **the square's dihedral group is isomorphic to none of them**. Its order is eight regardless of whether a notation convention calls it $D_4$ or $D_8$.

## 3A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3a/i">i</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/i/solution">Solution</h4>

↑ **Parent:** [I](#3a/i)

For a regular differentiable curve $\mathbf x(t)$, its speed is $ds/dt=|\mathbf x'(t)|>0$, where $s$ is [arc length](../../../riemannian-geometry.md#arc-length). The oriented [unit tangent vector](../../../differential-geometry.md#unit-tangent-vector) is $\widehat{\mathbf T}=\mathbf x'/|\mathbf x'|$. The [curvature of a space curve](../../../differential-geometry.md#curvature-of-a-space-curve) is $\kappa=|d\widehat{\mathbf T}/ds|$. Equivalently, for a twice differentiable regular curve,

$$
\kappa=\frac{|\mathbf x'\times\mathbf x''|}{|\mathbf x'|^3}.
$$

For the [helix](../../../topology.md#helix), differentiation gives $\mathbf x'=(-a\sin t,a\cos t,b)$ and speed $v=\sqrt{a^2+b^2}$. Consequently

$$
\boxed{\widehat{\mathbf T}(t)=\frac{(-a\sin t,a\cos t,b)}{\sqrt{a^2+b^2}},\qquad\kappa=\frac{|a|}{a^2+b^2}.}
$$

Indeed $d\widehat{\mathbf T}/dt=(-a\cos t,-a\sin t,0)/v$ has magnitude $|a|/v$, and division by $ds/dt=v$ gives the result. This requires $(a,b)\ne(0,0)$; the excluded constant curve has no well-defined [unit tangent vector](../../../differential-geometry.md#unit-tangent-vector). For $a=0,b\ne0$ the curve is a straight line with zero [curvature of a space curve](../../../differential-geometry.md#curvature-of-a-space-curve).

<h3 id="3a/ii">ii</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3a/ii)

Write the surface as the level set $F(x,y,z)=x^2y^3-y+1-z=0$. The [gradient](../../../calculus.md#gradient) is normal to a regular level surface because differentiating $F$ along any surface curve gives $\nabla F\cdot\mathbf v=0$ for its tangent vector. At the specified point,

$$
\nabla F=(2xy^3,3x^2y^2-1,-1)=(2,2,-1).
$$

Thus a [normal vector](../../../differential-geometry.md#normal-vector) and a unit normal are $(2,2,-1)$ and $(2,2,-1)/3$, respectively. The tangent-plane displacement is perpendicular to that normal, giving

$$
\boxed{\mathbf n=(2,2,-1),\qquad 2(x-1)+2(y-1)-(z-1)=0,\quad\text{or}\quad z=2x+2y-3.}
$$

Reversing the normal's sign gives the same plane.

## 4A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

Use [suffix notation](../../../linear-algebra.md#einstein-notation), with repeated indices summed from one to three. The [cross product](../../../vector-space.md#cross-product), [divergence](../../../calculus.md#divergence), and [curl](../../../calculus.md#curl) have components $(\mathbf A\times\mathbf B)_i=\epsilon_{ijk}A_jB_k$, $\nabla\cdot\mathbf A=\partial_iA_i$, and $(\nabla\times\mathbf A)_i=\epsilon_{ijk}\partial_jA_k$. Here $\epsilon$ is the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol).

The [product rule](../../../calculus.md#product-rule) gives

$$
\partial_i(\epsilon_{ijk}A_jB_k)=\epsilon_{ijk}(\partial_iA_j)B_k+\epsilon_{ijk}A_j\partial_iB_k.
$$

Using the cyclic identity $\epsilon_{ijk}=\epsilon_{kij}$ in the first term and $\epsilon_{ijk}=-\epsilon_{jik}$ in the second identifies these terms as $B_k(\nabla\times\mathbf A)_k$ and $-A_j(\nabla\times\mathbf B)_j$. Therefore

$$
\boxed{\nabla\cdot(\mathbf A\times\mathbf B)=\mathbf B\cdot(\nabla\times\mathbf A)-\mathbf A\cdot(\nabla\times\mathbf B).}
$$

For the second identity, contract two [Levi-Civita symbols](../../../calculus.md#levi-civita-symbol), using $\epsilon_{ijk}\epsilon_{klm}=\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl}$:

$$
\begin{aligned}
[\nabla\times(\mathbf A\times\mathbf B)]_i
&=\epsilon_{ijk}\epsilon_{klm}\partial_j(A_lB_m)\\
&=\partial_j(A_iB_j-A_jB_i)\\
&=B_j\partial_jA_i+A_i\partial_jB_j-A_j\partial_jB_i-B_i\partial_jA_j.
\end{aligned}
$$

The four component expressions translate into

$$
\boxed{\nabla\times(\mathbf A\times\mathbf B)=(\mathbf B\cdot\nabla)\mathbf A-\mathbf B(\nabla\cdot\mathbf A)-(\mathbf A\cdot\nabla)\mathbf B+\mathbf A(\nabla\cdot\mathbf B).}
$$

Both derivations require only continuously differentiable [vector fields](../../../calculus.md#vector-field); no additional divergence-free assumptions are used.

## 5D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

The [order of a group element](../../../group-theory.md#order-of-a-group-element) $x$ is the least positive integer $r$ with $x^r=e$, or infinity if none exists. In a [finite group](../../../group.md#finite-group), some two powers among $e,x,\ldots,x^{|G|}$ coincide; cancellation then gives a positive power equal to $e$, so $r$ exists. The generated [cyclic group](../../../group.md#cyclic-group) $H=\langle x\rangle$ consists of the distinct elements $e,x,\ldots,x^{r-1}$ and has size $r$.

We now prove the needed divisibility directly by [cosets](../../../group-theory.md#coset). Multiplication by $g$ bijects $H$ with the left [coset](../../../group-theory.md#coset) $gH$, so every left [coset](../../../group-theory.md#coset) has $r$ elements. If $gH$ and $hH$ intersect, write $ga=hb$ with $a,b\in H$. Then $h^{-1}g=ba^{-1}\in H$, which implies $gH=hH$. Thus distinct left [cosets](../../../group-theory.md#coset) are disjoint, and every element of $G$ belongs to its own left [coset](../../../group-theory.md#coset). The finite set $G$ is partitioned into, say, $k$ such [cosets](../../../group-theory.md#coset). Hence $|G|=kr$ and

$$
\boxed{\operatorname{ord}(x)\mid |G|.}
$$

This supplies the counting argument underlying [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), rather than appealing to it or to an unproved orbit formula.

A divisor of $|G|$ need not occur as an element order. Use $G=C_2\times C_2\times C_2$, of order eight, and $d=4<8$. Every element has square equal to the identity, so there is no element of order four. Thus **the proposed converse is false, even for an abelian group**.

For the [direct product of groups](../../../group-theory.md#direct-product-of-groups) $C_m\times C_n$, let $a,b$ generate the factors. The least $k>0$ for which $(a,b)^k=(e,e)$ is the [least common multiple](../../../number-theory.md#least-common-multiple) of $m,n$. If $m,n$ are [coprime](../../../number-theory.md#coprime-integers), this is $mn$, the size of the whole product, so $(a,b)$ generates every element. Conversely, for any pair $(u,v)$ its order is $\operatorname{lcm}(\operatorname{ord}u,\operatorname{ord}v)$ and divides $\operatorname{lcm}(m,n)$. If $\gcd(m,n)>1$, that bound is $mn/\gcd(m,n)<mn$, so no element can generate the product. Therefore

$$
\boxed{C_m\times C_n\text{ is cyclic exactly when }\gcd(m,n)=1.}
$$

This is the [cyclicity of a product of two finite cyclic groups](../../../group-theory.md#cyclicity-of-a-product-of-two-finite-cyclic-groups); the general pair-order criterion is the [order of a direct-product element](../../../group-theory.md#order-of-a-direct-product-element).

## 6D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6d/solution">Solution</h3>

↑ **Parent:** [6D](#6d)

A [subgroup](../../../group.md#subgroup) $H$ is a [normal subgroup](../../../group-theory.md#normal-subgroup) of $G$ if $gHg^{-1}=H$ for every $g\in G$, equivalently if $gH=Hg$ for every $g$. In the [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_3$, the [subgroup](../../../group.md#subgroup) $A_3=\{e,(123),(132)\}$ is normal: conjugation relabels a three-cycle as a three-cycle, so preserves this set. By contrast, $\{e,(12)\}$ is not normal because conjugating $(12)$ by $(23)$ gives $(13)$ outside the [subgroup](../../../group.md#subgroup).

If $H$ is normal, define a product on its left [cosets](../../../group-theory.md#coset) by $(gH)(kH)=(gk)H$. To check that this [quotient group](../../../group-theory.md#quotient-group) operation is well-defined, take different representatives $gh_1$ and $kh_2$, with $h_1,h_2\in H$. Their product is

$$
gh_1kh_2=gk(k^{-1}h_1k)h_2.
$$

Normality puts the last two factors in $H$, so its [coset](../../../group-theory.md#coset) is exactly $gkH$. Associativity follows from that in $G$, the identity [coset](../../../group-theory.md#coset) is $H$, and the inverse of $gH$ is $g^{-1}H$. Thus all the group axioms hold, and the projection $g\mapsto gH$ is a [group homomorphism](../../../group-theory.md#group-homomorphism).

<h3 id="6d/i">i</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/i/solution">Solution</h4>

↑ **Parent:** [I](#6d/i)

**Always true.** Suppose $G=\langle g\rangle$. If $H$ is nontrivial, let $d$ be the least positive integer with $g^d\in H$. For any $g^k\in H$, divide $k=qd+r$ with $0\le r<d$. Since $g^r=g^k(g^d)^{-q}\in H$, minimality forces $r=0$. Hence $H=\langle g^d\rangle$ is a [cyclic group](../../../group.md#cyclic-group). The trivial [subgroup](../../../group.md#subgroup) is cyclic as well. Every [coset](../../../group-theory.md#coset) in $G/H$ is $g^kH=(gH)^k$, so the [quotient group](../../../group-theory.md#quotient-group) is generated by $gH$. This proves the [subgroups and quotients of a cyclic group](../../../group.md#subgroups-and-quotients-of-a-cyclic-group) assertion.

<h3 id="6d/ii">ii</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6d/ii)

**Can be false.** Take the [Klein four-group](../../../finite-group-theory.md#klein-four-group) $G=C_2\times C_2$ and $H=C_2\times\{e\}$. It is a [normal subgroup](../../../group-theory.md#normal-subgroup) because $G$ is an [abelian group](../../../group.md#abelian-group). Both $H$ and $G/H$ have order two and are [cyclic groups](../../../group.md#cyclic-group). But every nonidentity element of $G$ has order two, so none generates its four elements. Thus $G$ is not cyclic.

<h3 id="6d/iii">iii</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6d/iii)

**Always true.** Elements of a [subgroup](../../../group.md#subgroup) $H$ commute when they are elements of an [abelian group](../../../group.md#abelian-group) $G$, so $H$ is abelian. In the [quotient group](../../../group-theory.md#quotient-group), $(gH)(kH)=gkH=kgH=(kH)(gH)$. Therefore $G/H$ is abelian too.

<h3 id="6d/iv">iv</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6d/iv)

**Can be false.** Use $G=S_3$ and the [normal subgroup](../../../group-theory.md#normal-subgroup) $H=A_3$ from the root solution. The [subgroup](../../../group.md#subgroup) $H$ is cyclic of order three, hence an [abelian group](../../../group.md#abelian-group), and the [quotient group](../../../group-theory.md#quotient-group) has the two [cosets](../../../group-theory.md#coset) $A_3$ and $(12)A_3$, so is cyclic of order two and abelian. Yet $(12)(23)=(123)$ whereas $(23)(12)=(132)$, proving that $S_3$ is not abelian. An abelian kernel and an abelian quotient do not force all elements of the original group to commute.

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

Allow an [eigenvector](../../../linear-operator-theory.md#eigenvector) $v\ne0$ to have complex entries, since real matrices can initially have complex [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Write $v^*$ for its conjugate transpose. Reality of $A$ gives $A^*=A^T$; symmetry then gives $A^*=A$. Thus $A$ is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). The scalar $v^*Av$ equals its complex conjugate, because $(v^*Av)^*=v^*A^*v=v^*Av$. If $Av=\lambda v$, then

$$
\lambda=\frac{v^*Av}{v^*v}\in\mathbb R,
$$

since $v^*v>0$. This proves that all [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are real. The equality $A^*=A^T$ is precisely where reality was used; a complex symmetric matrix need not be Hermitian, as $iI$ illustrates.

If $Au=\lambda u$ and $Av=\mu v$, then $u^*Av=\mu u^*v$, but also $u^*Av=(Au)^*v=\overline\lambda u^*v=\lambda u^*v$. Consequently $(\mu-\lambda)u^*v=0$. Distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) force $u^*v=0$. For real [eigenvectors](../../../linear-operator-theory.md#eigenvector) this is ordinary Euclidean orthogonality. These arguments establish [real symmetric spectral orthogonality](../../../linear-algebra.md#real-symmetric-spectral-orthogonality) without assuming a diagonalization in advance.

A real [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) satisfies $P^TP=I$, equivalently $P^{-1}=P^T$. If $A$ is symmetric,

$$
(P^{-1}AP)^T=(P^TAP)^T=P^TA^TP=P^TAP=P^{-1}AP,
$$

so orthogonal similarity preserves symmetry. An arbitrary real invertible change of basis need not do so. For example,

$$
A=\begin{pmatrix}1&0\\0&2\end{pmatrix},\qquad P=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad P^{-1}AP=\begin{pmatrix}1&-1\\0&2\end{pmatrix}.
$$

The final matrix is not symmetric. **Orthogonal similarity preserves real symmetry; general similarity does not.**

<h3 id="7d/i">i</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/i/solution">Solution</h4>

↑ **Parent:** [I](#7d/i)

Take

$$
\boxed{B=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.}
$$

Its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is $\lambda^2+1$, whose roots are $i$ and $-i$. Thus this real [matrix](../../../vector-space.md#matrix) has no real [eigenvalues](../../../linear-operator-theory.md#eigenvalue).

<h3 id="7d/ii">ii</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7d/ii)

Take the [Jordan block](../../../linear-operator-theory.md#jordan-block)

$$
\boxed{C=\begin{pmatrix}1&1\\0&1\end{pmatrix}.}
$$

Its only [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is one. An [eigenvector](../../../linear-operator-theory.md#eigenvector) satisfies $(C-I)v=0$, so its second coordinate vanishes; the [eigenspace](../../../linear-operator-theory.md#eigenspace) is one-dimensional. A [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) of size two requires a basis of two independent [eigenvectors](../../../linear-operator-theory.md#eigenvector), which this matrix lacks even over $\mathbb C$.

<h3 id="7d/iii">iii</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7d/iii)

Use

$$
\boxed{D=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.}
$$

It has independent complex [eigenvectors](../../../linear-operator-theory.md#eigenvector) $(1,-i)^T$ and $(1,i)^T$, with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $i$ and $-i$. Taking these as columns gives an invertible complex matrix $P$ with $P^{-1}DP=\operatorname{diag}(i,-i)$, so $D$ is a [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) over $\mathbb C$. It cannot be diagonalized over $\mathbb R$, since a real diagonal matrix would have real [eigenvalues](../../../linear-operator-theory.md#eigenvalue), whereas similarity preserves the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial).

<h3 id="7d/iv">iv</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#7d/iv)

Take

$$
\boxed{E=\begin{pmatrix}1&1\\0&2\end{pmatrix}.}
$$

The real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are one and two, with eigenlines spanned by $(1,0)^T$ and $(1,1)^T$ respectively. These independent vectors form a real [eigenbasis](../../../linear-operator-theory.md#eigenbasis), so $E$ is a [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) over $\mathbb R$. Their [inner product](../../../linear-algebra.md#inner-product) is one, and any two nonzero vectors on those eigenlines have nonzero [inner product](../../../linear-algebra.md#inner-product). Rescaling can normalize their lengths but cannot make them orthogonal. Hence no orthonormal [eigenbasis](../../../linear-operator-theory.md#eigenbasis) exists.

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

Work on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere), including zero and infinity. For $j(z)=1/z$, two iterations give the identity and one does not, so $\operatorname{ord}(j)=2$. For $k(z)=1/(1-z)$, direct composition gives

$$
k^2(z)=\frac{z-1}{z},\qquad k^3(z)=z.
$$

Neither $k$ nor $k^2$ is the identity; in particular $0\mapsto1\mapsto\infty\mapsto0$. Thus

$$
\boxed{\operatorname{ord}(z\mapsto1/z)=2,\qquad\operatorname{ord}(z\mapsto1/(1-z))=3.}
$$

To prove the [Möbius conjugacy normal forms](../../../group-theory.md#mobius-conjugacy-normal-forms), write a [Möbius transformation](../../../group-theory.md#mobius-transformation) as $f(z)=(az+b)/(cz+d)$ with $ad-bc\ne0$. A finite fixed point satisfies $cz^2+(d-a)z-b=0$. If $c\ne0$, this quadratic has two roots counting multiplicity, and infinity is not fixed. If $c=0$, the transformation is affine, infinity is fixed, and there is one further finite fixed point unless its slope is one. A nonidentity slope-one affine map is a nonzero translation with only infinity fixed. Thus any nonidentity [Möbius transformation](../../../group-theory.md#mobius-transformation) has one or two distinct fixed points.

If there are two, say $p,q$, choose a [Möbius transformation](../../../group-theory.md#mobius-transformation) $h$ taking them to zero and infinity. For finite $p,q$ one can use $h(z)=(z-p)/(z-q)$; the cases involving infinity use an affine map or reciprocal. The conjugate $hfh^{-1}$ fixes zero and infinity. Fixing infinity sets its denominator's linear coefficient to zero, and fixing zero sets its numerator's constant term to zero; hence it is $z\mapsto\mu z$ with $\mu\ne0$.

If there is only one fixed point, send it to infinity. The conjugate has the affine form $az+b$. If $a\ne1$, $b/(1-a)$ would be another fixed point, which is impossible; therefore $a=1,b\ne0$. Conjugating this translation by $z\mapsto z/b$ yields $z\mapsto z+1$. The identity is already the scaling $\mu=1$. This proves the classification, and invertibility excludes $\mu=0$.

Conjugation carries fixed-point sets bijectively. The translation $z+1$ has exactly one fixed point, infinity. A nonidentity scaling has the two fixed points zero and infinity, while the identity fixes every point. Therefore **$z+1$ is not conjugate to any scaling**.

Finally let $f$ have finite positive order $n$. A nonzero translation has infinite order, since its $k$th iterate is $z+k$ after normalization. Thus $f$ is conjugate to $z\mapsto\mu z$, where $\mu$ has multiplicative order exactly $n$. For $n>1$, zero and infinity each form a singleton orbit. At a finite nonzero $z$, an iterate returns precisely when $\mu^kz=z$, equivalently $\mu^k=1$; the least positive return time is $n$. Conjugacy preserves orbit sizes. Hence the [finite-order Möbius orbit sizes](../../../group-theory.md#finite-order-mobius-orbit-sizes) are

$$
\boxed{1\text{ and }n\quad(n>1),\qquad\text{only }1\quad(n=1).}
$$

For $n>1$ exactly two points have size-one orbits; every other point has orbit size $n$.

## 9A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9a/i">i</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/i/solution">Solution</h4>

↑ **Parent:** [I](#9a/i)

A [conservative vector field](../../../calculus.md#conservative-vector-field) is the [gradient](../../../calculus.md#gradient) of a single-valued differentiable scalar potential. Its [line integral](../../../calculus.md#line-integral) is path independent and equals the potential difference. If $\psi\mathbf A=\nabla F$ with a twice continuously differentiable potential, equality of mixed partial derivatives gives

$$
\partial_y(\psi A_1)=\partial_y\partial_xF=\partial_x\partial_yF=\partial_x(\psi A_2).
$$

The [product rule](../../../calculus.md#product-rule) then gives $\psi_yA_1+\psi A_{1,y}=\psi_xA_2+\psi A_{2,x}$. Rearranging proves the [integrating-factor equation for a planar vector field](../../../calculus.md#integrating-factor-equation-for-a-planar-vector-field):

$$
\boxed{\psi(A_{1,y}-A_{2,x})=A_2\psi_x-A_1\psi_y.}
$$

This argument does not require division by $\psi$, so it remains valid even at its zeros. A nonvanishing [integrating factor](../../../differential-equation.md#integrating-factor) is normally sought when one wants to recover useful potential curves for the original field.

<h3 id="9a/ii">ii</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9a/ii)

Assume $P,Q$ are continuously differentiable on a neighbourhood of a bounded region with a positively oriented piecewise smooth simple boundary. To prove [Green theorem](../../../calculus.md#green-theorem), first take a region between the graphs $y=f(x)$ and $y=g(x)$, $a\le x\le b$, with $f\le g$. Counterclockwise orientation traverses the lower graph to the right and the upper graph to the left; vertical end pieces contribute nothing to $P\,dx$. Thus the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives

$$
\oint_{\partial R}P\,dx=\int_a^b[P(x,f(x))-P(x,g(x))]dx=-\int_a^b\int_{f(x)}^{g(x)}P_y\,dy\,dx.
$$

Likewise, for a region between graphs $x=u(y)$ and $x=v(y)$, the right boundary is traversed upwards and the left one downwards. Horizontal end pieces contribute nothing to $Q\,dy$, so

$$
\oint_{\partial R}Q\,dy=\int_c^d[Q(v(y),y)-Q(u(y),y)]dy=\int_c^d\int_{u(y)}^{v(y)}Q_x\,dx\,dy.
$$

For a polygonal region, triangulate its interior. Each triangle is of both graph types with piecewise linear bounds, so adding the formulae gives the result: the double integrals add and the integrals on internal edges cancel because the adjacent triangles traverse them in opposite directions. For a regular piecewise smooth simple boundary, choose inscribed simple polygonal approximations to its piecewise smooth parametrization. Their line integrals converge to the original [line integral](../../../calculus.md#line-integral), since the parametrizations converge uniformly and their piecewise constant tangent vectors converge in the integral norm on each smooth arc. Their regions converge in area: the symmetric difference lies in a shrinking neighbourhood of the original boundary, which has planar measure zero. Boundedness of the continuous integrand then gives convergence of the area integrals. Passing to the limit proves the formula for the stated boundary class. Combining the two identities gives

$$
\boxed{\oint_{\partial R}(P\,dx+Q\,dy)=\iint_R(Q_x-P_y)\,dx\,dy.}
$$

Positive orientation is essential for the sign.

Choose $P=-y/2$ and $Q=x/2$, for which $Q_x-P_y=1$. The [boundary formula for planar area](../../../calculus.md#boundary-formula-for-planar-area) is

$$
\boxed{\operatorname{area}(R)=\frac12\oint_{\partial R}(x\,dy-y\,dx).}
$$

For the [ellipse](../../../geometry-and-topology.md#ellipse), take $a,b>0$ so the given increasing-angle parametrization is counterclockwise. Then $dx=-a\sin\theta\,d\theta$ and $dy=b\cos\theta\,d\theta$, so

$$
\operatorname{area}(R)=\frac12\int_0^{2\pi}ab(\cos^2\theta+\sin^2\theta)d\theta=\boxed{\pi ab}.
$$

If signed nonzero parameters are allowed, the unsigned area is $\pi|ab|$, with orientation corrected accordingly.

## 10A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10a/solution">Solution</h3>

↑ **Parent:** [10A](#10a)

The [divergence of a cross product](../../../calculus.md#divergence-of-a-cross-product) identity and the stated static field equations give

$$
\nabla\cdot(\mathbf E\times\mathbf B)=\mathbf B\cdot(\nabla\times\mathbf E)-\mathbf E\cdot(\nabla\times\mathbf B)=-\mathbf E\cdot\mathbf J.
$$

For an outward-oriented closed surface, the [divergence theorem](../../../calculus.md#divergence-theorem) therefore gives the flux of the specified [Poynting vector](../../../electromagnetism.md#poynting-vector) normalization:

$$
\boxed{\iint_{\partial V}\mathbf P\cdot d\mathbf S=-\iiint_V\mathbf E\cdot\mathbf J\,dV.}
$$

No open-surface conclusion follows from this equation without including its closing pieces.

For the particular fields, direct calculation gives

$$
\mathbf J=\nabla\times\mathbf B=(0,-z,-y),\qquad\mathbf P=\mathbf E\times\mathbf B=(x^2y,-xz^2,-xyz),\qquad\nabla\cdot\mathbf P=xy.
$$

The fields also have $\nabla\times\mathbf E=0$, $\nabla\cdot\mathbf B=0$, and $\nabla\cdot\mathbf J=0$, consistently with the required equations. Close the outward spherical patch by the two planar half-disks on $x=0$ and $y=0$, forming the quarter unit ball $V$. Its total closed flux is

$$
\iiint_Vxy\,dV=\int_0^{\pi/2}\cos\varphi\sin\varphi\,d\varphi\int_0^1r^3dr\int_{-\sqrt{1-r^2}}^{\sqrt{1-r^2}}dz=\int_0^1r^3\sqrt{1-r^2}\,dr=\frac{2}{15},
$$

where $r$ in this integral is cylindrical radius. The $x=0$ face has outward normal $-\mathbf e_x$ and zero flux because $P_x=0$ there. The $y=0$ face has outward normal $-\mathbf e_y$, so its flux is

$$
\int_{-1}^1\int_0^{\sqrt{1-z^2}}xz^2\,dx\,dz=\frac12\int_{-1}^1z^2(1-z^2)dz=\frac{2}{15}.
$$

Subtracting these planar contributions from the closed flux gives the requested open-patch answer

$$
\boxed{\iint_{\text{spherical patch}}\mathbf P\cdot d\mathbf S=0.}
$$

As a direct check, on the unit sphere the outward normal is $(x,y,z)$ and $\mathbf P\cdot\mathbf n=xy(x^2-2z^2)$. With spherical angles $0\le\vartheta\le\pi$, $0\le\varphi\le\pi/2$, its [surface integral](../../../calculus.md#surface-integral) is $\frac14\int_0^\pi\sin^5\vartheta\,d\vartheta-\int_0^\pi\sin^3\vartheta\cos^2\vartheta\,d\vartheta=\frac14(16/15)-4/15=0$. The curved patch's vanishing flux is a cancellation, not an inference that its flux density vanishes everywhere.

## 11A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11a/solution">Solution</h3>

↑ **Parent:** [11A](#11a)

For a real-valued function on a bounded regular region, apply the [divergence theorem](../../../calculus.md#divergence-theorem) to $\phi\nabla\phi$. The [product rule](../../../calculus.md#product-rule) yields $\nabla\cdot(\phi\nabla\phi)=|\nabla\phi|^2+\phi\nabla^2\phi$. The prescribed zero boundary values and [Laplace equation](../../../partial-differential-equation.md#laplace-equation) therefore imply

$$
\int_V|\nabla\phi|^2dV=\int_{\partial V}\phi\,\partial_n\phi\,dS-\int_V\phi\nabla^2\phi\,dV=0.
$$

The continuous nonnegative integrand must vanish everywhere. Hence $\phi$ is constant on each connected component, and its boundary value makes each constant zero. This proves [zero-boundary harmonic uniqueness](../../../analysis.md#zero-boundary-harmonic-uniqueness). If complex-valued functions are allowed, apply the same argument separately to their real and imaginary parts. If $\psi_1,\psi_2$ solve the same [Poisson equation](../../../partial-differential-equation.md#poisson-equation) and [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data), their difference is harmonic with zero boundary value, so is zero. Thus **there is at most one solution**. An exterior unbounded region would require an additional condition at infinity; the preceding bounded-domain proof does not assert uniqueness without one.

For the radial calculation use Cartesian coordinates with $r=(x_ix_i)^{1/2}>0$. The [chain rule](../../../calculus.md#chain-rule) gives $\partial_ir=x_i/r$ and

$$
\boxed{\nabla\psi=\frac{\psi'(r)}r\mathbf x.}
$$

Differentiate again and sum the three coordinates:

$$
\begin{aligned}
\nabla^2\psi&=\partial_i\left(\psi'(r)\frac{x_i}r\right)\\
&=\psi''(r)\frac{x_ix_i}{r^2}+\psi'(r)\left(\frac3r-\frac{x_ix_i}{r^3}\right)\\
&=\psi''(r)+\frac2r\psi'(r)=\boxed{\frac1r\frac{d^2(r\psi)}{dr^2}}.
\end{aligned}
$$

This derives the [radial Laplacian](../../../partial-differential-equation.md#radial-laplacian) directly in Cartesian coordinates. For $\nabla^2\psi=c$, set $u=r\psi$, so $u''=cr$. Integrating twice gives $u=cr^3/6+ar+b$, and consequently

$$
\boxed{\psi(r)=\frac{cr^2}{6}+a+\frac br,\qquad r>0.}
$$

If the solution must extend boundedly through the origin, $b=0$. The remaining polynomial is smooth there.

<h3 id="11a/i">i</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/i/solution">Solution</h4>

↑ **Parent:** [I](#11a/i)

The radial [Laplace equation](../../../partial-differential-equation.md#laplace-equation) has solution $a+b/r$. Boundedness at the origin requires $b=0$, and the value at $r=1$ fixes $a=1$. Thus

$$
\boxed{\psi(r)=1,\qquad0\le r\le1.}
$$

<h3 id="11a/ii">ii</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11a/ii)

The radial [Poisson equation](../../../partial-differential-equation.md#poisson-equation) with constant source one has $\psi=r^2/6+a+b/r$. The boundary conditions give

$$
\frac16+a+b=1,\qquad\frac46+a+\frac b2=1.
$$

Subtracting gives $b=1$, then $a=-1/6$. Hence

$$
\boxed{\psi(r)=\frac{r^2-1}{6}+\frac1r,\qquad1\le r\le2.}
$$

Its [radial Laplacian](../../../partial-differential-equation.md#radial-laplacian) is one and both endpoint values are one. The prescribed values ensure continuity with the adjacent region solutions, but do not impose derivative continuity.

<h3 id="11a/iii">iii</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11a/iii)

The exterior radial [Laplace equation](../../../partial-differential-equation.md#laplace-equation) has $\psi=a+b/r$. Decay at infinity forces $a=0$ and the value at $r=2$ forces $b=2$. Therefore

$$
\boxed{\psi(r)=\frac2r,\qquad r\ge2.}
$$

Together the three solutions satisfy their separate regional equations and specified boundary values. Their radial derivatives jump at the interfaces, so they should not be asserted to solve one globally smooth [Poisson equation](../../../partial-differential-equation.md#poisson-equation) with only the listed volume sources and no interface terms.

## 12A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

For a [Cartesian second-rank tensor](../../../linear-algebra.md#cartesian-second-rank-tensor), write

$$
P_{ij}=\frac12(P_{ij}+P_{ji})+\frac12(P_{ij}-P_{ji}).
$$

The first term is a [symmetric second-rank tensor](../../../linear-algebra.md#symmetric-second-rank-tensor) and the second is an [antisymmetric second-rank tensor](../../../linear-algebra.md#antisymmetric-second-rank-tensor). Taking the [trace](../../../linear-algebra.md#matrix-trace) of the symmetric term and subtracting it gives the [scalar, symmetric-traceless and axial tensor decomposition](../../../linear-algebra.md#scalar-symmetric-traceless-and-axial-tensor-decomposition):

$$
\boxed{P=\frac13P_{kk},\qquad S_{ij}=\frac12(P_{ij}+P_{ji})-\frac13P_{kk}\delta_{ij},\qquad A_k=\frac12\epsilon_{kij}P_{ij}.}
$$

Here $S_{ij}=S_{ji}$ and $S_{ii}=0$. To check reconstruction of the antisymmetric part, contract the [Levi-Civita symbols](../../../calculus.md#levi-civita-symbol):

$$
\epsilon_{ijk}A_k=\frac12\epsilon_{ijk}\epsilon_{klm}P_{lm}=\frac12(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})P_{lm}=\frac12(P_{ij}-P_{ji}).
$$

Thus $P_{ij}=P\delta_{ij}+S_{ij}+\epsilon_{ijk}A_k$, and the displayed contractions also prove uniqueness. The vector associated with the antisymmetric part is an [axial vector](../../../vector-space.md#pseudovector) under reflections, and an ordinary vector under proper rotations.

For the specified [isotropic tensor](../../../linear-algebra.md#isotropic-tensor) law, contract the [Kronecker deltas](../../../linear-algebra.md#kronecker-delta) first:

$$
P_{ij}=\alpha\delta_{ij}T_{kk}+\beta T_{ij}+\gamma T_{ji}.
$$

Write $T_{ij}=T\delta_{ij}+W_{ij}+\epsilon_{ijk}V_k$, where $T=T_{kk}/3$ and $W$ is symmetric and traceless. Transposition preserves its scalar and symmetric-traceless parts and reverses its antisymmetric part. Therefore

$$
P_{ij}=(3\alpha+\beta+\gamma)T\delta_{ij}+(\beta+\gamma)W_{ij}+(\beta-\gamma)\epsilon_{ijk}V_k.
$$

Uniqueness of the decomposition gives the [isotropic elasticity on tensor components](../../../linear-algebra.md#isotropic-elasticity-on-tensor-components) relations. Provided their respective coefficients are nonzero, the requested inverses are

$$
\boxed{T=\frac{P}{3\alpha+\beta+\gamma},\qquad W_{ij}=\frac{S_{ij}}{\beta+\gamma},\qquad V_k=\frac{A_k}{\beta-\gamma}.}
$$

If one coefficient vanishes, that strain component has zero stress response: the corresponding stress component must be zero for a solution to exist, and that strain component is not uniquely recoverable. Isotropy by itself does not guarantee invertibility.

If $T_{ij}$ is symmetric then $V=0$, hence $A=0$ and the stress is symmetric. Equivalently, direct transposition gives $P_{ij}-P_{ji}=(\beta-\gamma)(T_{ij}-T_{ji})=0$. Restricting to this symmetric-strain case gives

$$
\boxed{P_{ij}=\lambda\delta_{ij}T_{kk}+\mu T_{ij},\qquad\lambda=\alpha,\quad\mu=\beta+\gamma.}
$$

This final two-parameter expression uses the symmetry assumption from the preceding request. For a general nonsymmetric array, the transpose term cannot be absorbed into the same coefficient: it acts with $\beta+\gamma$ on the symmetric-traceless part and with $\beta-\gamma$ on the antisymmetric part. The stated coefficient $\mu$ is the coefficient of $T_{ij}$ itself; if one instead writes the conventional elastic law with $2\mu$ multiplying the strain, that shear-modulus convention is half this coefficient.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
