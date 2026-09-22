# Paper 4

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2026/Paperib_4_2026.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2026/Paperib_4_2026.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3G](#3g)
  - [Solution](#3g/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
- [6C](#6c)
  - [Solution](#6c/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8G](#8g)
  - [Solution](#8g/solution)
- [9E](#9e)
  - [Solution](#9e/solution)
- [10F](#10f)
  - [Solution](#10f/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12C](#12c)
  - [Solution](#12c/solution)
- [13B](#13b)
  - [Solution](#13b/solution)
- [14A](#14a)
  - [Solution](#14a/solution)
- [15B](#15b)
  - [Solution](#15b/solution)
- [16A](#16a)
  - [Solution](#16a/solution)
- [17H](#17h)
  - [Solution](#17h/solution)
- [18H](#18h)
  - [Solution](#18h/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

$|V|=p^n$. An ordered [basis](../../../vector-space.md#basis) is chosen successively in $(p^n-1)(p^n-p)\cdots(p^n-p^{n-1})$ ways, which also counts bijective endomorphisms. Counting ordered independent $k$-tuples and dividing by the number of [bases](../../../vector-space.md#basis) of $\mathbb F_p^k$ gives the Gaussian binomial $\prod_{i=0}^{k-1}(p^n-p^i)/(p^k-p^i)$.

## 2F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

The stated $d$ is a metric; the triangle inequality follows by routing through $x_0$, with equality in the only nontrivial case. Star-shaped sets are path-connected by joining each point to $x_0$. Along each radial segment, the fundamental theorem and $\|Df\|\le M$ give $\|f(x)-f(x_0)\|\le M\|x-x_0\|$; adding the two bounds proves the $Md(x,y)$ estimate. If $Df=0$, both radial differences vanish, so $f$ is constant.

## 3G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3g/solution">Solution</h3>

↑ **Parent:** [3G](#3g)

The argument principle says $(2\pi i)^{-1}\int_\gamma f\prime/f$ equals zeros minus poles. Applying it to the homotopy $f+tg$ proves Rouché when $|g|\lt |f|$ on the boundary. On $|z|=1$, $15z$ dominates $z^6+1$, so there is one zero inside; on $|z|=2$, $z^6$ dominates $15z+1$, so there are six. Hence the annulus contains five. For the [limit](../../../calculus.md#limit-of-a-function) theorem, if nonconstant $f$ took the same value at two points, use disjoint small circles and Rouché on $f_n-f_n(a)$ to force a second preimage, contradicting injectivity.

## 4B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

Direct [differentiation](../../../calculus.md#differentiation) verifies the free-particle [Schrödinger equation](../../../physics.md#schrodinger-equation), so $V=0$. At $t=0$, normalisation of $Ae^{-x^2/2}$ gives $A=\pi^{-1/4}$. Symmetry gives $\langle x\rangle=0$, while Gaussian integration gives

$$
\Delta x=\sqrt{\frac{1+(\hbar t/m)^2}{2}}.
$$

Its growth shows wave-packet spreading and therefore a nonstationary state.

## 5D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

The dispersion relation is $\omega=ck$. At a perfect conductor the tangential [electric field](../../../electromagnetism.md#electric-field) and normal [magnetic field](../../../electromagnetism.md#magnetic-field) vanish. Thus $E_{ref}=-E_0\hat x e^{i(-kz+\omega t)}$ and $B_{ref}=-E_0\hat y e^{i(-kz+\omega t)}/c$. At the surface the [magnetic field](../../../electromagnetism.md#magnetic-field) is $-2E_0\hat y/c$, so with outward normal $\hat z$ the surface current is $K=2E_0\hat x/(\mu_0c)$ (real parts understood).

## 6C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6c/solution">Solution</h3>

↑ **Parent:** [6C](#6c)

A [Givens rotation](../../../numerical-analysis.md#givens-rotation) is identity except for a $2\times2$ block $\begin{pmatrix}c&s\\-s&c\end{pmatrix}$ in rows $p,q$. Choose $p=j,q=i$ and $c=a_{jj}/r$, $s=a_{ij}/r$, $r=(a_{jj}^2+a_{ij}^2)^{1/2}$, with sign adjusted to the block convention; this mixes only those rows and zeros $a_{ij}$. For $3\times3$, successively apply rotations $(1,2)$, $(1,3)$, $(2,3)$, producing patterns $***;0**;***$, then $***;0**;0**$, then an upper triangular $R$. The product of transposed rotations is $Q$.

## 7H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

The transition [matrix](../../../vector-space.md#matrix) is symmetric with stationary projector $J/m$ and one other [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda=1-\alpha m/(m-1)$. Therefore, starting at BBC1, the probability of BBC2 after $60$ steps is $[1-\lambda^{60}]/m$.

## 8G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8g/solution">Solution</h3>

↑ **Parent:** [8G](#8g)

For $Av=\lambda v$, $v^*Av=\lambda v^*v$ is real, so $\lambda$ is real. The spectral theorem writes positive definite $C=U\operatorname{diag}(\lambda_i)U^*$; taking positive square roots gives $B$. For $H$, [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1,3$ with normalized [eigenvectors](../../../linear-operator-theory.md#eigenvector) $( -i,1)/\sqrt2$ and $(i,1)/\sqrt2$, so these columns form a suitable $U$. Finally expand $v$ in an orthonormal eigenbasis: the Rayleigh quotient is a weighted average of [eigenvalues](../../../linear-operator-theory.md#eigenvalue), bounded above by $\lambda_{max}$ and attaining it on a top [eigenvector](../../../linear-operator-theory.md#eigenvector).

## 9E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9e/solution">Solution</h3>

↑ **Parent:** [9E](#9e)

Noetherian means every [ideal](../../../commutative-algebra.md#ideal) is finitely generated, equivalently every ascending [ideal](../../../commutative-algebra.md#ideal) chain stabilises. Quotients preserve this; for example $\mathbb Z[\sqrt{-5}]$ is Noetherian as a quotient of $\mathbb Z[X]$ but not a UFD. A UFD need not be Noetherian (a [polynomial](../../../polynomial.md) [ring](../../../commutative-algebra.md#ring) in infinitely many variables is a counterexample). Stabilisation of kernels proves every surjective endomorphism of a [Noetherian ring](../../../algebra.md#noetherian-ring) injective. The shift $k[x_1,x_2,\ldots]\to k[x_1,x_2,\ldots]$, $x_1\mapsto0$, $x_{i+1}\mapsto x_i$, is surjective noninjective; $x\mapsto x^2$ on $k[x]$ shows injective need not mean surjective. Finally $f_n(X)=\binom Xn$ is integer-valued. Finite differences prove uniquely that every integer-valued [polynomial](../../../polynomial.md) is an [integral](../../../calculus.md#integral) linear combination of the $f_n$, so they are a $\mathbb Z$-basis. Int$(\mathbb Z)$ is not Noetherian: the denominators in $f_p$ yield an [ideal](../../../commutative-algebra.md#ideal) chain requiring new prime denominators.

## 10F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10f/solution">Solution</h3>

↑ **Parent:** [10F](#10f)

Bounded means finite diameter; sequential compactness means every [sequence](../../../real-analysis.md#sequence) has a convergent subsequence. A failure of uniform continuity supplies two close [sequences](../../../real-analysis.md#sequence) whose image distances stay apart; a convergent subsequence contradicts continuity. Into a discrete metric, continuity is local constancy, and compactness upgrades the radii uniformly. The Cantor set is closed in compact $[0,1]$, hence sequentially compact. Uniform local constancy gives a positive separation scale, so finitely many initial Cantor-code (binary) digits determine $f$. Removing zero destroys compactness: the hinted [function](../../../function.md) reading the digit after the first $1$ is continuous at every remaining [sequence](../../../real-analysis.md#sequence) but depends on arbitrarily late digits.

## 11F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

$P$ is a square with two open square holes; its boundary is the three square boundary curves. Using their twelve corners gives a triangulation with $V=12,E=27,F=14$. Doubling two compact connected copies along their common boundary is compact and connected, and boundary half-discs glue to discs, so the double is locally Euclidean and is a closed surface. Under the quotient the doubled triangulation has $V=12,E=42,F=28$, hence $\chi=-2$. The classification theorem says a connected compact orientable surface is a sphere or a connected sum of $k$ tori with $\chi=2-2k$; thus $k=2$.

## 12C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12c/solution">Solution</h3>

↑ **Parent:** [12C](#12c)

$Y(s)=\int_0^\infty e^{-st}y(t)dt$, with transforms $sY-y(0)$ and $s^2Y-sy(0)-\dot y(0)$; $e^{\lambda t}$ transforms to $(s-\lambda)^{-1}$ and $\delta$ to $1$. Algebra gives $Y=G H$ with $H=F+(s+2\gamma)y(0)+\dot y(0)$, so $y=g*h$. Writing $a=\sqrt{|\gamma^2-\omega^2|}$ gives $g=e^{-\gamma t}\sinh(at)/a$ for $\gamma\gt \omega$, $e^{-\gamma t}\sin(at)/a$ for $\gamma\lt \omega$, and $te^{-\gamma t}$ at equality. If $y(0)=0$, $h=f+\dot y(0)\delta$, so the initial [velocity](../../../classical-mechanics.md#velocity) contributes $\dot y(0)g(t)$.

## 13B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="13b/solution">Solution</h3>

↑ **Parent:** [13B](#13b)

Twice integrating by parts, with both endpoint variations fixed, gives $g_x-d(g_{\dot x})/dt+d^2(g_{\ddot x})/dt^2=0$. In the given [integral](../../../calculus.md#integral) the mixed $\dot x\ddot x$ term is a boundary term, and the equation is $(D^2-4)^2x=0$. Decay removes the growing solutions, so $x=(A+Bt)e^{-2t}$. The initial data give $A=1,B=3$, hence $x=(1+3t)e^{-2t}$.

## 14A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="14a/solution">Solution</h3>

↑ **Parent:** [14A](#14a)

Characteristics satisfy $\dot x=a$, $\dot y=b$, $\dot u=c$, with data prescribed on a transverse curve. If $(a,b)=(H_y,-H_x)$ then $dH/dt=H_xH_y-H_yH_x=0$. For the displayed field the divergence is zero and one may take $H=xy^2-x^3/3$. Thus characteristics are its level curves (a cubic foliation), and because $c=0$ the general solution is $u(x,y)=F(xy^2-x^3/3)$ for arbitrary [differentiable](../../../analysis.md#differentiable-function) $F$.

## 15B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="15b/solution">Solution</h3>

↑ **Parent:** [15B](#15b)

$\rho=|\psi|^2$ and $j=(\hbar/m)\operatorname{Im}(\psi^*\psi_x)$. Schrödinger’s equation and its conjugate give $\rho_t+j_x=0$; a [stationary state](../../../quantum-mechanics.md#stationary-state) has $j_x=0$. Continuity of $\psi,\psi\prime$ at $0,a$ and matching plane waves give

$$
T=\frac1{1+\frac13\sin^2(a\sqrt{3mU_0}/\hbar)},
$$

so $F=1/3$ and $G=a\sqrt{3m}/\hbar$. Transmission is minimised when $G\sqrt{U_0}=\pi/2+n\pi$, i.e. $U_0=(\pi/2+n\pi)^2/G^2$.

## 16A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="16a/solution">Solution</h3>

↑ **Parent:** [16A](#16a)

Vertical hydrostatic balance gives $p=\rho g(h-z)$; depth-independent horizontal [momentum](../../../classical-mechanics.md#momentum) and depth-integrated incompressibility yield the two shallow-water equations. Curling [momentum](../../../classical-mechanics.md#momentum) and combining with mass conservation gives $D[(\zeta+f)/h]/Dt=0$. Dot [momentum](../../../classical-mechanics.md#momentum) with $\rho h u$ and use continuity to obtain $E_t+\nabla\cdot J=0$ with $E=\rho h|u|^2/2+\rho gh^2/2$ and $J=u(E+\rho gh^2/2)$. It is kinetic plus gravitational [potential energy](../../../classical-mechanics.md#potential-energy). A no-normal-flow boundary kills the flux and conserves its [integral](../../../calculus.md#integral); a localized nonuniform height has excess positive energy relative to the uniform rest state with the same mass, so it cannot decay to that state without dissipation.

## 17H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="17h/solution">Solution</h3>

↑ **Parent:** [17H](#17h)

The MLE is $\hat\theta=n/S$, $S=\sum X_i$. Since $S\sim\Gamma(n,\theta)$, $\theta S\sim\Gamma(n,1)$ (in general $\gamma Y\sim\Gamma(\beta,\lambda/\gamma)$). If $q_r$ is the $r$-quantile of $\Gamma(n,1)$, a central confidence interval is $[(q_{\alpha/2}/n)\hat\theta,(q_{1-\alpha/2}/n)\hat\theta]$. A $\Gamma(\beta,\lambda)$ prior yields posterior $\Gamma(\beta+n,\lambda+S)$ and mean $\tilde\theta=(\beta+n)/(\lambda+S)$. With $q_r\prime$ the quantiles of $\Gamma(\beta+n,1)$, take $l\prime=q_{\alpha/2}\prime/(\beta+n)$ and $u\prime=q_{1-\alpha/2}\prime/(\beta+n)$.

## 18H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="18h/solution">Solution</h3>

↑ **Parent:** [18H](#18h)

An extreme point is not a nontrivial convex combination of two distinct points of the set. Write $x=x^+-x^-$ with nonnegative parts and set $y=(x^+,x^-)$, $c=(1,1)$, $M=(A,-A)$, $a=b$. An extreme feasible point of this standard-form LP has at most $m$ positive coordinates (otherwise the corresponding columns are dependent and permit a two-sided feasible perturbation); an optimum may be chosen extreme, and cancelling simultaneous positive pairs gives an $x$ with at most $m$ nonzeros. For the final problem, fix $b=Ax^*$ for any optimum and replace $x^*$ by such a sparse minimum-$\ell^1$ solution of $Ax=b$; $f(Ax)$ is unchanged and the penalty cannot increase.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
