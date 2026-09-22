# Paper 118

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_118.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_118.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [complex structure](../../../complex-geometry.md#complex-structure) splits the complexified [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle) into its $(1,0)$ and $(0,1)$ parts. Thus the space of smooth [differential forms of type (p, q)](../../../complex-geometry.md#differential-form-of-type-p-q) is

$$
\boxed{\mathcal A^{p,q}(M)=\Gamma\left(M,\bigwedge^p(T^{1,0}M)^*\otimes\bigwedge^q(T^{0,1}M)^*\right).}
$$

Here $\Gamma$ denotes smooth [sections of a vector bundle](../../../fiber-bundle.md#section-of-a-vector-bundle); exterior multiplication identifies the displayed bundle with a subbundle of the complexified exterior algebra. In [holomorphic coordinates](../../../complex-geometry.md#holomorphic-coordinate), such a [differential form of type (p, q)](../../../complex-geometry.md#differential-form-of-type-p-q) has the expression

$$
\alpha=\sum_{|I|=p,\,|J|=q}a_{IJ}(z,\bar z)\,dz_I\wedge d\bar z_J,
$$

where the coefficients are smooth and both multi-indices are increasing. Negative bidegrees, or bidegrees exceeding the complex dimension, give the zero space.

On a [complex manifold](../../../complex-geometry.md#complex-manifold), the [exterior derivative](../../../differential-form.md#exterior-derivative) has just two type components, $d=\partial+\bar\partial$. The [conjugate Dolbeault operator](../../../complex-geometry.md#conjugate-dolbeault-operator) and the [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator) are, respectively,

$$
\partial\alpha=\sum_{I,J,k}\frac{\partial a_{IJ}}{\partial z_k}\,dz_k\wedge dz_I\wedge d\bar z_J,
\qquad
\bar\partial\alpha=\sum_{I,J,k}\frac{\partial a_{IJ}}{\partial\bar z_k}\,d\bar z_k\wedge dz_I\wedge d\bar z_J.
$$

Keeping the differentiating factor at the front fixes the signs. These definitions are intrinsic because holomorphic coordinate changes preserve type. **The two operators are the type projections of the exterior derivative**, raising $p$ and $q$, respectively.

For a [holomorphic map](../../../complex-analysis.md#holomorphic-map) $f:M\to N$, its differential is a [complex-linear map](../../../vector-space.md#complex-linear-map), so the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) sends $(1,0)$ covectors to $(1,0)$ covectors and $(0,1)$ covectors to $(0,1)$ covectors. In coordinates $w$ on $N$,

$$
f^*dw_a=\sum_j\frac{\partial f_a}{\partial z_j}dz_j,
\qquad f^*d\bar w_a=\sum_j\overline{\frac{\partial f_a}{\partial z_j}}d\bar z_j.
$$

The [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) commutes with the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms), so it preserves the counts of these factors. Consequently

$$
\boxed{f^*:\mathcal A^{p,q}(N)\longrightarrow\mathcal A^{p,q}(M).}
$$

It also commutes separately with the [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator) and the [conjugate Dolbeault operator](../../../complex-geometry.md#conjugate-dolbeault-operator), because it commutes with $d$ and preserves type.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

**The assertion requires $p+q>0$.** As printed, it also includes $(p,q)=(0,0)$, where the nonzero constant function $1$ is closed but cannot be the [exterior derivative](../../../differential-form.md#exterior-derivative) of a negative-degree form. The zero constant is harmless; below we prove the intended positive-degree result.

Set $k=p+q>0$, let $\rho_t(z)=tz$, and let

$$
R=\sum_j\left(z_j\frac{\partial}{\partial z_j}+\bar z_j\frac{\partial}{\partial\bar z_j}\right).
$$

The [polydisc](../../../complex-geometry.md#polydisc) is preserved by these dilations. The [radial homotopy operator](../../../differential-form.md#radial-homotopy-operator) is

$$
\boxed{H\alpha=\int_0^1\rho_t^*(\iota_R\alpha)\,\frac{dt}{t}.}
$$

Here $\iota_R$ is the [interior product of a differential form](../../../differential-form.md#interior-product). For a smooth $k$-form, its pulled-back contraction is $O(t^k)$, so the integral and its coefficient derivatives converge at zero. The identity for a [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) along the radial flow and [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) give

$$
\frac{d}{dt}\rho_t^*\alpha=\frac1t\rho_t^*\mathcal L_R\alpha
=\frac1t\rho_t^*(d\iota_R\alpha+\iota_Rd\alpha).
$$

Integrating yields $dH\alpha+Hd\alpha=\alpha-\rho_0^*\alpha$. The final pullback vanishes in positive degree; since $d\alpha=0$, we have $dH\alpha=\alpha$.

Each $\rho_t$ is a [holomorphic map](../../../complex-analysis.md#holomorphic-map), so its [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) preserves bidegree. Contracting with the $(1,0)$ part of $R$ lowers $p$ by one, and contracting with its $(0,1)$ part lowers $q$ by one. Therefore the primitive has precisely the permitted types:

$$
\boxed{\beta=H\alpha\in\mathcal A^{p-1,q}(D)\oplus\mathcal A^{p,q-1}(D),\qquad d\beta=\alpha.}
$$

This is a type-preserving refinement of the [Poincaré lemma](../../../differential-form.md#poincare-lemma); when one index is zero, the corresponding negative-degree summand is simply absent.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use a radial [geometric Kähler potential](../../../complex-geometry.md#kahler-potential-complex-geometry). Write $s=|z_1|^2+|z_2|^2$ and $y(s)=\varphi'(s)$. The coefficient [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) of $i\partial\bar\partial\varphi(s)$ is

$$
G_{j\bar k}=y\delta_{jk}+y'\bar z_jz_k.
$$

Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $y$ in the complex tangential direction and $y+sy'$ in the complex radial direction. A [Kähler metric](../../../complex-geometry.md#kahler-metric) is positive precisely when both are positive. The standard form has coefficient [matrix](../../../vector-space.md#matrix) $\frac12 I$, so equality of the [Riemannian volume forms](../../../differential-geometry.md#riemannian-volume-form) is the condition

$$
y(y+sy')=\frac14.
$$

Indeed, the volume form is $\omega^2/2$ and its coefficient is proportional to $\det G$. Multiplying the determinant equation by $2s$ gives $(s^2y^2)'=s/2$, so we can take

$$
y(s)=\frac{\sqrt{s^2+a^2}}{2s}\qquad(a>0).
$$

An explicit antiderivative is

$$
\boxed{\varphi_a(s)=\frac12\left[\sqrt{s^2+a^2}+a\log\frac{s}{\sqrt{s^2+a^2}+a}\right],\qquad
\omega'=i\partial\bar\partial\varphi_a(s).}
$$

It is smooth for $s>0$. Its two [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are

$$
\lambda_{\mathrm{tan}}=\frac{\sqrt{s^2+a^2}}{2s}>0,
\qquad
\lambda_{\mathrm{rad}}=\frac{s}{2\sqrt{s^2+a^2}}>0,
\qquad \lambda_{\mathrm{tan}}\lambda_{\mathrm{rad}}=\frac14.
$$

The form is real and closed because it is $i\partial\bar\partial$ of a real function, so it is a [Kähler metric](../../../complex-geometry.md#kahler-metric) on the punctured space. Since $a>0$, neither [eigenvalue](../../../linear-operator-theory.md#eigenvalue) equals $1/2$, and the metric differs from the Euclidean one. **The radial and tangential stretches compensate exactly, preserving the volume form:**

$$
\boxed{\frac{(\omega')^2}{2}=\frac{\omega^2}{2},\qquad \omega'\ne\omega.}
$$

This is a [radial Kähler metric with Euclidean volume in complex dimension two](../../../complex-geometry.md#radial-kahler-metric-with-euclidean-volume-in-complex-dimension-two).

<a id="1/c/image-radial-and-tangential-metric-eigenvalues-relative-to-the-euclidean-metric-with-unchanged-volume"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-118-radial-metric.png)

**[Figure 1](#1/c/image-radial-and-tangential-metric-eigenvalues-relative-to-the-euclidean-metric-with-unchanged-volume). Radial and tangential metric eigenvalues relative to the Euclidean metric, with unchanged volume**.

## 2

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For the nonnegative [Hodge Laplacian](../../../differential-form.md#hodge-laplacian) $\Delta_d^{\mathrm H}=dd^*+d^*d$, the [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity) gives $\Delta_d^{\mathrm H}=2\Delta_{\bar\partial}$. If $u$ is a [holomorphic function](../../../complex-analysis.md#holomorphic-function), then $\bar\partial u=0$, while $\bar\partial^*u=0$ by degree. Therefore

$$
\Delta_{\bar\partial}u=(\bar\partial\bar\partial^*+\bar\partial^*\bar\partial)u=0,
\qquad \Delta_d^{\mathrm H}u=0.
$$

The divergence-of-gradient convention printed in part (b) is $\Delta_d=-\Delta_d^{\mathrm H}$ on functions. The sign changes no kernel, so the requested [harmonicity of holomorphic functions on a Kähler manifold](../../../complex-geometry.md#harmonicity-of-holomorphic-functions-on-a-kahler-manifold) is

$$
\boxed{\Delta_du=0.}
$$

**Holomorphic functions are harmonic without any compactness assumption.** This is a local identity from the [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity), not an integration argument requiring a compact manifold.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The real coordinate functions are real and imaginary parts of the [holomorphic coordinates](../../../complex-geometry.md#holomorphic-coordinate) $z_j$. Part (a), together with the real coefficients of the [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator), therefore shows that every $x_l$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function). For the given divergence-of-gradient convention, applying the operator to $x_l$ gives

$$
0=\Delta_dx_l=\frac1{\sqrt{\det g}}\sum_{k=1}^{2n}\frac{\partial}{\partial x_k}\left(\sqrt{\det g}\,g^{kl}\right).
$$

These are the [harmonic coordinate](../../../numerical-relativity.md#harmonic-coordinate) identities. Expanding the operator on an arbitrary smooth function now gives

$$
\Delta_du=\sum_{k,l=1}^{2n}g^{kl}\frac{\partial^2u}{\partial x_k\partial x_l}
+\sum_{l=1}^{2n}\left[\frac1{\sqrt{\det g}}\sum_{k=1}^{2n}\frac{\partial}{\partial x_k}\left(\sqrt{\det g}\,g^{kl}\right)\right]\frac{\partial u}{\partial x_l}.
$$

The bracketed coefficients vanish. Hence **there is no first-derivative term in these coordinates**:

$$
\boxed{\Delta_du=\sum_{k,l=1}^{2n}g^{kl}\frac{\partial^2u}{\partial x_k\partial x_l}.}
$$

The reason is that the real components of [holomorphic coordinates](../../../complex-geometry.md#holomorphic-coordinate) are [harmonic coordinates](../../../numerical-relativity.md#harmonic-coordinate) for a [Kähler metric](../../../complex-geometry.md#kahler-metric); a general real coordinate change need not retain this simplification.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $\pi_i:\mathbb C^{g_i}\to X_i$ be the quotient [covering maps](../../../algebraic-topology.md#covering-space). Since the source universal cover is [simply connected](../../../algebraic-topology.md#simply-connected-space), the [lifting criterion for a covering space](../../../algebraic-topology.md#lifting-criterion-for-a-covering-space) gives a lift $F:\mathbb C^{g_1}\to\mathbb C^{g_2}$ of $f\circ\pi_1$. The lift is a [holomorphic map](../../../complex-analysis.md#holomorphic-map) because $\pi_2$ is locally a [biholomorphism](../../../complex-analysis.md#biholomorphism).

For every $\lambda\in\Lambda_1$, the difference $F(z+\lambda)-F(z)$ belongs to the discrete [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice) $\Lambda_2$. It is a continuous function of $z$ on a [connected](../../../geometry-and-topology.md#connected-space) space, hence is constant. Differentiating shows that each coefficient of $DF$ is $\Lambda_1$-periodic. Such a coefficient is bounded on a compact fundamental parallelepiped, and periodicity bounds it on all of $\mathbb C^{g_1}$. The several-variable [Liouville theorem](../../../complex-analysis.md#liouville-theorem), obtained by applying the one-variable theorem on coordinate lines, makes every coefficient constant.

Consequently $DF=A$ for a constant [complex-linear map](../../../vector-space.md#complex-linear-map) $A$ and $F(z)=Az+x$. The period differences become $A\lambda\in\Lambda_2$. Thus the [affine lift of a holomorphic map between complex tori](../../../complex-geometry.md#affine-lift-of-a-holomorphic-map-between-complex-tori) gives

$$
\boxed{f(z+\Lambda_1)=Az+x+\Lambda_2,\qquad A\Lambda_1\subseteq\Lambda_2.}
$$

**Every holomorphic map between complex tori is a homomorphism followed by a translation.** The translation vector $x=F(0)$ is determined modulo $\Lambda_2$, while $A$ is the derivative of any lift and is unaffected by that ambiguity.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Choose a constant positive [Hermitian form](../../../linear-algebra.md#hermitian-form) on $V$. Its underlying flat [Kähler metric](../../../complex-geometry.md#kahler-metric) is translation-invariant and descends through the [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice) to the compact [complex torus](../../../complex-geometry.md#complex-torus) $X$. The [Dolbeault Hodge decomposition](../../../complex-geometry.md#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) gives a unique [Dolbeault Laplacian](../../../complex-geometry.md#dolbeault-laplacian)-harmonic representative of every [Dolbeault cohomology](../../../complex-geometry.md#dolbeault-cohomology) class. By the [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity), these are also [Hodge Laplacian](../../../differential-form.md#hodge-laplacian)-harmonic.

Choose a constant coframe on $V$. A lifted harmonic form is a sum of constant wedge basis forms with smooth periodic coefficients. For the flat metric, the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian) acts coefficientwise by the scalar constant-coefficient Laplacian. Each coefficient is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) on a compact flat real torus, hence is constant: [integration by parts](../../../calculus.md#integration-by-parts) gives $\int|Da|^2=0$. Conversely every constant-coefficient form is harmonic. Thus the harmonic representatives are exactly the translation-invariant [differential forms of type (p, q)](../../../complex-geometry.md#differential-form-of-type-p-q).

The constant $(1,0)$ covectors form $V^*=\operatorname{Hom}_{\mathbb C}(V,\mathbb C)$; the constant $(0,1)$ covectors form the space of [antilinear maps](../../../vector-space.md#antilinear-map) $\overline{V^*}=\operatorname{Hom}_{\overline{\mathbb C}}(V,\mathbb C)$. Sending a constant wedge form to its cohomology class gives

$$
\boxed{H_{\bar\partial}^{p,q}(X)\cong\bigwedge^pV^*\otimes\bigwedge^q\overline{V^*}.}
$$

The map is intrinsic and does not depend on the auxiliary flat metric: that metric proves every class has exactly one constant representative, while the inclusion of constant forms is defined directly by the quotient. **The Dolbeault cohomology of a complex torus consists of constant forms**, and in particular

$$
h^{p,q}(X)=\binom gp\binom gq,\qquad g=\dim_{\mathbb C}V.
$$

For indices outside $0,\ldots,g$, both the exterior-power expression and the cohomology group vanish.

## 3

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) is a real-linear map (complex-linear for a complex bundle)

$$
D:\Gamma(E)\longrightarrow\mathcal A^1(E),\qquad
D(fs)=df\otimes s+fDs.
$$

It extends to the [covariant exterior derivative](../../../fiber-bundle.md#exterior-covariant-derivative) by $D(\eta\otimes s)=d\eta\otimes s+(-1)^k\eta\wedge Ds$ when $\eta$ has degree $k$. Its square is linear over smooth functions: in $D^2(fs)$ the two $df\wedge Ds$ terms have opposite signs and $d^2f=0$. The [curvature form of a connection](../../../fiber-bundle.md#curvature-form) is therefore the endomorphism-valued two-form

$$
\boxed{\Theta=D^2\in\mathcal A^2(\operatorname{End}E).}
$$

In a local frame with $D=d+\theta$, it is $\Theta=d\theta+\theta\wedge\theta$.

Define the [tensor product connection](../../../fiber-bundle.md#tensor-product-connection) on decomposable sections by

$$
\boxed{D(s\otimes t)=D_1s\otimes t+s\otimes D_2t.}
$$

The [Leibniz rule](../../../calculus.md#leibniz-rule) for $D_1,D_2$ makes this well-defined over smooth functions and makes it a [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle). Applying its [covariant exterior derivative](../../../fiber-bundle.md#exterior-covariant-derivative) again gives

$$
D^2(s\otimes t)=D_1^2s\otimes t-D_1s\wedge D_2t
+D_1s\wedge D_2t+s\otimes D_2^2t.
$$

The mixed terms cancel by the graded sign. Thus **curvature adds on the two tensor factors**:

$$
\boxed{\Theta=\Theta_1\otimes I+I\otimes\Theta_2.}
$$

Equivalently, the mixed terms in $(\theta_1\otimes I+I\otimes\theta_2)\wedge(\theta_1\otimes I+I\otimes\theta_2)$ cancel because operators on the different factors commute. This also proves the [curvature of a tensor product connection](../../../fiber-bundle.md#curvature-of-a-tensor-product-connection) formula in local frames.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Fix the convention that the [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) is conjugate-linear in its first argument. In a [holomorphic local frame](../../../complex-geometry.md#holomorphic-local-trivialization) $e=(e_1,\ldots,e_r)$, let $H_{ij}=h(e_i,e_j)$, so $h(ev,ew)=v^\dagger Hw$. Write $De=e\theta$, or equivalently $D(ev)=e(dv+\theta v)$.

Compatibility with the [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) structure means $D^{0,1}=\bar\partial_E$. Since the frame is holomorphic, this forces $\theta^{0,1}=0$. [Metric compatibility](../../../fiber-bundle.md#metric-compatibility) means

$$
dh(s,t)=h(Ds,t)+h(s,Dt),
$$

or, in the chosen frame, $dH=\theta^\dagger H+H\theta$. Conjugate transpose here also conjugates the one-form factors. Taking the $(1,0)$ component gives $\partial H=H\theta$, and hence

$$
\boxed{\theta=H^{-1}\partial H.}
$$

This proves uniqueness and suggests existence. The proposed $\theta$ has type $(1,0)$, and its conjugate transpose obeys $\theta^\dagger H=\bar\partial H$, since $H=H^\dagger$. Therefore $dH=\theta^\dagger H+H\theta$, proving [metric compatibility](../../../fiber-bundle.md#metric-compatibility) as well.

Under a change of [holomorphic local frame](../../../complex-geometry.md#holomorphic-local-trivialization) $e'=eG$, we have $H'=G^\dagger HG$ and $\partial G^\dagger=0$. A direct computation yields

$$
(H')^{-1}\partial H'=G^{-1}\theta G+G^{-1}\partial G.
$$

Because $G$ is holomorphic, $\partial G=dG$; this is exactly the transformation rule for a [connection one-form](../../../fiber-bundle.md#connection-one-form). The locally defined connections therefore glue to a global [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle). **The Chern connection exists uniquely**, and its [local formula for the Chern connection on a vector bundle](../../../complex-geometry.md#local-formula-for-the-chern-connection-on-a-vector-bundle) is

$$
\boxed{D=d+H^{-1}\partial H,\qquad D^{0,1}=\bar\partial_E.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) $\pi_S$ is a smooth bundle map, since the [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) and the subbundle vary smoothly. The map

$$
E/S\longrightarrow S^\perp,\qquad [v]\longmapsto(I-\pi_S)v
$$

is independent of the representative, bijective on each fibre, and smooth with smooth inverse supplied by the quotient map on $S^\perp$. Hence it is a natural isomorphism of smooth [vector bundles](../../../fiber-bundle.md#vector-bundle). It need not be holomorphic. The [quotient Hermitian metric](../../../complex-geometry.md#quotient-hermitian-metric) is

$$
\boxed{h_Q([v],[w])=h_E((I-\pi_S)v,(I-\pi_S)w).}
$$

It is well-defined and positive definite because $S^\perp$ represents each quotient class uniquely.

On sections of $S$, set $D'=\pi_S D_E$. The [Leibniz rule](../../../calculus.md#leibniz-rule) makes $D'$ a [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle). For $s,t\in\Gamma(S)$, the orthogonal terms vanish in the metric pairing, so

$$
dh_S(s,t)=h_S(D's,t)+h_S(s,D't).
$$

Thus $D'$ has [metric compatibility](../../../fiber-bundle.md#metric-compatibility). Because $S$ is a holomorphic subbundle, the $(0,1)$ part of $D_E$ preserves $S$ and restricts to $\bar\partial_S$. Therefore $(D')^{0,1}=\bar\partial_S$. The uniqueness of the [Chern connection](../../../complex-geometry.md#chern-connection) in part (b) gives the [projected Chern connection](../../../complex-geometry.md#projected-chern-connection) formula

$$
\boxed{D_S=\pi_S D_E.}
$$

It follows that $A(s)=(I-\pi_S)D_Es$ is a quotient-valued one-form. **The printed target $T_M\otimes Q$ is missing a dual:** the [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle) is the correct factor,

$$
\boxed{A(s)\in\Gamma(T_M^*\otimes Q).}
$$

Complex-valued forms use the complexified cotangent bundle here. In fact the $(0,1)$ part cancels, so $A$ is the [second fundamental form of a holomorphic subbundle](../../../complex-geometry.md#second-fundamental-form-of-a-holomorphic-subbundle), an element of $\mathcal A^{1,0}(\operatorname{Hom}(S,Q))$. Finally the two connection [Leibniz rules](../../../calculus.md#leibniz-rule) give

$$
A(fs)=df\otimes s+fD_Es-df\otimes s-fD_Ss
=\boxed{fA(s)}.
$$

This proves its [tensoriality](../../../fiber-bundle.md#tensoriality) and all the asserted quotient and projection properties.

## 4

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For the usual additive [Čech cohomology](../../../ringed-space.md#cech-cohomology) groups, $\mathcal F$ is understood to be a [sheaf of abelian groups](../../../algebraic-geometry.md#sheaf-of-abelian-groups). Order the index set of the [open cover](../../../topology.md#open-cover) $\mathfrak U=(U_i)$. The [Čech cochain group](../../../ringed-space.md#cech-cochain-group) is

$$
\check C^q(\mathfrak U,\mathcal F)=\prod_{i_0<\cdots<i_q}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_q}),\qquad q\geq0.
$$

An empty intersection contributes the zero group. The [Čech coboundary](../../../ringed-space.md#cech-coboundary) is the alternating sum of restriction maps:

$$
(\delta c)_{i_0\ldots i_{q+1}}
=\sum_{a=0}^{q+1}(-1)^a
c_{i_0\ldots\widehat{i_a}\ldots i_{q+1}}\big|_{U_{i_0}\cap\cdots\cap U_{i_{q+1}}}.
$$

Every double omission appears twice with opposite sign, so $\delta^2=0$. **The Čech cohomology is the cohomology of this cochain complex**:

$$
\boxed{\check H^q(\mathfrak U,\mathcal F)
=\frac{\ker(\delta:\check C^q\to\check C^{q+1})}{\operatorname{im}(\delta:\check C^{q-1}\to\check C^q)}.}
$$

Here $\check C^{-1}=0$. The [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) identifies $\check H^0(\mathfrak U,\mathcal F)$ with $\Gamma(X,\mathcal F)$. This definition is for the fixed cover; no limit over refinements is part of the group requested here. Without the abelian-group structure, this additive [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex) is not defined.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The two opens are $U_1=\mathbb C\times\mathbb C^*$ and $U_2=\mathbb C^*\times\mathbb C$; their intersection is $(\mathbb C^*)^2$. There is just one degree-one term in the [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex), and no degree-two term. The [Čech coboundary](../../../ringed-space.md#cech-coboundary) sends $(g_1,g_2)$ to $g_2-g_1$, so

$$
\boxed{\check H^1(\mathfrak U,\mathcal O_X)
=\frac{\mathcal O((\mathbb C^*)^2)}{\mathcal O(\mathbb C\times\mathbb C^*)+\mathcal O(\mathbb C^*\times\mathbb C)}.}
$$

The denominator denotes the sum of the restricted function spaces.

To make the quotient explicit, expand a [holomorphic function](../../../complex-analysis.md#holomorphic-function) on the intersection in a normally convergent two-variable [Laurent series](../../../analysis.md#laurent-series),

$$
h=\sum_{m,n\in\mathbb Z}a_{mn}z_1^mz_2^n.
$$

The terms with $m\geq0$ extend to $U_1$. Of the remaining terms, those with $n\geq0$ extend to $U_2$. Both subseries converge normally on their stated domains, by the coefficient bounds from the [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula). The unique remaining representative is the doubly negative part

$$
h_{--}=\sum_{i,j\geq1}a_{-i,-j}z_1^{-i}z_2^{-j}.
$$

No nonzero series of this form lies in the denominator, since a function on $U_1$ has no negative $z_1$ exponents and a function on $U_2$ has no negative $z_2$ exponents.

Writing $w_i=z_i^{-1}$, these representatives are exactly $w_1w_2F(w_1,w_2)$ with $F$ an entire [holomorphic function](../../../complex-analysis.md#holomorphic-function) on $\mathbb C^2$. To see that $F$ is entire, integrate for the coefficients on arbitrarily small product circles: $|a_{-i,-j}|\leq M(r_1,r_2)r_1^ir_2^j$. Choosing $r_iR_i<1$ gives absolute convergence for $|w_i|\leq R_i$, for every finite pair $R_i$. Conversely every such entire $F$ supplies a normally convergent representative on the intersection. Therefore **the quotient consists of convergent doubly negative Laurent series**, not merely finite Laurent polynomials:

$$
\boxed{\check H^1(\mathfrak U,\mathcal O_X)\cong w_1w_2\mathcal O(\mathbb C_w^2).}
$$

This gives the [holomorphic first cohomology of punctured complex two-space](../../../ringed-space.md#holomorphic-first-cohomology-of-punctured-complex-two-space); for instance $1/(z_1z_2)$ represents a nonzero class.

For the comparison with [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology), $U_1,U_2$ and their intersection are [Stein manifolds](../../../complex-geometry.md#stein-manifold). They can be realized as closed [complex submanifolds](../../../complex-geometry.md#complex-submanifold) of affine complex spaces by adding equations $z_iw_i=1$ for their nonzero coordinates. [Cartan theorem B](../../../complex-geometry.md#cartan-theorem-b) makes their higher cohomology with coefficients in the [sheaf of holomorphic functions](../../../complex-geometry.md#structure-sheaf-of-a-complex-manifold) vanish. Thus the cover is acyclic for $\mathcal O_X$, and the [acyclic cover theorem](../../../ringed-space.md#leray-s-theorem) gives

$$
\boxed{\check H^1(\mathfrak U,\mathcal O_X)\cong H^1(X,\mathcal O_X).}
$$

The individual cover members are Stein; their union has the nonzero cohomology just computed.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Treat $0$ as the trivial group if $G$ is not abelian. The restriction maps satisfy the presheaf identities. To verify the [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom), take an [open cover](../../../topology.md#open-cover) $(V_i)$ of $U$. If $x\notin U$, every section group is trivial. If $x\in U$, at least one $V_i$ contains $x$. Every two such opens have an overlap containing $x$, so compatibility forces all their sections to have the same value $g\in G$. Opens not containing $x$ have their unique trivial section. The value $g\in\mathcal G(U)$ is exactly the unique glued section. Thus **the stated presheaf is a skyscraper sheaf**, including for nonabelian groups.

For the [stalk of a sheaf](../../../ringed-space.md#stalk-of-a-sheaf), take the direct limit over neighbourhoods of $y$. If some neighbourhood $V$ of $y$ omits $x$, neighbourhoods inside $V$ are cofinal and all their groups are trivial. If every neighbourhood of $y$ contains $x$, every group in the system is $G$ and every transition map is the identity. Consequently, on the arbitrary [topological space](../../../topology.md#topological-space) in the question,

$$
\boxed{\mathcal G_y\cong
\begin{cases}
G,&y\in\overline{\{x\}},\\
0,&y\notin\overline{\{x\}}.
\end{cases}}
$$

Membership in this [closure](../../../topology.md#closure-topology) means exactly that every neighbourhood of $y$ contains $x$. In particular $\mathcal G_x=G$. If $x$ is a [closed point](../../../topology.md#closed-point), the [closure](../../../topology.md#closure-topology) is just $\{x\}$ and the familiar point-supported answer results. The separation assumption is not present in the printed question, so it cannot be imposed silently.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $\mathcal P=\mathcal M_X/\mathcal O_X$, the [sheaf of meromorphic principal parts](../../../complex-geometry.md#sheaf-of-meromorphic-principal-parts). Exactness of taking [stalks](../../../ringed-space.md#stalk-of-a-sheaf) gives

$$
\mathcal P_x=\mathcal M_{X,x}/\mathcal O_{X,x}.
$$

Choose a [holomorphic coordinate](../../../complex-geometry.md#holomorphic-coordinate) $t$ vanishing at $x$. Every meromorphic germ has a finite negative tail in its [Laurent series](../../../analysis.md#laurent-series); the holomorphic tail vanishes in the quotient. Hence

$$
\boxed{\mathcal P_x\cong\bigoplus_{m\geq1}\mathbb C\,t^{-m}.}
$$

This coordinate description is a vector-space identification; the intrinsic space is the quotient of germs, so a coordinate change need not preserve the displayed basis.

For each point inclusion $i_x:\{x\}\to X$, a principal part defines a local meromorphic germ near $x$, whose quotient class is zero off $x$. Gluing with zero on the complement gives a map from its [skyscraper sheaf](../../../ringed-space.md#skyscraper-sheaf) to $\mathcal P$. These maps induce an isomorphism on every stalk and therefore an isomorphism of sheaves:

$$
\boxed{\mathcal P\cong\bigoplus_{x\in X}(i_x)_*\mathcal P_x.}
$$

The [direct sum of sheaves](../../../algebraic-geometry.md#direct-sum-of-sheaves) means the sheafification of the sectionwise direct-sum presheaf. Its sections can have infinitely many nonzero components globally, but their point supports form a [locally finite family of subsets](../../../topology.md#locally-finite-family-of-subsets). This matches the fact that poles of a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) are locally finite. On a compact [Riemann surface](../../../complex-analysis.md#riemann-surfaces) only finitely many points can occur; on a noncompact one a discrete infinite family is allowed.

For a global principal-part family $P$, choose local meromorphic lifts $m_i$ on a sufficiently small [open cover](../../../topology.md#open-cover). The differences $m_j-m_i$ are [holomorphic functions](../../../complex-analysis.md#holomorphic-function) and form a [Čech cocycle](../../../ringed-space.md#cech-cocycle-condition). The [connecting homomorphism](../../../homology.md#connecting-homomorphism) sends $P$ to the resulting class in $H^1(X,\mathcal O_X)$. If this class vanishes, after refining the cover write $m_j-m_i=h_j-h_i$; then the functions $m_i-h_i$ glue to a global [meromorphic function](../../../isolated-singularity.md#meromorphic-function). Conversely any global lift makes the class zero. Equivalently, exactness of the given [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) says

$$
\boxed{\delta(P)=0\iff\text{there is a global meromorphic function with exactly the prescribed principal parts}.}
$$

**The connecting class is the obstruction to the Mittag-Leffler problem on a Riemann surface.** It rules on the specified poles and their finite negative Laurent tails, with no additional poles allowed. When a solution exists, any two solutions differ by a global [holomorphic function](../../../complex-analysis.md#holomorphic-function).

## 5

↑ **Parent:** [Paper 118](paper-118.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

This is the [Poincaré residue](../../../complex-geometry.md#poincare-residue-along-a-smooth-hypersurface) of a meromorphic top form with a simple pole. Write $z=z_1$ and locally $\alpha=(dz/z)\wedge\beta$, with $\beta$ a holomorphic $(n-1)$-form. The proposed residue is the pullback of $\beta$ to $Y$.

First it does not depend on the choice of $\beta$: if $dz\wedge(\beta-\beta')=0$, then at each point the difference has a factor $dz$, and its pullback to $Y$ is zero. Now change the local defining coordinate to $t=az$, where $a$ is a nowhere-zero [holomorphic function](../../../complex-analysis.md#holomorphic-function). Such a factor exists because both coordinates define the same smooth [complex analytic hypersurface](../../../complex-geometry.md#complex-analytic-hypersurface). If $\alpha=(dt/t)\wedge\eta$, then

$$
dz\wedge\beta=z\alpha=\frac1a\,dt\wedge\eta
=dz\wedge\eta+\frac za\,da\wedge\eta.
$$

At points of $Y$, this is an equality in the ambient exterior-power fibre, and the last term is zero. It follows that $dz\wedge(\beta-\eta)=0$ there, so their pullbacks to $Y$ agree. This also covers changes of the tangential coordinates.

The restrictions are holomorphic top forms on $Y$, and their agreement on overlaps makes them a global section of the [canonical bundle](../../../complex-geometry.md#canonical-bundle). Thus **the residue is independent of the adapted coordinates**:

$$
\boxed{\operatorname{Res}_Y(\alpha)\in\Gamma(Y,K_Y),\qquad
\operatorname{Res}_Y(\alpha)=\left.h\,dz_2\wedge\cdots\wedge dz_n\right|_Y.}
$$

The ambient-fibre comparison is important: pulling an ambient $n$-form directly back to the $(n-1)$-dimensional hypersurface would give zero and would not prove the required independence.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

On $\mathbb C^{n+1}\setminus\{0\}$, let $\Omega=dz_0\wedge\cdots\wedge dz_n$ and let $E=\sum_i z_i\partial_{z_i}$ be the [Euler vector field](../../../complex-geometry.md#euler-vector-field). The numerator is its [interior product of a differential form](../../../differential-form.md#interior-product), so

$$
\alpha=\frac{\iota_E\Omega}{f}.
$$

Both numerator and denominator have homogeneous scaling degree $n+1$. Thus this meromorphic $n$-form is invariant under constant nonzero scalings, and $\iota_E\alpha=0$ makes it horizontal for the quotient to [Complex projective space](../../../algebraic-topology.md#complex-projective-space).

To check descent using the hint, take a local holomorphic section $Z$ of the quotient and another section $Z'=\lambda Z$, where $\lambda$ is a nowhere-zero [holomorphic function](../../../complex-analysis.md#holomorphic-function). In the evaluation

$$
(Z')^*(\iota_E\Omega)(v_1,\ldots,v_n)
=\Omega\bigl(\lambda Z,\lambda\,dZ(v_1)+d\lambda(v_1)Z,\ldots,\lambda\,dZ(v_n)+d\lambda(v_n)Z\bigr),
$$

every term involving $d\lambda$ has two collinear arguments and vanishes. The remaining term is $\lambda^{n+1}Z^*(\iota_E\Omega)$, while $f(\lambda Z)=\lambda^{n+1}f(Z)$. Hence $Z'^*\alpha=Z^*\alpha$. The forms therefore glue to a meromorphic section of the [canonical bundle](../../../complex-geometry.md#canonical-bundle) of [Complex projective space](../../../algebraic-topology.md#complex-projective-space).

On the affine chart $z_j\ne0$, use the section $z_j=1$ and list the remaining coordinates as $t_1,\ldots,t_n$ in increasing original-index order. If $F$ is the resulting polynomial, then

$$
\alpha=(-1)^j\frac{dt_1\wedge\cdots\wedge dt_n}{F}.
$$

At a point of $Y$, some derivative $F_{t_r}$ is nonzero. Otherwise all the homogeneous derivatives except possibly $f_{z_j}$ would vanish; the [Euler homogeneous function theorem](../../../real-analysis.md#euler-theorem-for-homogeneous-functions) gives $\sum_i z_if_{z_i}=(n+1)f=0$ there, forcing $f_{z_j}=0$ too. This contradicts the permitted smoothness criterion. The [holomorphic inverse function theorem](../../../geometry-and-topology.md#holomorphic-inverse-function-theorem) now makes $F$ a transverse coordinate, so the pole is simple. On a neighbourhood with $F_{t_r}\ne0$, rearranging the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms) gives

$$
\alpha=\frac{dF}{F}\wedge
\frac{(-1)^{j+r-1}}{F_{t_r}}\,dt_1\wedge\cdots\wedge\widehat{dt_r}\wedge\cdots\wedge dt_n.
$$

By part (a), its [Poincaré residue](../../../complex-geometry.md#poincare-residue-along-a-smooth-hypersurface) is consequently

$$
\boxed{\operatorname{Res}_Y(\alpha)=
\left.\frac{(-1)^{j+r-1}}{F_{t_r}}\,dt_1\wedge\cdots\wedge\widehat{dt_r}\wedge\cdots\wedge dt_n\right|_Y.}
$$

The remaining $t$ coordinates form a [holomorphic coordinate](../../../complex-geometry.md#holomorphic-coordinate) system on $Y$, and $F_{t_r}$ is nonzero in this neighbourhood. The displayed top form is therefore nowhere zero. These neighbourhoods cover $Y$ and part (a) guarantees agreement on their overlaps. **The residue is a nowhere-vanishing global holomorphic section**:

$$
\boxed{K_Y\cong\mathcal O_Y.}
$$

This is the explicit [residue trivialization for a degree n+1 projective hypersurface](../../../complex-geometry.md#residue-trivialization-for-a-degree-n-plus-1-projective-hypersurface), consistent with the [adjunction formula](../../../complex-geometry.md#adjunction-formula) $K_Y\cong\mathcal O_Y((n+1)-n-1)$, but obtained here directly from the indicated form.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
