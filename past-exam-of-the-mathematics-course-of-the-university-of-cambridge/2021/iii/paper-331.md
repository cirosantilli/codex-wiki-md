# Paper 331

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_331.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_331.pdf)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
- [2](#2)
  - [i](#2/i)
    - [a](#2/i/a)
      - [Solution](#2/i/a/solution)
    - [b](#2/i/b)
      - [Solution](#2/i/b/solution)
    - [c](#2/i/c)
      - [Solution](#2/i/c/solution)
  - [ii](#2/ii)
    - [a](#2/ii/a)
      - [Solution](#2/ii/a/solution)
    - [b](#2/ii/b)
      - [Solution](#2/ii/b/solution)
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

## 1

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

With $\mathbf u_0=0$ and $\theta_0=-z$, the [incompressibility condition](../../../fluid-mechanics.md#incompressible-flow) and temperature equation hold because $\nabla^2z=0$. The momentum equation is satisfied by the [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure)

$$
p_0=-\frac12\sigma Ra\,z^2+\text{constant},
$$

because $\nabla p_0=\sigma Ra\,\theta_0\widehat{\mathbf z}$. Thus this is the conductive basic state.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $\mathbf u=\mathbf u'$ and $\theta=-z+\theta'$. Dropping quadratic perturbation terms gives the [Linearized Boussinesq equations](../../../geophysical-fluid-dynamics.md#linearized-boussinesq-equations)

$$
\partial_t\mathbf u'+\lambda\widehat{\mathbf z}\times\mathbf u'+\nabla p'
=\sigma Ra\,\theta'\widehat{\mathbf z}+\sigma\nabla^2\mathbf u',
\qquad
\nabla\mathbin\cdot\mathbf u'=0,
$$

and

$$
\partial_t\theta'-W=\nabla^2\theta',
\qquad W=\mathbf u'\mathbin\cdot\widehat{\mathbf z}.
$$

The fixed temperatures give $\theta'=0$ at $z=0,1$. Impermeable [stress-free boundary conditions](../../../viscous-fluid-flow.md#stress-free-boundary-condition) give

$$
\boxed{W=D^2W=0,
\qquad
D\omega=0,
\qquad
\omega=\widehat{\mathbf z}\mathbin\cdot\nabla\times\mathbf u'.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Apply $\widehat{\mathbf z}\mathbin\cdot\nabla\times$ to the linear momentum equation. The pressure and buoyancy terms vanish, while incompressibility gives $\widehat{\mathbf z}\cdot\nabla\times(\widehat{\mathbf z}\times\mathbf u')=-D W$. Hence

$$
\boxed{(\partial_t-\sigma\nabla^2)\omega-\lambda DW=0}.
$$

Applying $\widehat{\mathbf z}\cdot\nabla\times\nabla\times$ and using the identity supplied in the question gives

$$
\boxed{
(\partial_t-\sigma\nabla^2)\nabla^2W
+\lambda D\omega
=\sigma Ra\,\nabla_H^2\theta'}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For a [normal mode](../../../wave-equation.md#normal-mode) proportional to $e^{\mu t+ikx}$, put $\widehat D^2=D^2-k^2$. The three scalar equations become

$$
(\mu-\sigma\widehat D^2)\widehat\omega-\lambda D\widehat W=0,
$$



$$
(\mu-\sigma\widehat D^2)\widehat D^2\widehat W
+\lambda D\widehat\omega=-\sigma Ra\,k^2\widehat\theta,
$$

and

$$
(\mu-\widehat D^2)\widehat\theta=\widehat W.
$$

Multiplying through by the two scalar operators and eliminating $\widehat\omega,\widehat\theta$ yields

$$
\boxed{
\left[(\mu-\widehat D^2)(\mu-\sigma\widehat D^2)^2\widehat D^2
+\lambda^2D^2(\mu-\widehat D^2)
+\sigma Ra\,k^2(\mu-\sigma\widehat D^2)\right]\widehat W=0}.
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

At stationary onset, $\mu=0$. The lowest stress-free vertical mode is $\widehat W=\sin\pi z$, for which $D^2=-\pi^2$ and $\widehat D^2=-(\pi^2+k^2)$. Substitution gives

$$
\boxed{
Ra(k)=\frac{(\pi^2+k^2)^3+\pi^2(\lambda/\sigma)^2}{k^2}}.
$$

The rotation term is positive, so rotation raises the critical Rayleigh number and is stabilizing.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Put $x=k^2$ and $T=\lambda/\sigma$. Differentiating $Ra$ gives the exact stationarity equation

$$
(\pi^2+x)^2(2x-\pi^2)=\pi^2T^2.
$$

When $T\gg1$, the optimum has $x\gg\pi^2$, so $2x^3\sim\pi^2T^2$. Therefore

$$
\boxed{k\sim\left(\frac{\pi^2}{2}\right)^{1/6}
\left(\frac\lambda\sigma\right)^{1/3}}.
$$

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

Let $r=Ra-Ra_c$. The [amplitude equation](../../../dynamical-systems.md#amplitude-equation) is $\dot A=A(r-A^2)$. For $r<0$, $A=0$ is the sole equilibrium and every solution tends monotonically to it. At $r=0$, the origin remains attracting but only algebraically. For $r>0$, the origin is unstable and the two equilibria

$$
A_\pm=\pm\sqrt r
$$

are stable: positive initial data tend to $A_+$, negative initial data tend to $A_-$, and $A(0)=0$ remains zero. A plot of $A(t)$ therefore shows a [pitchfork bifurcation normal form](../../../dynamical-systems.md#pitchfork-bifurcation-normal-form) at $Ra=Ra_c$.

## 2

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/a">a</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/a/solution">Solution</h5>

↑ **Parent:** [A](#2/i/a)

The linearized vorticity equation for a [inviscid parallel shear flow](../../../hydrodynamic-stability.md#inviscid-parallel-shear-flow) is

$$
(\partial_t+U\partial_x)\nabla^2\psi-U''\partial_x\psi=0.
$$

Substituting $\psi=\phi(y)e^{ik(x-ct)}$ gives [Rayleigh's equation](../../../hydrodynamic-stability.md#rayleigh-equation-for-inviscid-shear-flow)

$$
\boxed{(U-c)(\phi''-k^2\phi)-U''\phi=0}.
$$

<h4 id="2/i/b">b</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/b/solution">Solution</h5>

↑ **Parent:** [B](#2/i/b)

No normal flow at a rigid wall gives $\boxed{\phi(\pm1)=0}$. At a free surface $y=1+\eta$, the linearized [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) is

$$
(\partial_t+U\partial_x)\eta=v=-\partial_x\psi,
$$

so $(U-c)\eta=-\phi$. The linearized tangential momentum equation gives the pressure amplitude $p=(U-c)\phi'-U'\phi$. Constant surface pressure therefore requires

$$
\boxed{(U-c)\phi'-U'\phi=0}.
$$

<h4 id="2/i/c">c</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/c/solution">Solution</h5>

↑ **Parent:** [C](#2/i/c)

For $U=y$, Rayleigh's equation reduces to $\phi''-k^2\phi=0$, so $\phi=A\cosh ky+B\sinh ky$. Applying the free-surface condition at $y=\pm1$ and setting the determinant to zero gives

$$
\boxed{c^2=\frac{(k\tanh k-1)(k-\tanh k)}{k^2\tanh k}}.
$$

For $k>0$, $k-\tanh k>0$, so instability occurs exactly when $c^2<0$, or

$$
k\tanh k<1.
$$

Thus $0<k<k_c$, where the unique positive cutoff satisfies $\boxed{k_c\tanh k_c=1}$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/a">a</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#2/ii/a)

Linearization about zero and expansion in the [Fourier sine series](../../../fourier-series.md#fourier-sine-series) give, for the $n$th mode,

$$
\ddot q_n+\left(f'(0)+\frac{n^2}{R}\right)q_n=0.
$$

Every mode is oscillatory exactly when the smallest coefficient, at $n=1$, is nonnegative. Since $f'(0)<0$,

$$
\boxed{R\leq R_c=-\frac1{f'(0)}}.
$$

<h4 id="2/ii/b">b</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#2/ii/b)

Write $T=\varepsilon t$ and expand

$$
\frac1R=\frac1{R_c+\varepsilon^2}
=-f'(0)-\varepsilon^2f'(0)^2+O(\varepsilon^4).
$$

At order $\varepsilon^2$, the assumptions $f''(0)=0$ and the orthogonality normalization leave a homogeneous equation for $u_2$ with no forcing, hence $\boxed{u_2=0}$.

At order $\varepsilon^3$, project the equation onto the null mode $\sin z$. Since

$$
\frac{\int_0^\pi\sin^4z\,dz}{\int_0^\pi\sin^2z\,dz}=\frac34,
$$

the [Fredholm solvability condition](../../../analysis.md#fredholm-solvability-condition) obtained directly from the definitions printed in the question is

$$
\boxed{
\frac{d^2A}{dT^2}
=f'(0)^2A-\frac18f'''(0)A^3}.
$$

The paper asks for $A/f'(0)^2$ in place of $f'(0)^2A$, but that coefficient is incompatible with $R_c=-1/f'(0)$ and $\varepsilon^2=R-R_c$: differentiating $1/R$ at $R_c$ gives $-1/R_c^2=-f'(0)^2$. Thus the displayed target appears to contain a reciprocal typo. It would agree with the expansion only under a correspondingly rescaled definition of the small parameter.

The imposed orthogonality of every $u_j$, $j\geq2$, removes the freedom to transfer a multiple of $\sin z$ between $A$ and the higher-order terms.

## 3

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The eigenvalues of $L$ are

$$
s_\pm=-\varepsilon\pm\sqrt{\beta^2-1}.
$$

Since $\beta<1$, the origin is linearly stable exactly when the determinant is positive:

$$
\boxed{1+\varepsilon^2-\beta^2>0},
$$

or $|\beta|<\sqrt{1+\varepsilon^2}$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Direct multiplication shows $LL^t\ne L^tL$ for $\beta\ne0$, so $L$ is a [non-normal matrix](../../../linear-operator-theory.md#non-normal-matrix). Meanwhile

$$
\dot E=2(x,y)\frac{L+L^t}{2}\binom xy
=-2\varepsilon(x^2+y^2)-4\beta xy.
$$

The symmetric part has eigenvalues $-\varepsilon\pm|\beta|$, so instantaneous growth is possible exactly when $|\beta|>\varepsilon$. Under the intended $0\leq\beta<1$ regime this is $\boxed{\beta>\varepsilon}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $\varepsilon=0$, $L^2=-(1-\beta^2)I=-\Gamma^2I$. The [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) therefore gives

$$
\boxed{
e^{Lt}=I\cos\Gamma t+\frac L\Gamma\sin\Gamma t
=\begin{pmatrix}
\cos\Gamma t&-(1+\beta)\sin\Gamma t/\Gamma\\
\Gamma\sin\Gamma t/(1+\beta)&\cos\Gamma t
\end{pmatrix}}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The maximum of $E(t)/E(0)$ is the square of the largest [singular value](../../../linear-algebra.md#singular-value) of $A(t)$, hence the largest eigenvalue $\lambda$ of $A(t)^tA(t)$. Its determinant is one and its trace gives

$$
\boxed{(\lambda-1)^2
=\frac{4\beta^2}{1-\beta^2}\lambda\sin^2\Gamma t}.
$$

For $0<\beta<1$, this is largest when $|\sin\Gamma t|=1$, namely $\Gamma t=\pi/2$ modulo $\pi$. Then

$$
\boxed{\lambda_{\max}=\frac{1+\beta}{1-\beta}}.
$$

At such a time $A(t)$ is off diagonal, and the maximizing initial condition is $\boxed{x(0)=0}$ with $y(0)\ne0$. For negative $\beta$, the axes interchange and the formula uses $|\beta|$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

When $\varepsilon=0$, trajectories conserve

$$
(1-\beta)x^2+(1+\beta)y^2,
$$

so they are closed ellipses around the origin. Ordinary energy measures circular radius rather than this conserved elliptical radius. Starting on the short-energy axis and rotating to the long-energy axis produces the transient amplification from part d; the state later returns, so the growth is transient despite neutral eigenvalues.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
