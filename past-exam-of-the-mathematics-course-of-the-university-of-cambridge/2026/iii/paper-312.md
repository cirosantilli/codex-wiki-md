# Paper 312

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20312.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20312.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $\phi=\bar\phi+\varphi$ and evaluate derivatives of $P$ on the homogeneous background

$$
\bar X=\frac{\bar\phi'^2}{2a^2}.
$$

The first- and second-order changes in $X$ are

$$
\delta_1X=\frac{\bar\phi'\varphi'}{a^2},
\qquad
\delta_2X=\frac{\varphi'^2-(\nabla\varphi)^2}{2a^2}.
$$

After using the background equation to remove the linear action, the quadratic action of the [P(X, phi) scalar field theory](../../../cosmology.md#p-x-phi-scalar-field-theory) is

$$
S_2=\frac12\int d\tau\,d^3x\left\lbrace
a^2A\varphi'^2-a^2P_X(\nabla\varphi)^2
+2a^2P_{X\phi}\bar\phi'\varphi\varphi'
+a^4P_{\phi\phi}\varphi^2\right\rbrace,
$$

where

$$
A=P_X+2\bar XP_{XX}.
$$

Varying gives

$$
(a^2A\varphi')'-a^2P_X\nabla^2\varphi
+\left[(a^2P_{X\phi}\bar\phi')'-a^4P_{\phi\phi}\right]\varphi=0.
$$

The [Sound speed of a P(X, phi) scalar perturbation](../../../cosmology.md#sound-speed-of-a-p-x-phi-scalar-perturbation) is

$$
\boxed{c_s^2=\frac{P_X}{P_X+2\bar XP_{XX}}=\frac{P_X}{A}}.
$$

At leading slow variation, take $H$, $c_s$, and the kinetic coefficients as nearly constant and neglect the effective mass and their logarithmic derivatives. The Fourier equation then becomes

$$
\varphi_k''+2\frac{a'}a\varphi_k'+c_s^2k^2\varphi_k=0.
$$

For $u_k=a\varphi_k$ and [de Sitter spacetime](../../../general-relativity.md#de-sitter-spacetime) $a''/a=2/\tau^2$, this is

$$
u_k''+\left(c_s^2k^2-\frac2{\tau^2}\right)u_k=0.
$$

Two independent solutions are

$$
u_k^{\pm}=\left(1\pm\frac{i}{c_sk\tau}\right)e^{\pm ic_sk\tau}.
$$

The [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum) selects the positive-frequency behavior $e^{-ic_sk\tau}$ as $-c_sk\tau\to\infty$. Canonical normalization of $v=a\sqrt A\,\varphi$ gives the general amplitude; with the field normalization $P_X\simeq1$, so $A\simeq c_s^{-2}$, it reduces, up to an overall phase, to

$$
\boxed{\varphi_k(\tau)=
\frac{H}{\sqrt{2c_sk^3}}
(1+ic_sk\tau)e^{-ic_sk\tau}}.
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

At cubic order, the expansion of $P(X,\phi)$ produces the schematic operators

$$
\varphi'^3,quad
\varphi'(\nabla\varphi)^2,quad
\varphi\varphi'^2,quad
\varphi(\nabla\varphi)^2,quad
\varphi^2\varphi',quad
\varphi^3.
$$

The derivative self-interactions involving $P_{XX}$ and $P_{XXX}$ are generally largest when $c_s\ll1$, while coefficients containing explicit $\phi$ derivatives of a slowly varying $P$ are commonly slow-variation suppressed. The former therefore tend to dominate [primordial non-Gaussianity](../../../cosmology.md#primordial-non-gaussianity).

The terms contributing to $\varphi\varphi'^2$ are

$$
a^4P_{X\phi}\varphi\,\delta_2X
+\frac{a^4}{2}P_{XX\phi}\varphi(\delta_1X)^2.
$$

Thus

$$
S_3\supset\int d\tau\,d^3x\,a^2\lambda_0
\varphi\varphi'^2,
\qquad
\boxed{\lambda_0=\frac12(P_{X\phi}+2\bar XP_{XX\phi})}.
$$

Equivalently, if the complete time-dependent coefficient is called $\lambda$, then $\lambda(\tau)=a^2\lambda_0$.

Treat $\lambda_0$ as constant at leading slow variation. To cubic order the corresponding [interaction Hamiltonian](../../../quantum-field-theory.md#interaction-hamiltonian) is

$$
H_I=-a^2\lambda_0
\int_{\mathbf p_1\mathbf p_2\mathbf p_3}
(2\pi)^3\delta^{(3)}(\mathbf p_1+\mathbf p_2+\mathbf p_3)
\varphi_{\mathbf p_1}\varphi'_{\mathbf p_2}\varphi'_{\mathbf p_3}.
$$

For $q_i=c_sk_i$, the mode function above satisfies

$$
\varphi_k(0)=A_k,
\qquad
\varphi_k^{*\prime}(\tau)=A_kq_k^2\tau e^{iq_k\tau},
\qquad
A_k=\frac{H}{\sqrt{2c_sk^3}}.
$$

Writing $K=k_1+k_2+k_3$, the needed regulated integral is

$$
\int_{-\infty(1-i\epsilon)}^0
(1-iq_i\tau)e^{ic_sK\tau}\,d\tau
=-\frac{i}{c_s}\left(\frac1K+\frac{k_i}{K^2}\right).
$$

There are three choices for the undifferentiated leg and two contractions interchanging the differentiated legs. The stated [in-in formalism](../../../quantum-field-theory.md#keldysh-formalism) formula therefore gives

$$
\langle\varphi_{\mathbf k_1}\varphi_{\mathbf k_2}\varphi_{\mathbf k_3}\rangle
=(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)
B_\lambda(k_1,k_2,k_3),
$$

with

$$
\boxed{
B_\lambda
=\frac{\lambda_0H^4}{2(k_1k_2k_3)^3}
\sum_{\mathrm{cyc}}
k_j^2k_l^2
\left(\frac1K+\frac{k_i}{K^2}\right)}.
$$

The powers of $c_s$ cancel for this vertex with the normalization specified in part (i). Reversing the convention for the sign of $H_I$ reverses the displayed overall sign but not the momentum shape of the [primordial bispectrum](../../../cosmology.md#primordial-bispectrum).

## 2

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use the Fourier convention $f(\mathbf x)=\int_{\mathbf k}f(\mathbf k)e^{i\mathbf k\cdot\mathbf x}$ with $\int_{\mathbf k}=\int d^3k/(2\pi)^3$. Neglect [anisotropic stress](../../../linear-cosmological-perturbation-theory.md#scalar-anisotropic-stress) and assume the pressureless velocity is irrotational, so

$$
\mathbf v(\mathbf k)=-i\frac{\mathbf k}{k^2}\theta(\mathbf k).
$$

Fourier transforming $\nabla\mathbin\cdot(\delta\mathbf v)$ in the nonlinear continuity equation gives

$$
\delta'(\mathbf k)+\theta(\mathbf k)
=-\int_{\mathbf k_1\mathbf k_2}
(2\pi)^3\delta_D(\mathbf k_1+\mathbf k_2-\mathbf k)
\alpha(\mathbf k_1,\mathbf k_2)
\theta(\mathbf k_1)\delta(\mathbf k_2),
$$

where the [alpha mode-coupling kernel](../../../large-scale-structure-of-the-universe.md#alpha-mode-coupling-kernel) and its symmetrization are

$$
\alpha(\mathbf k_1,\mathbf k_2)
=\frac{(\mathbf k_1+\mathbf k_2)\cdot\mathbf k_1}{k_1^2},
$$



$$
\boxed{\alpha_s
=1+\frac{\mathbf k_1\cdot\mathbf k_2}{2}
\left(\frac1{k_1^2}+\frac1{k_2^2}\right)}.
$$

Taking the divergence of the Euler equation gives

$$
\theta'+\mathcal H\theta+\frac32\mathcal H^2\delta
=-\int_{\mathbf k_1\mathbf k_2}
(2\pi)^3\delta_D(\mathbf k_1+\mathbf k_2-\mathbf k)
\beta(\mathbf k_1,\mathbf k_2)
\theta(\mathbf k_1)\theta(\mathbf k_2),
$$

with the symmetric [beta mode-coupling kernel](../../../large-scale-structure-of-the-universe.md#beta-mode-coupling-kernel)

$$
\boxed{\beta(\mathbf k_1,\mathbf k_2)
=\frac{|\mathbf k_1+\mathbf k_2|^2
(\mathbf k_1\cdot\mathbf k_2)}{2k_1^2k_2^2}}.
$$

In the [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $a'=\mathcal Ha$ and $\mathcal H'=-\mathcal H^2/2$. At linear order the ansatz gives $\widetilde\theta^{(1)}=\widetilde\delta^{(1)}$. At second order, the continuity and Euler equations become

$$
2\widetilde\delta^{(2)}-\widetilde\theta^{(2)}
=\int\alpha_s\widetilde\delta^{(1)}\widetilde\delta^{(1)},
$$



$$
3\widetilde\delta^{(2)}-5\widetilde\theta^{(2)}
=-2\int\beta\widetilde\delta^{(1)}\widetilde\delta^{(1)},
$$

where each integral includes the momentum-conserving measure above. Eliminating $\widetilde\theta^{(2)}$ yields

$$
\widetilde\delta^{(2)}(\mathbf k)
=\int_{\mathbf k_1\mathbf k_2}(2\pi)^3\delta_D(\mathbf k_1+\mathbf k_2-\mathbf k)
F_2(\mathbf k_1,\mathbf k_2)
\widetilde\delta^{(1)}(\mathbf k_1)
\widetilde\delta^{(1)}(\mathbf k_2),
$$

with the [standard perturbation theory density kernel](../../../large-scale-structure-of-the-universe.md#standard-perturbation-theory-density-kernel)

$$
\boxed{F_2=\frac57\alpha_s+\frac27\beta}.
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Expand $\delta=a\delta_1+a^2\delta_2+a^3\delta_3+\cdots$. For a Gaussian linear density field, odd linear correlators vanish and [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) reduces the fourth-order terms to products of the linear [power spectrum](../../../probability-and-statistics.md#power-spectrum). Hence

$$
P_{\rm 1-loop}(k)
=a^2P(k)+a^4[P_{22}(k)+2P_{13}(k)].
$$

The two contractions of the two quadratic fields give

$$
\boxed{P_{22}(k)=2\int\frac{d^3q}{(2\pi)^3}
F_2(\mathbf q,\mathbf k-\mathbf q)^2
P(q)P(|\mathbf k-\mathbf q|)}.
$$

The three choices for which argument of $F_3$ carries the external momentum give

$$
\boxed{P_{13}(k)=3P(k)\int\frac{d^3q}{(2\pi)^3}
F_3(\mathbf k,\mathbf q,-\mathbf q)P(q)}.
$$

**Thus the contribution conventionally called $P_{13}+P_{31}$ is $2P_{13}=6P(k)\int F_3P$. These are the two one-loop diagrams of the [one-loop matter power spectrum](../../../large-scale-structure-of-the-universe.md#one-loop-matter-power-spectrum).**

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Set $\mathbf q=\mathbf k_1$, $\mathbf k-\mathbf q=\mathbf k_2$, $q=|\mathbf q|$, and $\mu=\widehat{\mathbf k}\cdot\widehat{\mathbf q}$. Substitution into $F_2=5\alpha_s/7+2\beta/7$ gives

$$
F_2(\mathbf q,\mathbf k-\mathbf q)
=\frac{k^2[7k\mu+q(3-10\mu^2)]}
{14q(k^2-2kq\mu+q^2)}.
$$

The azimuthal integral in $d^3q=q^2dq\,d\mu\,d\phi$ and the factor two in $P_{22}$ then give

$$
P_{22}(k)=\int_0^\infty\frac{dq}{4\pi^2}
\int_{-1}^1d\mu\,
\frac{k^4[7k\mu+q(3-10\mu^2)]^2}
{98(k^2-2kq\mu+q^2)^2}
P(q)P(\sqrt{k^2-2kq\mu+q^2}).
$$

For the [scale-free matter power spectrum](../../../large-scale-structure-of-the-universe.md#scale-free-matter-power-spectrum) $P(k)=Ak^n$, put $r=q/k$ and

$$
s(r,\mu)=\sqrt{1-2r\mu+r^2}.
$$

All dimensional factors separate:

$$
\boxed{P_{22}(k)=A^2k^{2n+3}
\int_0^\infty dr\int_{-1}^1d\mu\,K_{22}(r,\mu;n)},
$$

where

$$
\boxed{K_{22}(r,\mu;n)=
\frac{r^n[7\mu+r(3-10\mu^2)]^2}
{392\pi^2[1-2r\mu+r^2]^{,2-n/2}}}.
$$

As $r\to0$, $K_{22}\sim r^n\mu^2/(8\pi^2)$, so the soft-$q$ integral converges exactly when $n>-1$. For $r\to\infty$, $K_{22}\sim r^{2n-2}$ times an angular function, requiring $n<1/2$. At fixed $\mu<1$, $r\to1$ is regular. The corner $(r,\mu)=(1,1)$ makes $|\mathbf k-\mathbf q|$ soft; after resolving that corner in the local soft momentum, its radial behavior is again $p^n dp$, requiring $n>-1$. Therefore

$$
\boxed{-1<n<\frac12}
$$

is the infrared- and ultraviolet-convergence window for $P_{22}$.

## 3

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a Gaussian smoothed density contrast, the Press-Schechter factor of two gives the collapsed mass fraction

$$
F(>M)=2\int_{\delta_c}^{\infty}
\frac{d\delta}{\sqrt{2\pi}\sigma}
e^{-\delta^2/(2\sigma^2)}
=\operatorname{erfc}\left(\frac\nu{\sqrt2}\right),
\qquad
\nu=\frac{\delta_c}{\sigma(M)}.
$$

The fraction in the interval $[M,M+dM]$ is $-(dF/dM)dM=(M/\bar\rho)(dn/dM)dM$. Since $d\nu/dM=-\nu\,d\log\sigma/dM$,

$$
\boxed{
\frac{dn}{dM}
=-\sqrt{\frac2\pi}\frac{\bar\rho}{M^2}
\nu e^{-\nu^2/2}\frac{d\log\sigma}{d\log M}}
$$

or, equivalently, the same expression with $|d\log\sigma/d\log M|$. The minus sign is needed because $\sigma(M)$ decreases with $M$; this is the positive [Press-Schechter halo mass function](../../../large-scale-structure-of-the-universe.md#press-schechter-halo-mass-function).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

In the [peak-background split](../../../large-scale-structure-of-the-universe.md#peak-background-split), a long-wavelength overdensity changes the local threshold from $\delta_c$ to $\delta_c-\delta_l$. At fixed mass, the [Press-Schechter halo mass function](../../../large-scale-structure-of-the-universe.md#press-schechter-halo-mass-function) depends on the threshold through $\nu e^{-\nu^2/2}$. Therefore

$$
b_L
=\left.\frac1n\frac{\partial n}{\partial\delta_l}\right|_{\delta_l=0}
=-\frac{\partial\log n}{\partial\delta_c}
=-\frac1{\delta_c}\frac{\partial}{\partial\log\nu}
\log(\nu e^{-\nu^2/2}).
$$

It follows that the [linear Lagrangian halo bias](../../../large-scale-structure-of-the-universe.md#linear-lagrangian-halo-bias) is

$$
\boxed{b_L(M)=\frac{\nu^2-1}{\delta_c}}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

On wavelengths much larger than halos, all matter is partitioned among halos. The mass-weighted halo overdensity must therefore equal the matter overdensity. Since $\delta_h(M)=b(M)\delta_m$, [mass conservation](../../../continuum-mechanics.md#mass-conservation) requires

$$
\int_0^\infty dM\,\frac{dn}{dM}\frac{M}{\bar\rho}b(M)=1.
$$

For the [Press-Schechter formalism](../../../large-scale-structure-of-the-universe.md#press-schechter-formalism), the mass-fraction measure becomes

$$
f(\nu)d\nu=\sqrt{\frac2\pi}e^{-\nu^2/2}d\nu,
\qquad \nu\geq0.
$$

It is normalized and is a half-normal distribution, so

$$
\int_0^\infty f(\nu)d\nu=1,
\qquad
\int_0^\infty\nu^2f(\nu)d\nu=1.
$$

Using the [linear Eulerian halo bias](../../../large-scale-structure-of-the-universe.md#linear-eulerian-halo-bias)

$$
b=1+b_L=1+\frac{\nu^2-1}{\delta_c}
$$

therefore gives

$$
\int_0^\infty f(\nu)b(\nu)d\nu
=1+\frac{1-1}{\delta_c}=1,
$$

which verifies the consistency relation.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Write the matter density as a sum over normalized halo profiles,

$$
\rho(\mathbf x)=\sum_iM_i u(\mathbf x-\mathbf x_i|M_i),
\qquad
\int d^3x\,u(\mathbf x|M)=1.
$$

For $\mathbf k\ne0$, its density contrast is

$$
\delta(\mathbf k)=\frac1{\bar\rho}
\sum_iM_i\widetilde u(k|M_i)e^{-i\mathbf k\cdot\mathbf x_i}.
$$

If halo locations form an uncorrelated Poisson process, only equal-halo terms survive after subtracting the homogeneous contribution. Replacing the sum per unit volume by the halo abundance gives the [one-halo term](../../../large-scale-structure-of-the-universe.md#one-halo-term)

$$
\boxed{P(k)=P_{1h}(k)
=\int_0^\infty dM\,\frac{dn}{dM}
\left(\frac{M}{\bar\rho}\right)^2
|\widetilde u(k|M)|^2}.
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

For distinct halos, insert their linearly biased correlation

$$
\xi_{hh}(r|M_1,M_2)=b(M_1)b(M_2)\xi_{\rm lin}(r)
$$

into the double sum. Fourier transformation converts $\xi_{\rm lin}$ into $P_{\rm lin}$, while the two independent mass integrals factorize. The result is the [halo model](../../../large-scale-structure-of-the-universe.md#halo-model)

$$
P(k)=P_{1h}(k)+P_{2h}(k),
$$

where

$$
\boxed{P_{2h}(k)=
\left[\int_0^\infty dM\,\frac{dn}{dM}
\frac{M}{\bar\rho}b(M)\widetilde u(k|M)\right]^2
P_{\rm lin}(k)}.
$$

Thus the requested function is

$$
\boxed{f(M,\bar\rho)=\frac{M}{\bar\rho}}.
$$

At small $k$, profile normalization gives $\widetilde u\to1$ and the bias consistency relation makes the square bracket tend to one, so the [two-halo term](../../../large-scale-structure-of-the-universe.md#two-halo-term) approaches the linear matter spectrum.

## 4

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Project the photon [Boltzmann equation](../../../statistical-physics.md#boltzmann-equation) onto [Legendre polynomials](../../../differential-equation.md#legendre-polynomial). The angular average uses $\langle\Theta\rangle=\Theta_0$ and $\langle\mu\rangle=0$, so the collision term has no monopole and

$$
\boxed{\Theta_0'=-k\Theta_1+\Phi'}.
$$

For the dipole, the recurrence relation makes free streaming couple $\Theta_1$ to $\Theta_0$ and $\Theta_2$. The gravitational term $-ik\mu\Psi$ contributes $k\Psi/3$, while projection of $i\mu v_b$ gives the baryon-velocity source. Thus

$$
\Theta_1'=\frac{k}{3}(\Theta_0+\Psi-2\Theta_2)
-\Gamma\left(\Theta_1+\frac{v_b}{3}\right).
$$

Neglecting the [photon quadrupole](../../../cosmic-microwave-background-anisotropy.md#photon-quadrupole) gives

$$
\boxed{3\Theta_1'=k(\Theta_0+\Psi)-\Gamma(3\Theta_1+v_b)}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In the [tight-coupling approximation](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation), finiteness of the photon Euler equation as $\Gamma\to\infty$ requires

$$
v_b=-3\Theta_1+O(\Gamma^{-1}).
$$

Let $S=3\Theta_1+v_b$. Rearranging the baryon Euler equation and substituting the leading relation only on its right-hand side gives

$$
S=-\frac R\Gamma(v_b'+\mathcal Hv_b+k\Psi)
=\frac R\Gamma(3\Theta_1'+3\mathcal H\Theta_1-k\Psi)
+O(\Gamma^{-2}).
$$

Insert this slip into the photon Euler equation:

$$
3(1+R)\Theta_1'+3\mathcal HR\Theta_1
=k\Theta_0+k(1+R)\Psi.
$$

The photon continuity equation gives $\Theta_1=-(\Theta_0'-\Phi')/k$. Eliminating the dipole yields

$$
\boxed{
\Theta_0''+\frac{\mathcal HR}{1+R}\Theta_0'
+c_s^2k^2\Theta_0
=-\frac{k^2}{3}\Psi+\Phi''
+\frac{\mathcal HR}{1+R}\Phi'},
$$

where the [photon-baryon sound speed](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-sound-speed) is

$$
\boxed{c_s^2=\frac1{3(1+R)}}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For $R=0$, $c_s=1/\sqrt3$. If the [Newtonian potentials](../../../linear-cosmological-perturbation-theory.md#newtonian-gauge) are constant and equal, the equation in part (b) becomes

$$
\Theta_0''+c_s^2k^2\Theta_0=-c_s^2k^2\Psi.
$$

The [Sachs-Wolfe combination](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-combination) $D=\Theta_0+\Psi$ therefore obeys

$$
D''+c_s^2k^2D=0.
$$

Adiabatic initial conditions have vanishing initial fluid velocity, hence $D'(0)=0$. With the [sound horizon](../../../cosmic-microwave-background-anisotropy.md#sound-horizon) $r_s(\eta)=\int_0^\eta c_s,d\eta'$, the solution is

$$
\boxed{\Theta_0+\Psi=(\Theta_0+\Psi)_{\rm ini}\cos(kr_s)}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The $\ell=2$ projection of the [Boltzmann hierarchy](../../../statistical-physics.md#boltzmann-hierarchy) is

$$
\Theta_2'=\frac{k}{5}(2\Theta_1-3\Theta_3)-\Gamma\Theta_2.
$$

In tight coupling, $\Theta_2=O(k/\Gamma)$ and $\Theta_3$ is higher order. Neglecting $\Theta_2'$ relative to $\Gamma\Theta_2$ at leading order gives

$$
\boxed{\Theta_2\simeq\frac25\frac{k}{\Gamma}\Theta_1},
$$

so $C=2/5$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The continuity equation and the cosine solution give

$$
\Theta_1=-\frac{\Theta_0'}k
\propto c_s\sin(kr_s)
$$

when the potentials are constant. Part (d) then implies

$$
\Theta_2\propto\frac{k}{\Gamma}\sin(kr_s).
$$

Since [Cosmic microwave background polarization](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-polarization) is sourced by the local quadrupole at last scattering,

$$
\boxed{\mathcal P_*(k)\propto\sin(kr_{s*})}.
$$

The monopole contribution to the CMB temperature oscillates as $\cos(kr_{s*})$, so its acoustic extrema occur near $kr_{s*}=m\pi$, whereas polarization extrema occur near $kr_{s*}=(m+\tfrac12)\pi$. The principal polarization peaks are therefore interleaved with the principal temperature peaks. Projection, baryon loading, time-varying potentials, and the temperature Doppler contribution shift the observed angular peaks from this idealized phase relation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
