# Paper 107

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_107.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_107.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
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
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $M=\sup_\Omega u$ and suppose $u(y)=M$. The set $\Omega_M=\{x\in\Omega:u(x)=M\}$ is closed in $\Omega$ by [continuity](../../../calculus.md#continuous-function). If $x\in\Omega_M$, choose a ball $B(x,r)\Subset\Omega$. The [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) assumed in the question gives

$$
M=u(x)=\frac1{|B(x,r)|}\int_{B(x,r)}u\leq M.
$$

The nonnegative continuous function $M-u$ consequently has integral zero and therefore vanishes throughout the ball. Thus $\Omega_M$ is also open. Since $\Omega$ is [connected](../../../geometry-and-topology.md#connected-space) and $\Omega_M$ is nonempty, $\Omega_M=\Omega$, so $u$ is constant. Applying the same argument to $-u$ proves the assertion for an attained infimum.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Fix $B=B(x_0,r)\Subset\Omega$. Solvability of the [Dirichlet problem](../../../analysis.md#dirichlet-problem) on a ball gives a unique [harmonic function](../../../partial-differential-equation.md#harmonic-function) $h\in C^2(B)\cap C^0(\overline B)$ with $h=u$ on $\partial B$. Both $u$ and $h$ have the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions), so $v=u-h$ has it as well and vanishes on $\partial B$.

If $v$ were not zero, compactness of $\overline B$ would give either a positive maximum or a negative minimum in the interior. Part 1(i) would make $v$ constant, contradicting its zero boundary values. Hence $u=h$ on $B$. Every point lies in such a ball, so

$$
\boxed{\Delta u=0\text{ throughout }\Omega.}
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Radiality gives $\phi_\varepsilon(x-y)=\phi_\varepsilon(y-x)$. Since $\phi_\varepsilon$ is supported in $B(0,\varepsilon)$, the changes of variables $y=x+z$ and then $z=\varepsilon r\omega$ in [spherical coordinates](../../../calculus.md#spherical-coordinate-system) give

$$
\begin{aligned}
(u*\phi_\varepsilon)(x)
&=\int_{B(0,\varepsilon)}u(x+z)\varepsilon^{-d}\phi(z/\varepsilon)\,dz\\
&=\boxed{\int_0^1\int_{S^{d-1}}u(x+\varepsilon r\omega)\phi(r\omega)r^{d-1}\,d\omega\,dr.}
\end{aligned}
$$

The restriction $\varepsilon<\operatorname{dist}(x,\partial\Omega)$ ensures that every sampled point remains in $\Omega$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

For each $0<r<1$, the spherical [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) gives

$$
\int_{S^{d-1}}u(x+\varepsilon r\omega)\,d\omega=d\omega_d u(x).
$$

Insert this into part 1(iii). The normalization of the radial [mollifier](../../../distribution-theory.md#mollifier) is $d\omega_d\int_0^1\phi(r)r^{d-1}dr=1$, hence

$$
\boxed{(u*\phi_\varepsilon)(x)=u(x).}
$$

A convolution with a [smooth function](../../../analysis.md#smooth-function) of compact support is smooth wherever it is defined. Every point admits such an $\varepsilon$, so $u\in C^\infty(\Omega)$.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Fix $x\in\Omega'$ and $0<\rho<R(\Omega')$. Differentiate the ball mean-value formula and apply the [divergence theorem](../../../calculus.md#divergence-theorem):

$$
\partial_{x_j}u(x)
=\frac1{\omega_d\rho^d}\int_{B(x,\rho)}\partial_j u
=\frac1{\omega_d\rho^d}\int_{\partial B(x,\rho)}u\nu_j\,dS.
$$

Since $|\nu_j|\leq1$ and $|\partial B(x,\rho)|=d\omega_d\rho^{d-1}$,

$$
|\partial_{x_j}u(x)|\leq\frac d\rho\max_\Omega|u|.
$$

Letting $\rho\uparrow R(\Omega')$ and taking both maxima proves

$$
\boxed{\max_{1\leq j\leq d}\max_{\Omega'}|\partial_{x_j}u|\leq\frac d{R(\Omega')}\max_\Omega|u|.}
$$

## 2

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let the exterior ball be $B(y,R)$, tangent at $x_0$. Then $|x-y|\geq R$ on $\overline\Omega$, with equality only at $x_0$. Choose $\delta=R^{-1}$ and define

$$
w(x)=\log\frac{|x-y|}{R}.
$$

In two dimensions, $\log|x-y|$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) away from $y$, so $\Delta w=0\leq0$ in $\Omega$. Moreover $w(x_0)=0$ and $w>0$ on $\overline\Omega\setminus\{x_0\}$. Thus $w$ is a [barrier for the Dirichlet problem](../../../analysis.md#barrier-for-the-dirichlet-problem), and $\boxed{x_0\text{ is a regular boundary point}}$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) here states

$$
Lu\geq0\text{ in }\Omega\quad\Longrightarrow\quad
\max_{\overline\Omega}u\leq\max_{\partial\Omega}u
$$

for $u\in C^2(\Omega)\cap C^0(\overline\Omega)$.

To prove it, suppose the interior maximum exceeds the boundary maximum. Put $q(x)=e^{-\ell x_1}$. Since $c=0$,

$$
Lq=q(\ell^2a^{11}-\ell b^1)
\geq q\ell(\lambda\ell-|b^1|)>0.
$$

For sufficiently small $\varepsilon>0$, $u_\varepsilon=u+\varepsilon q$ still has an interior maximum. At that point its [gradient](../../../calculus.md#gradient) vanishes and its [Hessian matrix](../../../calculus.md#hessian-matrix) is negative semidefinite; ellipticity gives $Lu_\varepsilon\leq0$. But $Lu_\varepsilon=Lu+\varepsilon Lq>0$, a contradiction. This proves the principle.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

No. A positive zeroth-order coefficient can overturn the [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators). On $\Omega=(0,1)$ take

$$
L=\frac{d^2}{dx^2}+\pi^2,
\qquad
u(x)=\sin(\pi x).
$$

Then $L\nu=0$, $\nu=0$ on $\partial\Omega$, and $\nu>0$ in $\Omega$. Thus the boundary maximum is zero while the interior maximum is one. This is a counterexample satisfying uniform ellipticity and zero drift.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

If $u_1,u_2$ solve the same [Dirichlet problem](../../../analysis.md#dirichlet-problem), their difference $v=u_1-u_2$ satisfies

$$
Lv=0\text{ in }\Omega,
\qquad
v=0\text{ on }\partial\Omega.
$$

Part 2(ii) applied to $v$ gives $v\leq0$, and applied to $-v$ gives $v\geq0$. Hence $v=0$ and **the solution is unique**.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

The stated assumptions alone do not imply regularity up to the boundary: continuous boundary data need not have two Hölder derivatives. A standard sufficient set of hypotheses for the [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) is

$$
\partial\Omega\in C^{2,\alpha},\qquad
\phi\in C^{2,\alpha}(\overline\Omega),\qquad
f\in C^{0,\alpha}(\overline\Omega),
$$

with $a^{ij},b^i,c\in C^{0,\alpha}(\overline\Omega)$ and uniform ellipticity. Then the [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) gives

$$
\boxed{u\in C^{2,\alpha}(\overline\Omega)}
$$

and bounds its norm by the forcing, boundary data, and $C^0$ norm.

## 3

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Here $w$ is the [harmonic replacement](../../../partial-differential-equation.md#harmonic-replacement) of $u$ in $B_r=B(x_0,r)$, so $v=u-w\in H_0^1(B_r)$. Subtract the weak equations and test with $v$:

$$
\int_{B_r}|\nabla v|^2
=\frac12\int_{B_r}x_1^2u_{x_1}v_{x_1}+\int_{B_r}fv.
$$

Because $B_r\subset B(0,1)$, $|x_1|\leq1$. The [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) $\|v\|_6\leq C\|\nabla v\|_2$ and the [Holder inequality](../../../functional-analysis.md#holder-inequality) give

$$
\|\nabla v\|_2^2
\leq\frac12\|\nabla u\|_2\|\nabla v\|_2
+C\|f\|_{6/5}\|\nabla v\|_2.
$$

After division and squaring,

$$
\boxed{\int_{B_r}|\nabla v|^2
\leq C_1\int_{B_r}|\nabla u|^2
+C_2\left(\int_{B_r}|f|^{6/5}\right)^{5/3}.}
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

On the finite-measure ball, the [Holder inequality](../../../functional-analysis.md#holder-inequality) gives

$$
\|f\|_{L^{6/5}(B_r)}
\leq |B_r|^{1/3}\|f\|_{L^2(B_r)}.
$$

Squaring and using $|B_r|=\omega_3r^3$ yields

$$
\left(\int_{B_r}|f|^{6/5}\right)^{5/3}
\leq\omega_3^{2/3}r^2\int_{B_r}|f|^2.
$$

Since $2=1+2\alpha$ for $\alpha=1/2$, this is (6), with $\boxed{C_3=\omega_3^{2/3}}$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [Poincare-Wirtinger inequality](../../../sobolev-space.md#poincare-wirtinger-inequality) on a ball and the assumed estimate (8) imply

$$
\begin{aligned}
\int_{B(x_0,\rho)}|u-u_{B(x_0,\rho)}|^2
&\leq C\rho^2\int_{B(x_0,\rho)}|\nabla u|^2\\
&\leq CC_4\rho^{3+2\alpha}
\left(\|\nabla u\|_{L^2(B)}^2+\|f\|_{L^2(B)}^2\right).
\end{aligned}
$$

This is exactly the stated [Campanato space](../../../sobolev-space.md#campanato-space) criterion with a constant $M$ independent of the ball. Therefore

$$
\boxed{u\in C^{0,\alpha}(B).}
$$

## 4

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For $w\in X_\delta$, hypothesis (2) gives $F(w)\in C^{0,\alpha}(\overline\Omega)$. Thus $f-F(w)$ is Hölder continuous and the classical [Dirichlet problem](../../../analysis.md#dirichlet-problem) for the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) has a unique solution $u=T(w)\in C^{2,\alpha}(\overline\Omega)$. The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) gives

$$
\|T(w)\|_{C^{2,\alpha}}
\leq C\left(\|F(w)\|_{C^{0,\alpha}}+
\|f\|_{C^{0,\alpha}}+
\|T(w)\|_{C^0}+\|\phi\|_{C^{2,\alpha}}\right).
$$

The maximum estimate for the Poisson problem also gives

$$
\|T(w)\|_{C^0}\leq C\left(\|f\|_{C^0}+\|F(w)\|_{C^0}+\|\phi\|_{C^0}\right).
$$

These estimates prove that $T$ is well defined and give the requested norm control.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For $w\in X_\delta$, hypothesis (2) gives

$$
\|F(w)\|_{C^{0,\alpha}}\leq\|w\|_{C^0}^2\leq\delta^2.
$$

Combining the two estimates in part 4(i) with (5) yields

$$
\|T(w)\|_{C^{2,\alpha}}\leq C(\delta^2+\varepsilon).
$$

Choose $0<\delta<\min\{1,(2C)^{-1}\}$, so that $C\delta^2\leq\delta/2$, and then choose $\varepsilon\leq\delta/(2C)$. Uniformly for $w\in X_\delta$ we obtain $\|T(w)\|_{C^{2,\alpha}}\leq\delta$. Hence

$$
\boxed{T(X_\delta)\subseteq X_\delta.}
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

As printed, the hypotheses admit no function $F$. Take the constant function $g\equiv z$ in (2). Its Hölder seminorm vanishes, so

$$
0\leq F(z)=\|F(g)\|_{C^{0,\alpha}}\leq\|g\|_{C^0}^2=z^2.
$$

But (1) simultaneously requires $F(z)\geq|z|$. For every $0<|z|<1$, this would give $|z|\leq z^2$, which is false. Therefore **no $F\in C^\infty(\mathbb R)$ satisfies (1) and (2), and the contraction question is vacuous under the stated assumptions**. This contradiction is present in the official paper, rather than arising from the text conversion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
