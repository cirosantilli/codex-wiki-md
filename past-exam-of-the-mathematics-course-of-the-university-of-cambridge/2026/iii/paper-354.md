# Paper 354

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20354.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20354.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)

## 1

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [Euclidean conformal transformation](../../../string-theory.md#euclidean-conformal-transformation) is a coordinate map whose Jacobian preserves angles:

$$
\frac{\partial\widetilde x^\rho}{\partial x^\mu}
\frac{\partial\widetilde x^\sigma}{\partial x^\nu}
\delta_{\rho\sigma}=\Omega(x)^2\delta_{\mu\nu}.
$$

For $\widetilde x^\mu=x^\mu+\delta\epsilon^\mu+O(\delta^2)$, its left side is

$$
\delta_{\mu\nu}+\delta(\partial_\mu\epsilon_\nu+
\partial_\nu\epsilon_\mu)+O(\delta^2).
$$

Taking the trace identifies the infinitesimal scale change as $2\partial\cdot\epsilon/d$. The traceless part must vanish, giving the [Conformal Killing equation](../../../general-relativity.md#conformal-killing-equation)

$$
\boxed{\partial_\mu\epsilon_\nu+\partial_\nu\epsilon_\mu
=\frac2d(\partial\cdot\epsilon)\delta_{\mu\nu}}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Translation and rotation invariance make the two-point function depend only on $|x_{12}|$. Scale covariance then fixes its power, and inversion or special-conformal invariance requires equal dimensions for a nonzero scalar two-point function. For identical [scalar primary operators](../../../string-theory.md#primary-field),

$$
\boxed{\langle O(x_1)O(x_2)\rangle
=\frac{C_2}{|x_{12}|^{2\Delta}}}.
$$

Only the normalization $C_2$ depends on the operator convention.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The same symmetries fix the scalar three-point function to

$$
\boxed{
\langle O_1(x_1)O_2(x_2)O_3(x_3)\rangle
=\frac{C_{123}}
{|x_{12}|^{\Delta_1+\Delta_2-\Delta_3}
 |x_{23}|^{\Delta_2+\Delta_3-\Delta_1}
 |x_{31}|^{\Delta_3+\Delta_1-\Delta_2}}}.
$$

Each insertion acquires total scaling weight $2\Delta_i$ from the two distances containing it, while special conformal transformations leave no independent cross-ratio for three points.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Under the [AdS/CFT correspondence](../../../string-theory.md#ads-cft-correspondence), each [single-trace operator](../../../string-theory.md#single-trace-operator) is represented by one bulk field. The leading two-point [Witten diagram](../../../string-theory.md#witten-diagram) is a bulk propagator joining the two boundary insertions, equivalently two bulk-to-boundary legs contracted through the quadratic bulk action. The leading connected three-point diagram has one bulk cubic vertex integrated over AdS and three bulk-to-boundary propagators ending at $x_1,x_2,x_3$. The bulk kinetic normalization fixes $C_2$, while the cubic coupling fixes $C_{123}$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For three identical operators, conformal invariance gives

$$
\langle O(x)O(0)O(y)\rangle
=\frac{C_3}{|x|^\Delta|y|^\Delta|y-x|^\Delta}.
$$

When $|x|\ll|y|$, $|y-x|=|y|[1+O(|x|/|y|)]$, so

$$
\langle O(x)O(0)O(y)\rangle
\sim\frac{C_3}{|x|^\Delta|y|^{2\Delta}}.
$$

Inserting the [operator product expansion](../../../string-theory.md#operator-product-expansion), the identity term has zero expectation with $O(y)$, while the $O(0)$ term gives

$$
\frac{C_{OOO}^{\rm OPE}}{|x|^\Delta}
\langle O(0)O(y)\rangle
=\frac{C_{OOO}^{\rm OPE}C_2}{|x|^\Delta|y|^{2\Delta}},
$$

which has precisely the required position dependence.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Comparing the coefficients in the short-distance limit gives

$$
\boxed{C_{OOO}^{\rm OPE}=\frac{C_3}{C_2}}.
$$

If the operator is normalized so that $C_2=1$, its OPE coefficient equals the three-point normalization.

## 2

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Varying the gauge field and integrating by parts gives

$$
\boxed{\nabla_aF^{ab}=0},
\qquad
\boxed{\nabla_{[a}F_{bc]}=0},
$$

the second identity following from $F=dA$. Varying the inverse metric, using

$$
\delta F^2=2F_{ac}F_b{}^c\delta g^{ab},
$$

and discarding the Einstein--Hilbert boundary term gives

$$
\boxed{R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}
=2\left(F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd}\right)}.
$$

For AdS$_4$, $\Lambda=-3/L^2$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The horizon equation gives

$$
2M=\frac{r_+^3}{L^2}+\frac{Q^2}{r_+}.
$$

With $Q=r_+^2\mu/L$, define

$$
g(z)=1-(1+\mu^2)z^3+\mu^2z^4.
$$

The coordinate changes in the question give

$$
\boxed{ds^2=\frac{L^2}{z^2}
\left[-g(z)d\tau^2+\frac{dz^2}{g(z)}+dX^2+dY^2\right]},
$$



$$
\boxed{A=\mu L(1-z)d\tau}.
$$

The horizon is at $z=1$, and all nontrivial dimensionless dependence is through $\mu$; $L$ remains only as the overall curvature scale.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Choose the [Fefferman--Graham coordinates](../../../string-theory.md#fefferman-graham-coordinates) radial variable from

$$
\frac{dZ}{Z}=\frac{dz}{z\sqrt{g(z)}}.
$$

Near the boundary,

$$
Z=z\left[1+\frac{1+\mu^2}{6}z^3+O(z^4)\right],
\qquad
z=Z+O(Z^4).
$$

Consequently, through $O(Z^2)$,

$$
\boxed{ds^2=\frac{L^2}{Z^2}
\left[dZ^2-d\tau^2+dX^2+dY^2+O(Z^3)\right]},
$$



$$
\boxed{A_\tau=\mu L-\mu LZ+O(Z^4)}.
$$

By the [holographic dictionary](../../../string-theory.md#holographic-dictionary), the leading boundary value of $A_\tau$ is the source for charge density. Thus $\mu$ is the dimensionless [holographic chemical potential](../../../string-theory.md#holographic-chemical-potential); the coefficient of the normalizable linear term is proportional to the CFT charge density, $\rho=\mu L/(4\pi G)$ with the action normalization and outward-orientation convention used here.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The transformation is a boundary Lorentz boost of rapidity $\beta$. It preserves $-d\tau^2+dX^2=-dT^2+dW^2$ and describes the charged thermal state in a frame moving with speed $|v|=\tanh\beta$. The gauge field becomes

$$
A=\mu L(1-z)(\cosh\beta\,dT+\sinh\beta\,dW).
$$

If the rest-frame contravariant current is $J^\mu=(\rho,0,0)$, then in the new coordinates

$$
\boxed{J^T=\rho\cosh\beta,
\qquad J^W=-\rho\sinh\beta,
\qquad J^Y=0},
$$

where the sign of the spatial component follows from the stated passive coordinate transformation. Reversing the boost convention reverses that sign. For small $\beta$, the induced spatial current is $J^W\simeq-\rho\beta$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The boost produces a persistent current without an applied electric field. More generally, at nonzero charge density a homogeneous electric field injects momentum, and exact translation invariance provides no mechanism to relax it. Therefore

$$
\boxed{\sigma_{\rm DC}=\infty}.
$$

Equivalently, the real optical conductivity contains a delta function at zero frequency and its imaginary part has a $1/\omega$ pole. This [holographic D.C. conductivity](../../../string-theory.md#holographic-d-c-conductivity) is physically reasonable for the ideal translationally invariant model. A lattice, disorder, impurities, or another source of momentum relaxation is needed for finite D.C. resistivity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
