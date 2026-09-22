# Paper 126

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_126.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_126.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 126](paper-126.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $X=V/\Gamma$ be a [complex torus](../../../complex-geometry.md#complex-torus). A [Riemann form on a complex torus](../../../complex-geometry.md#riemann-form-on-a-complex-torus) is a [Hermitian form](../../../linear-algebra.md#hermitian-form) $H$ on $V$ whose imaginary part

$$
E(v,w)=\operatorname{Im}H(v,w)
$$

takes integer values on $\Gamma\times\Gamma$. Equivalently, $E$ is an integral alternating form satisfying

$$
E(iv,iw)=E(v,w),
\qquad E(iv,v)>0
$$

for every nonzero $v$. A [polarisation of a complex torus](../../../complex-geometry.md#polarization-of-a-complex-torus) is such a positive Riemann form, or equivalently its integral cohomology class. By the [Appell–Humbert theorem](../../../complex-geometry.md#appell-humbert-theorem), it is the first Chern class of an ample holomorphic line bundle. A polarisation is principal when the homomorphism $\Gamma\to\Gamma^*$ induced by $E$ is an isomorphism.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The rank assumption says that $\Gamma'=\Gamma\cap V'$ is a full lattice in the real vector space underlying $V'$. Thus $X'=V'/\Gamma'$ is compact, and the inclusion $V'\hookrightarrow V$ descends to an injective holomorphic homomorphism $X'\hookrightarrow X$. It is therefore a [complex subtorus](../../../complex-geometry.md#complex-subtorus).

Conversely, let $j:Y\hookrightarrow X$ be a subtorus. Its differential at the identity identifies the universal cover of $Y$ with a complex subspace $V'\subseteq V$. Lifting $j$ to universal covers shows that the period lattice of $Y$ is precisely $V'\cap\Gamma$. Compactness of $Y$ makes this a full lattice of rank $2\dim_{\mathbb C}V'$, so every subtorus has the stated form.

Now let $H$ be a polarisation on $X$. Its restriction to $V'$ is still positive definite, and its imaginary part remains integral on $\Gamma'$, so it polarises $X'$. Define the Hermitian orthogonal complement

$$
V''=(V')^{\perp_H}.
$$

Because $V'$ is spanned over $\mathbb R$ by lattice vectors and $E=\operatorname{Im}H$ is integral on $\Gamma$, the real equations $E(v,\gamma')=0$ for $\gamma'\in\Gamma'$ make $V''$ rational with respect to $\Gamma$. Hence $\Gamma''=V''\cap\Gamma$ is a full lattice in $V''$, and $X''=V''/\Gamma''$ is a subtorus. Since $V=V'\oplus V''$, the lattice $\Gamma'+\Gamma''$ has finite index in $\Gamma$. Consequently the addition map

$$
X'\times X''\longrightarrow X
$$

is an [isogeny of complex tori](../../../complex-geometry.md#isogeny-of-complex-tori): it is surjective and has finite kernel. Therefore $X=X'+X''$ and $X'\cap X''$ is finite.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Write a lattice vector as

$$
u=(a+ci+d\sqrt2,\ b+di\sqrt3),
\qquad a,b,c,d\in\mathbb Z.
$$

A one-dimensional subtorus would give two $\mathbb Z$-independent lattice vectors $u,u'$ spanning one complex line, so their determinant would vanish. Separating the real and imaginary parts and using the $\mathbb Q$-linear independence of $1,\sqrt2,\sqrt3$ gives

$$
ab'-a'b=0,quad db'-d'b=0,quad c'd-cd'=0,quad cb'-c'b=0,quad ad'-a'd=0.
$$

If either $b$ or $b'$ is nonzero, these relations make $(a,b,c,d)$ and $(a',b',c',d')$ rationally proportional, contradicting their lattice independence. Thus $b=b'=0$. If either $d$ or $d'$ is nonzero, the last two relevant relations again make all four coordinates proportional. Hence $d=d'=0$, and both vectors lie in $\mathbb C(1,0)$. Conversely, $(1,0)$ and $(i,0)$ lie in $\Gamma$, so

$$
X'=mathbb C(1,0)/(\mathbb Z+i\mathbb Z)(1,0)
$$

is a one-dimensional subtorus. It is the unique one.

If $X$ admitted a polarisation, part (ii) would give a one-dimensional complementary subtorus $X''$ with $X=X'+X''$. Uniqueness would force $X''=X'$, making $X'+X''=X'\ne X$, a contradiction. Thus $X$ is a nonprojective complex torus and has no polarisation.

## 2

↑ **Parent:** [Paper 126](paper-126.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [group scheme](../../../ringed-space.md#group-scheme) over $k$ is a $k$-scheme $G$ equipped with multiplication $m:G\times_kG\to G$, identity $e:\operatorname{Spec}k\to G$, and inversion $j:G\to G$ satisfying the associativity, identity, and inverse diagrams.

Consider

$$
q:G\times_kG\longrightarrow G,
\qquad q(x,y)=xy^{-1}.
$$

The [diagonal morphism](../../../ringed-space.md#diagonal-morphism) is $\Delta_{G/k}=q^{-1}(e)$. For a finite-type $k$-scheme the rational identity point is closed, so its inverse image is closed. Thus the diagonal is a closed immersion and every such group scheme over a field is a [separated scheme](../../../ringed-space.md#separated-scheme).

In characteristic $p>0$, the infinitesimal additive group

$$
\alpha_p=\operatorname{Spec}k[t]/(t^p)
$$

is a nonreduced group scheme. Its comultiplication is $t\mapsto t\otimes1+1\otimes t$, which is well defined because $(t\otimes1+1\otimes t)^p=t^p\otimes1+1\otimes t^p$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [Mumford rigidity lemma](../../../abelian-variety.md#mumford-rigidity-lemma) says that if $A$ is complete, $B$ is connected, and a morphism $F:A\times B\to Z$ maps the fiber over some $b_0\in B$ to a point, then $F$ is constant on every $A$-fiber and factors through $B$.

Put $y=f(e_X)$ and normalize

$$
g=T_{-y}\circ f,
$$

so $g(e_X)=e_G$. Define

$$
F:X\times X\longrightarrow G,
\qquad F(x,z)=g(x+z)g(z)^{-1}.
$$

When the first coordinate is $e_X$, this is constantly $e_G$. Apply rigidity with the second copy of the complete variety $X$ as the complete factor. It follows that $F(x,z)$ is independent of $z$, and evaluation at $z=e_X$ gives $F(x,z)=g(x)$. Therefore

$$
g(x+z)=g(x)g(z),
$$

so $g$ is a [homomorphism of group varieties](../../../algebraic-geometry.md#homomorphism-of-group-varieties) and $f=T_y\circ g$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Completeness is essential. Take $X=G=\mathbb G_a$. In characteristic different from two, the morphism $f(t)=t^2$ satisfies $f(0)=0$ but is not additive. If it were $T_y\circ g$ with $g$ a group homomorphism, evaluation at zero would give $y=0$ and hence $f=g$, a contradiction. In characteristic two the same argument works with $f(t)=t^3$.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

For an [abelian variety](../../../abelian-variety.md) $X$, consider the commutator morphism

$$
c:X\times X\longrightarrow X,
\qquad c(x,y)=xyx^{-1}y^{-1}.
$$

It is the identity whenever either coordinate is the identity. The [Mumford rigidity lemma](../../../abelian-variety.md#mumford-rigidity-lemma) applied successively to the two complete connected factors makes $c$ constant everywhere; its value at $(e,e)$ is $e$. Therefore every pair of points commutes, so the group law is commutative.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

Because $p:X_1\times X_2\to X$ is an isomorphism and $X$ is connected, each $X_i$ is connected. They are complete because they are closed in the complete variety $X$. Let

$$
q_i=\operatorname{pr}_i\circ p^{-1}:X\longrightarrow X_i
$$

be the two component morphisms.

For $x,x'\in X_1$, the morphism

$$
(x,x')\longmapsto q_2(x+x')
$$

from $X_1\times X_1$ to $X_2$ is constantly $e$ on either coordinate axis. Rigidity therefore makes it constantly $e$, so $X_1$ is closed under addition. The same argument applies to $X_2$. If $-x=u+v$ is the unique decomposition with $u\in X_1$ and $v\in X_2$, then $e=(x+u)+v$; uniqueness of the decomposition of $e$ gives $v=e$ and $u=-x$. Thus each $X_i$ is also closed under inversion.

The restrictions of the multiplication and inversion morphisms of $X$ now make each $X_i$ a complete connected group variety, hence an abelian variety. Since the group law on $X$ is commutative,

$$
p((x_1,x_2)+(y_1,y_2))
=x_1+y_1+x_2+y_2
=p(x_1,x_2)+p(y_1,y_2).
$$

**Thus $p$ is a homomorphism. It is already an isomorphism of varieties, and its inverse consequently respects the group operations as well, so $p$ is an isomorphism of group schemes.**

## 3

↑ **Parent:** [Paper 126](paper-126.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $m_I:X^3\to X$ add the coordinates indexed by a nonempty subset $I$ of the three-element index set. The [Theorem of the Cube](../../../abelian-variety.md#theorem-of-the-cube) says that for every line bundle $\mathcal L$ on an abelian variety,

$$
m_{123}^*\mathcal L
\otimes m_{12}^*\mathcal L^\vee
\otimes m_{13}^*\mathcal L^\vee
\otimes m_{23}^*\mathcal L^\vee
\otimes m_1^*\mathcal L
\otimes m_2^*\mathcal L
\otimes m_3^*\mathcal L
$$

is trivial, up to the harmless constant line given by the fiber of $\mathcal L$ at the identity.

Pull this line bundle back along $(f,g,h):Y\to X^3$. Pullback commutes with tensor products and duals, and $m_I\circ(f,g,h)$ is the corresponding sum of morphisms. The resulting bundle is precisely $\mathcal M_{f,g,h}$, so it is trivial.

Take $Y=X$, $f=\operatorname{id}_X$, and let $g,h$ be the constant maps with values $x,y$. All pullbacks along constant maps are trivial line bundles. The formula for $\mathcal M_{f,g,h}$ then becomes

$$
T_{x+y}^*\mathcal L\otimes
(T_x^*\mathcal L)^\vee\otimes
(T_y^*\mathcal L)^\vee\otimes\mathcal L
\simeq\mathcal O_X,
$$

or equivalently

$$
T_{x+y}^*\mathcal L
\simeq T_x^*\mathcal L\otimes T_y^*\mathcal L\otimes\mathcal L^\vee.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For a line bundle $\mathcal L$ on $X$, define the [homomorphism associated to a line bundle on an abelian variety](../../../abelian-variety.md#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety)

$$
\phi_{\mathcal L}:X(k)\longrightarrow\operatorname{Pic}X,
\qquad
x\longmapsto T_x^*\mathcal L\otimes\mathcal L^\vee.
$$

The translation identity from part (i) gives

$$
\phi_{\mathcal L}(x+y)
\simeq\phi_{\mathcal L}(x)\otimes\phi_{\mathcal L}(y),
$$

so $\phi_{\mathcal L}$ is a homomorphism.

Suppose $\mathcal M\simeq T_y^*\mathcal L\otimes\mathcal L^\vee$ lies in its image. Then

$$
\phi_{\mathcal M}(x)
\simeq
T_{x+y}^*\mathcal L\otimes
(T_x^*\mathcal L)^\vee\otimes
(T_y^*\mathcal L)^\vee\otimes\mathcal L,
$$

which is trivial by the same translation identity. Hence $\phi_{\mathcal M}=0$; the image of every $\phi_{\mathcal L}$ lies in the [Identity component of the Picard group](../../../abelian-variety.md#identity-component-of-the-picard-group) $\operatorname{Pic}^0X$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Directly from the definition,

$$
\phi_{\mathcal L\otimes\mathcal L'}(x)
=\phi_{\mathcal L}(x)\otimes\phi_{\mathcal L'}(x),
\qquad
\phi_{\mathcal L^\vee}(x)=\phi_{\mathcal L}(x)^{-1}.
$$

Also

$$
\phi_{T_x^*\mathcal L}(y)
=T_x^*\bigl(T_y^*\mathcal L\otimes\mathcal L^\vee\bigr).
$$

The bundle in parentheses lies in $\operatorname{Pic}^0X$ by part (ii), so it is translation invariant. This proves $\phi_{T_x^*\mathcal L}=\phi_{\mathcal L}$.

Finally, $[n]\circ T_x=T_{nx}\circ[n]$, and therefore

$$
\phi_{[n]^*\mathcal L}(x)
=[n]^*\bigl(T_{nx}^*\mathcal L\otimes\mathcal L^\vee\bigr)
=[n]^*\phi_{\mathcal L}(nx).
$$

For $\mathcal N\in\operatorname{Pic}^0X$, the multiplication pullback formula reduces to $[n]^*\mathcal N\simeq\mathcal N^{\otimes n}$. Consequently

$$
\phi_{[n]^*\mathcal L}(x)=\phi_{\mathcal L}(nx)^n,
$$

as required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
