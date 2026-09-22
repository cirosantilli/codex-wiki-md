# Paper 357

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20357.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20357.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
  - [g](#3/g)
    - [Solution](#3/g/solution)

## 1

↑ **Parent:** [Paper 357](paper-357.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a fixed scalar function $f$, the equation $\Box_gf=0$ is coordinate invariant. A coordinate label $x^\lambda$, however, is not a geometrically specified scalar under an arbitrary change of chart: a nonlinear redefinition of harmonic coordinates need not remain harmonic. Thus $\Box_gx^\lambda=0$ is a coordinate or gauge condition selecting a class of charts, rather than a tensor equation asserting the vanishing of a tensor field with index $\lambda$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Treating $x^\lambda$ as a scalar during differentiation,

$$
\nabla_\mu\nabla_\nu x^\lambda
=\partial_\mu\partial_\nu x^\lambda
-\Gamma^\rho_{\mu\nu}\partial_\rho x^\lambda
=-\Gamma^\lambda_{\mu\nu}.
$$

Hence

$$
\boxed{\Box_gx^\lambda=0
\iff g^{\mu\nu}\Gamma^\lambda_{\mu\nu}=0}.
$$

Metric compatibility and the determinant identity give the contracted-Christoffel formula

$$
g^{\mu\nu}\Gamma^\lambda_{\mu\nu}
=-\frac1{\sqrt{-g}}\partial_\mu
(\sqrt{-g}\,g^{\lambda\mu}).
$$

Therefore

$$
\boxed{g^{\mu\nu}\Gamma^\lambda_{\mu\nu}=0
\iff\partial_\mu(\sqrt{-g}\,g^{\lambda\mu})=0}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Differentiate the determinant using $\partial\gamma/\partial\gamma_{ij}=\gamma\gamma^{ij}$:

$$
\partial_t\gamma=\gamma\gamma^{ij}\partial_t\gamma_{ij}.
$$

The advection term is $\gamma\gamma^{ij}\beta^m\partial_m\gamma_{ij}=\beta^m\partial_m\gamma$. The symmetrized shift-gradient term contracts to $2\gamma\partial_m\beta^m$, and the curvature term to $-2\alpha\gamma K$. Thus

$$
\boxed{\partial_t\gamma
=\beta^m\partial_m\gamma+2\gamma\partial_m\beta^m
-2\alpha\gamma K}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $\lambda=0$, $\sqrt{-g}=\alpha\sqrt\gamma$, $g^{00}=-\alpha^{-2}$, and $g^{0i}=\beta^i\alpha^{-2}$. The [harmonic coordinate](../../../numerical-relativity.md#harmonic-coordinate) condition is

$$
\partial_t\left(-\frac{\sqrt\gamma}{\alpha}\right)
+\partial_i\left(\frac{\sqrt\gamma\,\beta^i}{\alpha}\right)=0.
$$

Using

$$
\frac{\partial_t\sqrt\gamma}{\sqrt\gamma}
=\beta^i\partial_i\log\sqrt\gamma
+\partial_i\beta^i-\alpha K
$$

from the determinant evolution, all shift-divergence and volume terms cancel, leaving

$$
\boxed{(\partial_t-\beta^i\partial_i)\alpha=-\alpha^2K}.
$$

Thus harmonic slicing is the [Bona--Masso slicing condition](../../../numerical-relativity.md#bona-masso-slicing-condition) with

$$
\boxed{f(\alpha)=1}.
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The Ricci tensor contains second derivatives from $\partial\Gamma$ and quadratic first-derivative terms from $\Gamma\Gamma$. Its second-derivative terms can be rearranged as

$$
R_{\alpha\beta}
=-\frac12g^{\mu\nu}\partial_\mu\partial_\nu g_{\alpha\beta}
+\partial_{(\alpha}\Gamma_{\beta)}
+Q_{\alpha\beta}(g,\partial g),
$$

where $\Gamma_\beta=g_{\beta\lambda}g^{\mu\nu}\Gamma^\lambda_{\mu\nu}$. Harmonic gauge sets $\Gamma_\beta=0$, so

$$
\boxed{R_{\alpha\beta}
=-\frac12g^{\mu\nu}\partial_\mu\partial_\nu g_{\alpha\beta}
+Q_{\alpha\beta}(g,\partial g)=0}.
$$

The principal part is the spacetime wave operator acting on every metric component. This [hyperbolic reduction of Einstein's equations](../../../numerical-relativity.md#hyperbolic-reduction-of-einstein-s-equations) turns the reduced vacuum equations into a quasilinear hyperbolic system with finite-speed propagation and a well-posed local Cauchy problem, provided the constraints and harmonic gauge constraints hold initially.

## 2

↑ **Parent:** [Paper 357](paper-357.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

From $\gamma=c/r+O(r^{-2})$,

$$
\partial_r\gamma=-\frac c{r^2}+O(r^{-3}).
$$

The first hypersurface equation gives

$$
\partial_r\beta=\frac{c^2}{2r^3}+O(r^{-4}),
$$

and hence

$$
\boxed{\beta=\beta_0(u,\theta)-\frac{c^2}{4r^2}+O(r^{-3})}.
$$

Asymptotic flatness in the standard Bondi frame sets the integration function $\beta_0=0$.

With this choice, the leading bracket in the second hypersurface equation is

$$
\frac{\partial_\theta c+2c\cot\theta}{r^2}+O(r^{-3}).
$$

Therefore

$$
\partial_r(r^4\partial_rU)
=2(\partial_\theta c+2c\cot\theta)+O(r^{-1}).
$$

Writing $D=\partial_\theta c+2c\cot\theta$ and integrating twice,

$$
\boxed{U=U_0(u,\theta)-\frac{D}{r^2}
-\frac{U_3(u,\theta)}{3r^3}+O(r^{-4})}.
$$

Standard asymptotic flatness sets $U_0=0$; $U_3$ is free integration data at the next order.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The azimuthal metric component is

$$
g_{\phi\phi}=r^2e^{-2\gamma}\sin^2\theta.
$$

Since $\gamma=c/r+O(r^{-2})$,

$$
\partial_ug_{\phi\phi}
=-2r^2e^{-2\gamma}(\partial_u\gamma)\sin^2\theta
=-2r(\partial_uc)\sin^2\theta+O(1).
$$

Thus the [Bondi news function](../../../general-relativity.md#bondi-news-function) satisfies

$$
\boxed{\partial_uc
=-\frac12\lim_{r\to\infty}
r^{-1}(\sin\theta)^{-2}\partial_ug_{\phi\phi}}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Only the transverse metric components are needed. At fixed $(u,r,\theta)$,

$$
\partial_\phi\widetilde x=-\widetilde y,
\qquad
\partial_\phi\widetilde y=\widetilde x.
$$

Contracting this vector with the $\widetilde x,\widetilde y$ block of the metric makes all angular factors combine to $\widetilde\rho^2$:

$$
g_{\phi\phi}
=\kappa^2\widetilde\rho^2
+\kappa\lambda\widetilde\rho^2E
=r^2\sin^2\theta
\left(1+\frac\lambda\kappa E\right).
$$

Substitution into the preceding news formula gives

$$
\boxed{\partial_uc
=-\frac\lambda{2\kappa}
\lim_{r\to\infty}\left(r\,\partial_uE\right)}.
$$

Therefore the requested constants are

$$
\boxed{p=-\frac\lambda{2\kappa},\qquad q=1}.
$$

## 3

↑ **Parent:** [Paper 357](paper-357.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Decompose each index with $\delta^\rho{}_\mu=\perp^\rho{}_\mu-n^\rho n_\mu$. Since $n^\nu n_\nu=-1$, one has $n^\nu\nabla_\mu n_\nu=0$, so the second index of $\nabla_\mu n_\nu$ is spatial. Its spatial projection in the first index is $-K_{\mu\nu}$ by definition, while its normal projection is

$$
-n_\mu n^\rho\nabla_\rho n_\nu=-n_\mu a_\nu.
$$

Hence

$$
\boxed{\nabla_\mu n_\nu=-K_{\mu\nu}-n_\mu a_\nu}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use $n_\mu=-\alpha\nabla_\mu t$. Differentiating, contracting with $n^\rho$, and using $n^\rho\nabla_\rho t=1/\alpha$ gives a gradient of $\log\alpha$ plus a component parallel to $n_\mu$. The acceleration is orthogonal to $n^\mu$, so spatial projection removes the parallel part:

$$
\boxed{a_\mu=D_\mu\log\alpha
=\frac{D_\mu\alpha}{\alpha}}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Because $n^\mu\partial_\mu\phi=-2\Pi$,

$$
Q=-n_\mu J^\mu
=i(\bar\phi\Pi-\phi\bar\Pi).
$$

Writing $\phi=\phi_R+i\phi_I$ and $\Pi=\Pi_R+i\Pi_I$ gives

$$
\boxed{Q=2(\phi_I\Pi_R-\phi_R\Pi_I)}.
$$

Every quantity on the right is real, so the Noether charge density is explicitly real valued.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

By definition,

$$
Q^\alpha=(\delta^\alpha{}_\mu+n^\alpha n_\mu)J^\mu
=J^\alpha+n^\alpha(n_\mu J^\mu)
=J^\alpha-Qn^\alpha.
$$

Therefore

$$
\boxed{J^\alpha=Qn^\alpha+Q^\alpha},
$$

with $n_\alpha Q^\alpha=0$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Taking the divergence of the [Noether current](../../../quantum-field-theory.md#noether-current),

$$
\nabla_\mu J^\mu
=\frac i2\left[
\bar\phi\Box\phi-\phi\Box\bar\phi
\right],
$$

because the two gradient-product terms cancel. The field equation and its conjugate are $\Box\phi=V'\phi$ and $\Box\bar\phi=V'\bar\phi$, with real $V'(|\phi|^2)$. Hence

$$
\boxed{\nabla_\mu J^\mu=0}.
$$

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Insert $J^\mu=Qn^\mu+Q^\mu$:

$$
0=n^\mu\nabla_\mu Q+Q\nabla_\mu n^\mu+\nabla_\mu Q^\mu.
$$

The extrinsic-curvature convention gives $\nabla_\mu n^\mu=-K$. For a spatial vector,

$$
\nabla_\mu Q^\mu=D_\mu Q^\mu+Q^\mu a_\mu.
$$

Therefore

$$
\boxed{n^\mu\nabla_\mu Q
=KQ-D_\mu Q^\mu-Q^\mu a_\mu}.
$$

The constants are

$$
\boxed{c_1=1,\qquad c_2=-1,\qquad c_3=-1}.
$$

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

In adapted coordinates,

$$
n^\mu\nabla_\mu Q
=\frac1\alpha(\partial_t-\beta^i\partial_i)Q,
\qquad
a_i=\frac{D_i\alpha}{\alpha}.
$$

Multiplying the conservation law by $\alpha$ gives

$$
\boxed{\partial_tQ
=\beta^i\partial_iQ+\alpha KQ
-\alpha D_iQ^i-Q^iD_i\alpha}.
$$

Equivalently, combining the last two terms,

$$
\boxed{\partial_tQ
=\beta^i\partial_iQ+\alpha KQ
-D_i(\alpha Q^i)}.
$$

This is the coordinate form of the [3+1 Noether-current conservation law](../../../numerical-relativity.md#3-plus-1-noether-current-conservation-law).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
