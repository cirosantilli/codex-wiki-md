# Paper 313

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_313.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_313.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write the [scalar field](../../../quantum-field-theory.md#scalar-field) energy as $E=T+V$, where

$$
T=\frac12\int_{-\infty}^{\infty}(\phi')^2\,dx,
\qquad
V=\int_{-\infty}^{\infty}U(\phi)\,dx.
$$

Under the [Derrick scaling](../../../classical-field-theory-soliton.md#derrick-scaling) $\phi_\lambda(x)=\phi(\lambda x)$, a [change of variables](../../../calculus.md#change-of-variables-formula) gives

$$
E(\lambda)=\lambda T+\lambda^{-1}V.
$$

A finite-energy solution of the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is stationary under this admissible variation. The [Derrick virial identity](../../../classical-field-theory-soliton.md#derrick-virial-identity) is therefore

$$
0=E'(1)=T-V,
\qquad
\boxed{\frac12\int_{-\infty}^{\infty}(\phi')^2\,dx
=\int_{-\infty}^{\infty}U(\phi)\,dx}.
$$

The static field equation is $\phi''=U'(\phi)$, so integration gives

$$
U(\phi)=\frac12\phi^6-\phi^4+\frac12\phi^2+C
=\frac12\phi^2(1-\phi^2)^2+C.
$$

The polynomial before $C$ is nonnegative and vanishes, so requiring the minimum to be zero fixes $C=0$. Hence the [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) is

$$
\boxed{U^{-1}(0)=\{-1,0,1\}},
$$

which has three elements. A finite-energy [scalar-field kink](../../../classical-field-theory-soliton.md#scalar-field-kink) can join only adjacent vacua: a solution cannot cross the intermediate vacuum at finite $x$ because its first integral would have $\phi=\phi'=0$ there and the [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem) would make it constant. There are therefore four oriented topological sectors,

$$
-1\to0,\qquad0\to-1,\qquad0\to1,\qquad1\to0,
$$

comprising two increasing kinks and their two antikinks. Symmetry under $\phi\mapsto-\phi$ and spatial reflection generates all four from one profile.

For the $0\to1$ sector, completing the square gives the [Bogomolny bound](../../../quantum-field-theory.md#bogomolny-bound)

$$
\begin{aligned}
E
&=\frac12\int_{-\infty}^{\infty}
\left[\phi'-\phi(1-\phi^2)\right]^2dx
+\int_{-\infty}^{\infty}\phi'\phi(1-\phi^2)\,dx\\
&\geq\int_0^1\phi(1-\phi^2)\,d\phi.
\end{aligned}
$$

Equality holds for the [Bogomolny equation](../../../quantum-field-theory.md#bogomolny-equations)

$$
\boxed{\phi'=\phi(1-\phi^2)}.
$$

With $y=\phi^2$, this becomes the [logistic differential equation](../../../differential-equation.md#logistic-differential-equation) $y'=2y(1-y)$. Translation invariance supplies an arbitrary center $x_0$, and the explicit [kink in a phi-six model](../../../classical-field-theory-soliton.md#kink-in-a-phi-six-model) is

$$
\boxed{\phi(x)=\frac1{\sqrt{1+e^{-2(x-x_0)}}}}.
$$

It tends to $0$ and $1$ at the two spatial ends and saturates the bound. Its mass is consequently

$$
\boxed{M=\int_0^1\phi(1-\phi^2)\,d\phi=\frac14}.
$$

## 2

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Finite energy requires $|\phi|\to1$ and $D\phi\to0$ on the circle at spatial infinity. Writing $\phi\sim e^{i\chi}$ there gives $A\sim d\chi$. The [vortex number](../../../classical-field-theory-soliton.md#vortex-number) is the [winding number](../../../complex-analysis.md#winding-number)

$$
N=\frac1{2\pi}\oint_{S_\infty^1}d\chi\in\mathbb Z.
$$

By [Stokes theorem](../../../calculus.md#stokes-theorem), the [magnetic flux](../../../electromagnetism.md#magnetic-flux) is quantized:

$$
\boxed{\int_{\mathbb R^2}B\,dx^1\wedge dx^2
=\oint_{S_\infty^1}A=2\pi N}.
$$

For the rotationally symmetric [Abelian Higgs vortex](../../../classical-field-theory-soliton.md#nielsen-olesen-vortex) ansatz, $A=f(r)d\theta$ and $\phi=h(r)e^{ik\theta}$ give

$$
B=\frac{f'}r,
\qquad
|D\phi|^2=(h')^2+\frac{(k-f)^2h^2}{r^2}.
$$

After the angular integration, the [Abelian Higgs model](../../../classical-field-theory-soliton.md#abelian-higgs-model) energy becomes

$$
\mathcal E(f,h)=\pi\int_0^\infty
\left[
\frac{(f')^2}{r}+r(h')^2
+\frac{(k-f)^2h^2}{r}
+\frac r4(1-h^2)^2
\right]dr.
$$

[Completing the square](../../../polynomial.md#completing-the-square) in the two pairs of terms gives

$$
\begin{aligned}
\frac{\mathcal E}{\pi}
={}&\int_0^\infty\left[
r\left(h'-\frac{k-f}{r}h\right)^2
+\frac1r\left(f'-\frac r2(1-h^2)\right)^2
\right]dr\\
&-\left[(k-f)(1-h^2)\right]_{0}^{\infty}.
\end{aligned}
$$

Regularity at the origin and approach to the vacuum at infinity require

$$
\boxed{f(0)=0,\quad h(0)=0,\qquad
f(\infty)=k,\quad h(\infty)=1}.
$$

More precisely, $h(r)=O(r^k)$ and $f(r)=O(r^2)$ near the origin. The boundary term is $k$, so

$$
\boxed{\mathcal E\geq k\pi}.
$$

The bound is saturated exactly when both squares vanish, giving the radial [Bogomolny vortex equations](../../../classical-field-theory-soliton.md#bogomolny-vortex-equation)

$$
\boxed{
h'=\frac{k-f}{r}h,
\qquad
f'=\frac r2(1-h^2)}.
$$

The asymptotic value $f(\infty)=k$ also makes the flux $2\pi k$, so the ansatz has vortex number $N=k$.

## 3

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

On an oriented pseudo-Riemannian vector space $(\mathbb R^n,\eta,\operatorname{vol})$, the [Hodge star operator](../../../differential-form.md#hodge-star-operator) is the unique linear map

$$
*:\Lambda^p\longrightarrow\Lambda^{n-p}
$$

satisfying

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle_\eta\operatorname{vol}
$$

for all $p$-forms $\alpha,\beta$. If $s$ is the number of negative metric directions, then

$$
*^2=(-1)^{p(n-p)+s}
$$

on $p$-forms under this convention. For the two-forms in the question,

$$
\sigma\wedge\mu=(*\sigma)\wedge\mu
=\langle\mu,\sigma\rangle_\eta\operatorname{vol},
$$

whereas

$$
\sigma\wedge\mu=-\sigma\wedge(*\mu)
=-\langle\sigma,\mu\rangle_\eta\operatorname{vol}.
$$

The induced inner product is symmetric, so these expressions are negatives of one another. Hence a [self-dual differential form](../../../differential-form.md#self-dual-differential-form) and an [anti-self-dual differential form](../../../differential-form.md#anti-self-dual-differential-form) are orthogonal and

$$
\boxed{\sigma\wedge\mu=0}.
$$

Write $w=x^1+ix^2$ and $z=x^3+ix^4$. The metric is conformal to the standard Euclidean metric, and the [Hodge star on middle-degree differential forms is conformally invariant](../../../differential-form.md#hodge-star-on-middle-degree-differential-forms-is-conformally-invariant). Taking $e^{ij}=dx^i\wedge dx^j$, the three real forms are

$$
\omega_1=e^{13}-e^{24},
\qquad
\omega_2=e^{14}+e^{23},
\qquad
\omega_3=2(e^{12}+e^{34}),
$$

because $\omega_1+i\omega_2=dw\wedge dz$. For the orientation specified by  
$dw\wedge dz\wedge d\bar w\wedge d\bar z$, one has

$$
*e^{13}=-e^{24},\qquad
*e^{14}=e^{23},\qquad
*e^{12}=e^{34}.
$$

The corresponding relations for the complementary basis forms immediately give

$$
\boxed{*\omega_k=\omega_k,\qquad k=1,2,3}.
$$

Thus these forms give a real basis of the self-dual two-forms.

Let $D_\alpha=\partial_\alpha+A_\alpha$ be the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative). In these complex coordinates the [Anti-self-dual Yang-Mills equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations) are

$$
F_{wz}=0,\qquad
F_{\bar w\bar z}=0,\qquad
F_{w\bar w}+F_{z\bar z}=0.
$$

Introduce the [spectral parameter](../../../integrable-systems.md#spectral-parameter) $\lambda$ and the linear operators

$$
L(\lambda)=D_w-\lambda D_{\bar z},
\qquad
M(\lambda)=D_z+\lambda D_{\bar w}.
$$

Their commutator is

$$
[L,M]
=F_{wz}
+\lambda(F_{w\bar w}+F_{z\bar z})
+\lambda^2F_{\bar w\bar z}.
$$

Therefore the [Lax pair for the anti-self-dual Yang-Mills equations](../../../integrable-systems.md#lax-pair-for-the-anti-self-dual-yang-mills-equations)

$$
L(\lambda)\Psi=0,\qquad M(\lambda)\Psi=0
$$

is compatible for every $\lambda$ exactly when the ASDYM equations hold.

In particular, $F_{wz}=0$ says that the connection restricted to each $(w,z)$ surface is a [flat connection](../../../relativistic-quantum-field.md#flat-connection). On a simply connected coordinate patch, the compatible equations

$$
(\partial_w+A_w)g=0,
\qquad
(\partial_z+A_z)g=0
$$

have an invertible solution $g$. Applying the associated [gauge transformation](../../../electromagnetism.md#gauge-transformation) sets

$$
\boxed{A_w=A_z=0}.
$$

This conclusion is local; global topology can obstruct a single such gauge over the whole space.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
