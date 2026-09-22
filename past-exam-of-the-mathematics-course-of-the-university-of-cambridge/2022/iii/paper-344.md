# Paper 344

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_344.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_344.pdf)

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
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
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

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [binary fluid mixture](../../../critical-phenomenon.md#binary-fluid-mixture), the scalar [compositional order parameter](../../../critical-phenomenon.md#compositional-order-parameter) $\phi(\mathbf r)$ may be taken as the local concentration difference between its two molecular species. Its spatial integral is fixed by their separately fixed total amounts:

$$
\int_V\phi(\mathbf r)\,d\mathbf r=V\bar\phi.
$$

Locally, $\phi$ can change only through transport and therefore obeys a [continuity equation](../../../physics.md#continuity-equation). By contrast, $\mathbf p$ is the local [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) measuring the mean tail-to-head orientation of the [surfactant](../../../fluid-mechanics.md#surfactant) molecules. Individual molecules can rotate in place, so the integral of $\mathbf p$ need not be conserved.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The composition changes most rapidly across an interface, so $\nabla\phi$ points along its normal. The term

$$
\lambda\mathbf p\mathbin\cdot\nabla\phi
$$

therefore couples the surfactant's head-to-tail orientation to the interface normal. Minimization aligns $\mathbf p$ antiparallel to $\nabla\phi$ when $\lambda>0$ and parallel when $\lambda<0$. The sign is fixed by which fluid component is called positive $\phi$ and by which molecular end defines positive $\mathbf p$, together with the preferential affinity of the head and tail for the two components.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The terms involving $\mathbf p$ can be written by [completing the square](../../../polynomial.md#completing-the-square):

$$
\frac\nu2|\mathbf p|^2+\lambda\mathbf p\mathbin\cdot\nabla\phi
=\frac\nu2\left|\mathbf p+\frac\lambda\nu\nabla\phi\right|^2
-\frac{\lambda^2}{2\nu}|\nabla\phi|^2.
$$

Translation of the integration variable in the [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) over $\mathbf p$ contributes only a $\phi$-independent determinant. The effective free energy is therefore

$$
F[\phi]=\int\left[
\frac a2\phi^2+\frac b4\phi^4
+\frac{\widetilde\kappa}{2}|\nabla\phi|^2
+\frac\gamma2(\nabla^2\phi)^2
\right]d\mathbf r,
$$

where

$$
\boxed{\widetilde\kappa=\kappa-\frac{\lambda^2}{\nu}.}
$$

This is the [surfactant renormalization of the square-gradient coefficient](../../../critical-phenomenon.md#surfactant-renormalization-of-the-square-gradient-coefficient).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Surfactants accumulate at an interface and orient their two chemically distinct ends toward their preferred fluid components. The relaxation found in part c lowers the coefficient of the [gradient energy](../../../critical-phenomenon.md#gradient-energy), and hence generally lowers the [surface tension](../../../fluid-mechanics.md#surface-tension). If the reduction makes $\widetilde\kappa<0$, the positive fourth-gradient term proportional to $\gamma$ can stabilize structure at a nonzero [wavevector](../../../continuum-mechanics.md#wavevector), producing the modulated correlations characteristic of a [microemulsion](../../../critical-phenomenon.md#microemulsion).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Use $\partial_x\mapsto iq$ under the [Fourier transform](../../../analysis.md#fourier-transform) and the reality conditions $\phi(-q)=\phi(q)^*$ and $p(-q)=p(q)^*$. With $\Psi=(\phi,p)$, the quadratic free energy is

$$
F=\frac12\sum_q\Psi_i(q)G_{ij}(q)\Psi_j(-q),
$$

where

$$
\boxed{
G(q)=
\begin{pmatrix}
a+\kappa q^2+\gamma q^4&i\lambda q\\
-i\lambda q&\nu
\end{pmatrix}.}
$$

The opposite imaginary off-diagonal entries make $G(q)$ a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). Reversing the Fourier-sign convention reverses both of those signs without changing any correlator.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The covariance of a centered [multivariate Gaussian distribution](../../../probability-theory.md#multivariate-gaussian-distribution) is the inverse of its quadratic kernel. Writing $A(q)=a+\kappa q^2+\gamma q^4$, one finds

$$
G(q)^{-1}
=\frac1{\nu A(q)-\lambda^2q^2}
\begin{pmatrix}
\nu&-i\lambda q\\
i\lambda q&A(q)
\end{pmatrix}.
$$

Consequently the composition [static structure factor](../../../critical-phenomenon.md#static-structure-factor) is

$$
\boxed{\langle\phi(q)\phi(-q)\rangle
=\frac1{a+\widetilde\kappa q^2+\gamma q^4}.}
$$

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

The other diagonal entry of the same inverse gives

$$
\boxed{\langle p(q)p(-q)\rangle
=\frac{a+\kappa q^2+\gamma q^4}
{\nu\left(a+\widetilde\kappa q^2+\gamma q^4\right)}}
$$

or, more revealingly,

$$
\boxed{\langle p(q)p(-q)\rangle
=\frac1\nu+\frac{\lambda^2q^2}
{\nu^2\left(a+\widetilde\kappa q^2+\gamma q^4\right)}.}
$$

The first term is the uncoupled local orientational fluctuation. The second shows that every nonuniform composition fluctuation induces a correlated surfactant-polarization fluctuation. It vanishes at $q=0$, as the coupling contains a gradient, and is enhanced at wavevectors where the composition structure factor is large.

## 2

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A real symmetric traceless $2$ by $2$ matrix has eigenvalues $\lambda$ and $-\lambda$ and can be written

$$
Q_{ij}=2\lambda\left(n_in_j-\frac12\delta_{ij}\right)
$$

for a unit [nematic director](../../../critical-phenomenon.md#nematic-director) $\mathbf n\sim-\mathbf n$. Since $Q_{ij}Q_{ji}=2\lambda^2$, the uniform [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) is

$$
\mathbb F_{\rm bulk}=2a\lambda^2+4b\lambda^4.
$$

For $a<0<b$, its nonzero minima satisfy

$$
4a\lambda+16b\lambda^3=0,
$$

and hence

$$
\boxed{\lambda_0=\sqrt{-\frac a{4b}}.}
$$

The signs $\pm\lambda_0$ amount to exchanging the two orthogonal eigenvectors, so the chosen convention takes $\lambda_0\geq0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The bulk potential gives fluctuations in $\lambda$ a nonzero restoring force, whereas slowly rotating the [nematic director](../../../critical-phenomenon.md#nematic-director) costs only gradients. At lengths much larger than the amplitude correlation length, it is therefore the leading [gradient expansion](../../../critical-phenomenon.md#gradient-expansion) approximation to set $\lambda=\lambda_0$ while retaining $\mathbf n(\mathbf r)$.

Differentiating

$$
Q_{ij}=2\lambda_0\left(n_in_j-\frac12\delta_{ij}\right)
$$

gives

$$
\nabla_iQ_{ij}
=2\lambda_0\left[(\nabla\mathbin\cdot\mathbf n)n_j
+(\mathbf n\mathbin\cdot\nabla)n_j\right].
$$

Substitution into the elastic term yields

$$
\boxed{\mathbb F_{\rm elastic}
=2K\lambda_0^2
\left|(\nabla\mathbin\cdot\mathbf n)\mathbf n
+(\mathbf n\mathbin\cdot\nabla)\mathbf n\right|^2.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $\mathbf n=(\cos\theta,\sin\theta)=(c,s)$ with $\theta=\theta(x)$. Then

$$
(\nabla\mathbin\cdot\mathbf n)\mathbf n
+(\mathbf n\mathbin\cdot\nabla)\mathbf n
=\theta'(-2sc,c^2-s^2).
$$

The squared norm is $(\theta')^2$ because

$$
4s^2c^2+(c^2-s^2)^2=1.
$$

Thus the [one-elastic-constant nematic free energy](../../../critical-phenomenon.md#one-elastic-constant-nematic-free-energy) becomes

$$
\mathbb F_{\rm elastic}
=2K\lambda_0^2(\theta')^2
=\frac{\widetilde K}{2}(\theta')^2,
$$

with

$$
\boxed{\widetilde K=4K\lambda_0^2=-\frac{Ka}{b}.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The anchoring conditions are $\theta(0)=0$ modulo $\pi$ and $\theta(L)=\pi/2$ modulo $\pi$, since the [nematic director](../../../critical-phenomenon.md#nematic-director) identifies angles differing by $\pi$. Their difference can therefore be $m\pi/2$ for any odd integer $m$. The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) of

$$
F[\theta]=\frac{\widetilde K}{2}\int_0^L(\theta')^2dx
$$

is $\theta''=0$, so every stationary solution has the form

$$
\boxed{\theta_m(x)=\frac{m\pi x}{2L}\qquad(m\text{ odd}).}
$$

Its free energy per unit length in the $y$ direction is

$$
F_m=\frac{\widetilde K m^2\pi^2}{8L}.
$$

The smallest possible $m^2$ is one, giving exactly the two degenerate global minima $m=1$ and $m=-1$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Traverse the large rectangle counterclockwise, taking its lower edge at $y\to-\infty$ and upper edge at $y\to+\infty$. Along the lower edge the director angle changes by $-\pi/2$; along the upper edge, traversed from $x=L$ to $x=0$, it changes by another $-\pi/2$. The anchored director is constant along the two vertical edges. The net continuous angle change is therefore

$$
\Delta\theta=-\pi.
$$

The [topological charge of a two-dimensional nematic disclination](../../../critical-phenomenon.md#topological-charge-of-a-two-dimensional-nematic-disclination) enclosed by a circuit is $q=\Delta\theta/(2\pi)$, so

$$
\boxed{q_{\rm total}=-\frac12.}
$$

A nonsingular director field on the enclosed disk would have zero winding. At least one [nematic disclination](../../../critical-phenomenon.md#nematic-disclination) must therefore lie inside.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

The least costly configuration contains one charge-$-1/2$ [nematic disclination](../../../critical-phenomenon.md#nematic-disclination), placed near $(L/2,0)$ by the reflection symmetries of the boundary data. Away from its small core, the director interpolates as smoothly as possible between the wall anchoring and the two far-field textures. Locally around the defect one may sketch

$$
\theta(r,\varphi)=-\frac{\varphi}{2}+\theta_0.
$$

The elastic energy of an isolated defect scales as $q^2\log(R/a_{\rm core})$. Splitting the required total $-1/2$ charge into additional allowed half-charge defects is impossible without also adding compensating defects, which raises both the logarithmic elastic energy and the positive core energy. The single centered $-1/2$ defect is therefore the lowest-energy topology, up to smooth distortions and symmetry-related core placement.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

For general odd $m_+$ and $m_-$, the same rectangular circuit gives

$$
\Delta\theta=\frac{(m_--m_+)\pi}{2},
\qquad
q_{\rm total}=\frac{m_--m_+}{4}.
$$

Every elementary two-dimensional nematic defect has $|q|=1/2$, so the minimum number is

$$
\boxed{N_{\rm 2D}=\frac{|m_+-m_-|}{2}.}
$$

In three dimensions the director takes values in the [real projective plane](../../../differential-geometry.md#real-projective-plane), whose [fundamental group](../../../algebraic-topology.md#fundamental-group) is $\mathbb Z/2\mathbb Z$. The signs of half-charge line defects are no longer distinct topological classes, and two such lines can annihilate by [escape into the third dimension](../../../critical-phenomenon.md#escape-into-the-third-dimension). Hence only the parity of $N_{\rm 2D}$ remains:

$$
\boxed{
N_{\rm 3D}=
\begin{cases}
0,&(m_+-m_-)/2\text{ even},\\
1,&(m_+-m_-)/2\text{ odd}.
\end{cases}}
$$

When one is required, it is a disclination line extending through the unbounded $z$ direction.

## 3

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put $E(t)=-\delta A/\delta\mathbf x(t)$. For a specified forward trajectory, the equation of motion determines

$$
\mathbf f_F=E+\zeta\dot{\mathbf x},
$$

whereas its time reverse requires

$$
\mathbf f_B=E-\zeta\dot{\mathbf x}.
$$

Assume the action is invariant under [time-reversal symmetry](../../../quantum-field-theory.md#t-symmetry), the position is even and velocity is odd under time reversal, and the trajectory-to-noise Jacobian is identical in the two directions. The [Onsager--Machlup path probability](../../../critical-phenomenon.md#onsager-machlup-path-probability) is then

$$
\mathbb P_F[\mathbf x]
=\mathcal N\exp\left[-\frac1{2\sigma^2}
\int_{t_1}^{t_2}|E+\zeta\dot{\mathbf x}|^2dt\right],
$$

with $\zeta\dot{\mathbf x}$ replaced by $-\zeta\dot{\mathbf x}$ for $\mathbb P_B$. Since

$$
|E+\zeta\dot{\mathbf x}|^2-|E-\zeta\dot{\mathbf x}|^2
=4\zeta E\mathbin\cdot\dot{\mathbf x},
$$

their ratio is

$$
\boxed{\frac{\mathbb P_F}{\mathbb P_B}
=\exp\left[\frac{2\zeta}{\sigma^2}
\int_{t_1}^{t_2}
\dot{\mathbf x}\mathbin\cdot
\frac{\delta A}{\delta\mathbf x(t)}dt\right].}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [functional derivative](../../../calculus-of-variations.md#functional-derivative) of the action is

$$
\frac{\delta A}{\delta\mathbf x}
=\frac{\partial\mathcal L}{\partial\mathbf x}
-\frac d{dt}\frac{\partial\mathcal L}{\partial\dot{\mathbf x}}.
$$

For the [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function)

$$
H=\dot{\mathbf x}\mathbin\cdot
\frac{\partial\mathcal L}{\partial\dot{\mathbf x}}-\mathcal L,
$$

and a time-independent [Lagrangian](../../../calculus-of-variations.md#lagrangian),

$$
\frac{dH}{dt}
=\dot{\mathbf x}\mathbin\cdot
\left(\frac d{dt}\frac{\partial\mathcal L}{\partial\dot{\mathbf x}}
-\frac{\partial\mathcal L}{\partial\mathbf x}\right).
$$

Therefore

$$
\boxed{\dot{\mathbf x}\mathbin\cdot
\frac{\delta A}{\delta\mathbf x}=-\frac{dH}{dt}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

[Detailed balance](../../../markov-process.md#detailed-balance) says that each equilibrium transition is balanced by its time reverse:

$$
P_{\rm eq}(1)\mathbb P_F(1\to2)
=P_{\rm eq}(2)\mathbb P_B(2\to1).
$$

With the [Boltzmann distribution](../../../thermodynamics.md#boltzmann-distribution) $P_{\rm eq}\propto e^{-\beta H}$ and $\Delta H=H_2-H_1$, this requires

$$
\frac{\mathbb P_F}{\mathbb P_B}=e^{-\beta\Delta H}.
$$

Parts a and b instead give $\exp[-(2\zeta/\sigma^2)\Delta H]$. Equality for every pair of endpoints yields the [fluctuation-dissipation relation for a Langevin particle](../../../thermodynamics.md#fluctuation-dissipation-relation-for-a-langevin-particle)

$$
\boxed{\sigma^2=\frac{2\zeta}{\beta}=2\zeta k_BT.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

With an external force $\mathbf F$, the required forward and backward noise histories become

$$
\mathbf f_F=E+\zeta\dot{\mathbf x}-\mathbf F,
\qquad
\mathbf f_B=E-\zeta\dot{\mathbf x}-\mathbf F.
$$

Repeating the difference of squares and using $2\zeta/\sigma^2=\beta$ gives

$$
\boxed{\frac{\mathbb P_F}{\mathbb P_B}
=\exp\left[-\beta\Delta H
+\beta\int_{t_1}^{t_2}
\mathbf F(\mathbf x)\mathbin\cdot\dot{\mathbf x}\,dt\right].}
$$

The second term is $\beta$ times the [work](../../../classical-mechanics.md#work) performed by the external force.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics), with $\Delta Q$ defined as heat lost by the particle to the bath, is

$$
\Delta H=W-\Delta Q.
$$

Thus $W-\Delta H=\Delta Q$, and part d becomes the [local detailed balance](../../../thermodynamics.md#local-detailed-balance) identity

$$
\boxed{\frac{\mathbb P_F}{\mathbb P_B}=e^{\beta\Delta Q}.}
$$

The logarithmic path-probability ratio is the bath's [entropy production](../../../thermodynamics.md#entropy-production) $\Delta S_{\rm bath}=\Delta Q/T$ in units of $k_B$.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

If $\nabla\times\mathbf F=0$ on a simply connected region containing the bounded trajectory, then the [Poincaré lemma](../../../differential-form.md#poincare-lemma) gives a scalar potential $U$ with $\mathbf F=-\nabla U$. The work is

$$
W=\int\mathbf F\mathbin\cdot d\mathbf x
=U(\mathbf x_1)-U(\mathbf x_2),
$$

which remains bounded when $\mathbf x$ and $\mathbf F$ remain bounded. Since $H$ is also bounded, $\Delta Q=W-\Delta H$ cannot grow linearly with the observation time.

Thus sustained linear heat dissipation in this setting requires a [nonconservative force](../../../classical-mechanics.md#nonconservative-force), and, under the stated simply connectedness assumption,

$$
\boxed{\nabla\times\mathbf F\ne0.}
$$

Such a force can perform nonzero work on repeated bounded cycles. On a multiply connected domain, a curl-free force can have nonzero circulation, so the topological assumption is essential.

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

For a specified field trajectory, the required normalized noise is

$$
\boldsymbol\Lambda_F
=\frac{\dot{\mathbf p}
+\Gamma\,\delta F/\delta\mathbf p-\Gamma\mathbf Y}
{\sqrt{2k_BT\Gamma}},
$$

and time reversal changes only $\dot{\mathbf p}$ to $-\dot{\mathbf p}$. Assuming equal additive-noise Jacobians, the difference of the two [Onsager--Machlup actions](../../../critical-phenomenon.md#onsager-machlup-path-probability-for-model-a-dynamics) gives

$$
\log\frac{\mathbb P_F}{\mathbb P_B}
=-\beta\int_{t_1}^{t_2}dt\int d\mathbf r\,
\dot{\mathbf p}\mathbin\cdot
\left(\frac{\delta F}{\delta\mathbf p}-\mathbf Y\right).
$$

The [functional chain rule](../../../calculus-of-variations.md#functional-chain-rule) identifies the first term as $-\beta\Delta F$, so

$$
\boxed{\frac{\mathbb P_F[\mathbf p]}{\mathbb P_B[\mathbf p]}
=\exp\left[
-\beta\Delta F
+\beta\int_{t_1}^{t_2}dt\int d\mathbf r\,
\mathbf Y\mathbin\cdot\dot{\mathbf p}
\right].}
$$

The forcing performs generalized work $W_Y=\int\mathbf Y\cdot\dot{\mathbf p}$, and $W_Y-\Delta F$ is the heat dissipated into the bath. The formula is therefore the field-theory form of [local detailed balance](../../../thermodynamics.md#local-detailed-balance) and quantifies nonequilibrium entropy production.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
