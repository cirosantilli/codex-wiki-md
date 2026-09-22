# Paper 41

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper41.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper41.pdf)

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
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

An [order parameter](../../../critical-phenomenon.md#order-parameter) distinguishes phases through a macroscopic observable, such as the mean spin $m$ of a ferromagnet. Its vanishing can reflect an unbroken symmetry, while choosing one of several nonzero equilibrium values gives [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking). [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory) treats it as a slowly varying field and expands the [free energy](../../../thermodynamics.md#thermodynamic-free-energy) in terms allowed by symmetry:

$$
\mathcal A[m]=\int d^Dx\left[\frac K2|\nabla m|^2+\frac r2m^2+\frac u4m^4+\frac v6m^6-hm\right].
$$

Here $K>0$ penalizes spatial variation, $h$ is the conjugate field, and the highest retained even coefficient must stabilize large $|m|$. For a spin-flip-symmetric system, odd powers are forbidden at $h=0$. Equilibrium in the [Landau approximation](../../../critical-phenomenon.md#landau-approximation) minimizes this functional; near an ordinary continuous transition $r=r_t t$ with $t=(T-T_c)/T_c$ and $r_t>0$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For $u>0$, the quartic [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) at $h=0$ minimizes at $m=0$ for $r>0$ and at $m=\pm\sqrt{-r/u}$ for $r<0$. The [order parameter](../../../critical-phenomenon.md#order-parameter) changes continuously at $r=0$, giving a [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition) and a divergent response. The minimized potential is $0$ above the transition and $-r^2/(4u)$ below it, so its first temperature derivative is continuous while its second derivative jumps.

For $u<0$, retain $v>0$. A [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition) occurs when the $m=0$ minimum and a nonzero minimum have equal free energy. Combining stationarity $r+um^2+vm^4=0$ with equality of potential values gives

$$
\boxed{m^2=-\frac{3u}{4v},\qquad r=\frac{3u^2}{16v}.}
$$

The order parameter jumps at a positive $r$ before the disordered minimum loses local stability. Generic temperature dependence then also produces a jump in entropy and a [latent heat](../../../thermodynamics.md#latent-heat). Equality of global minima locates coexistence; the disappearance of a metastable minimum instead defines a [spinodal point](../../../critical-phenomenon.md#spinodal-point).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

At fixed average [order parameter](../../../critical-phenomenon.md#order-parameter), a nonconvex local potential need not describe the equilibrium free energy. A mixture of two phases can lower it to the common-tangent convex envelope. If their magnetizations are $m_1,m_2$, the coexistence field satisfies

$$
f'(m_1)=f'(m_2)=h_{\rm coex},\qquad f(m_2)-f(m_1)=h_{\rm coex}(m_2-m_1).
$$

Equivalently, $\int_{m_1}^{m_2}[f'(m)-h_{\rm coex}]\,dm=0$, the equal-area [Maxwell construction](../../../thermodynamics.md#maxwell-construction). An average $\bar m$ between $m_1$ and $m_2$ is obtained by choosing their volume fractions according to the lever rule. The gradient term in [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory) gives a finite interfacial energy and smooth [domain walls](../../../critical-phenomenon.md#domain-wall); in the thermodynamic limit the bulk gain dominates the interface cost. Domains are therefore especially natural under a constrained mean magnetization or suitable boundary conditions. Without such a constraint, one pure phase is also an equilibrium state at coexistence.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

[Critical exponents](../../../critical-phenomenon.md#critical-exponent) describe singular behavior near a [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition). Define $m(t,0)\sim(-t)^\beta$ below $T_c$, susceptibility $\chi(t,0)=\partial m/\partial h\sim|t|^{-\gamma}$, singular [heat capacity](../../../thermodynamics.md#heat-capacity) $C_s\sim|t|^{-\alpha}$, and critical isotherm $m(0,h)\sim\operatorname{sgn}(h)|h|^{1/\delta}$. The ordinary quartic [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) gives the equation of state

$$
h=r_t t\,m+um^3.
$$

At zero field its ordered minimum is proportional to $(-t)^{1/2}$. Differentiating the equation of state gives $\chi^{-1}=r_t t+3um^2$, proportional to $|t|$ on either side. At $t=0$, $h=um^3$, and the minimized free energy below the transition is proportional to $-t^2$. Thus

$$
\boxed{\beta=\tfrac12,\qquad\gamma=1,\qquad\delta=3,\qquad\alpha=0.}
$$

Here $\alpha=0$ denotes a finite heat-capacity jump, rather than a power divergence. Including gradients gives the [Landau scalar correlation length](../../../critical-phenomenon.md#landau-scalar-correlation-length) $\xi\propto|t|^{-1/2}$ and correlation-length exponent $\nu=1/2$.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

A [tricritical point](../../../critical-phenomenon.md#tricritical-point) occurs at $r=u=h=0$ with $v>0$: tuning $u$ changes a continuous transition into a first-order one. At $u=0$, the equation of state is $h=rm+vm^5$. It gives $m\propto(-r)^{1/4}$ at $h=0$, $m\propto h^{1/5}$ at $r=0$, and a minimized free energy proportional to $-|r|^{3/2}$ below the transition. The mean-field tricritical exponents are

$$
\boxed{\beta=\tfrac14,\quad\delta=5,\quad\gamma=1,\quad\alpha=\tfrac12.}
$$

In the three-dimensional parameter space $(r,u,h)$, the zero-field disordered-to-ordered continuous line $r=0,u>0$ meets the first-order line $r=3u^2/(16v),u<0$ at the tricritical point. The zero-field surface also contains coexistence of positive and negative ordered phases. For negative $u$, tilting with $h$ produces two symmetric [tricritical wings](../../../critical-phenomenon.md#tricritical-wing) of first-order coexistence, each bounded by a line of ordinary critical endpoints. Those wings and their critical edges meet at the tricritical point. The [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension) of tricritical sextic theory is three, so mean-field values can acquire logarithmic corrections there.

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [scaling hypothesis for critical phenomena](../../../critical-phenomenon.md#scaling-hypothesis-for-critical-phenomena) says that the singular equilibrium [free-energy density](../../../statistical-physics.md#free-energy-density) is a generalized homogeneous function of the thermal and field variables, after analytic backgrounds are removed. To derive the ordinary mean-field form, put $r=r_t t$, $u>0$ and neglect the higher powers near the transition. Rescale $m=\sqrt{r_t/u}\,|t|^{1/2}\psi$. Minimizing the quartic potential becomes

$$
A_s=\frac{r_t^2}{u}|t|^2\min_\psi\left[\frac{\operatorname{sgn}(t)}2\psi^2+\frac14\psi^4-\frac{\sqrt u}{r_t^{3/2}}\frac h{|t|^{3/2}}\psi\right].
$$

This is the [mean-field scalar free-energy scaling](../../../critical-phenomenon.md#mean-field-scalar-free-energy-scaling) form with $a=r_t^2/u$, $b=\sqrt u/r_t^{3/2}$. The two functions correspond to $t>0$ and $t<0$; the latter has two pure-phase branches and a cusp at zero field. The question's $>$ and $<$ subscripts distinguish these temperatures above and below $T_c$.

Differentiating with respect to $h$ gives $m=-\partial_hA_s\propto|t|^{1/2}$ on an ordered pure branch, and differentiating again gives $\chi=-\partial_h^2A_s\propto|t|^{-1}$. Thus the displayed scaling form independently yields $\beta=1/2$ and $\gamma=1$.

To allow anomalous powers, replace it by

$$
A_s=a|t|^{2-\alpha}f_\pm\left(\frac{bh}{|t|^\Delta}\right).
$$

Then $\beta=2-\alpha-\Delta$ and $\gamma=2\Delta-(2-\alpha)$. Taking $t\to0$ at fixed small $h$ gives $A_s\propto|h|^{(2-\alpha)/\Delta}$, so $1/\delta=(2-\alpha-\Delta)/\Delta=\beta/\Delta$. Eliminating $\Delta$ proves the [Rushbrooke scaling relation](../../../critical-phenomenon.md#rushbrooke-scaling-relation) and [Widom scaling relation](../../../critical-phenomenon.md#widom-scaling-relation):

$$
\boxed{\alpha+2\beta+\gamma=2,\qquad\beta\delta=\Delta=\beta+\gamma.}
$$

These power-law relations assume the simple scaling form; marginal corrections or [dangerously irrelevant couplings](../../../critical-phenomenon.md#dangerously-irrelevant-coupling) can require additional scaling variables.

## 2

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function) $G(r)=\langle\sigma_0\sigma_r\rangle-\langle\sigma_0\rangle\langle\sigma_r\rangle$. Away from criticality its large-distance envelope decays exponentially on the [correlation length](../../../critical-phenomenon.md#correlation-length) $\xi$, often with an algebraic prefactor. At criticality $\xi$ diverges and a short-range scalar model instead has the power law $G(r)\sim r^{-(D-2+\eta)}$, with [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension) $\eta$.

A [blocking kernel](../../../critical-phenomenon.md#blocking-kernel) $K_b(\sigma',\sigma)$ assigns coarse spins to each block of side $b$ lattice spacings, with $\sum_{\sigma'}K_b(\sigma',\sigma)=1$. Define the coarse Hamiltonian by

$$
e^{-\beta H(u',\sigma')-\beta N'C'}=\sum_\sigma K_b(\sigma',\sigma)e^{-\beta H(u,\sigma)-\beta NC}.
$$

The operator basis must be sufficiently complete to include interactions generated by blocking. Summing over coarse spins preserves the [partition function](../../../statistical-physics.md#canonical-partition-function), while the physical lattice spacing and site count change to $a'=ba$, $N'=b^{-D}N$. After $p$ steps they are $a_p=b^pa$ and $N_p=b^{-pD}N$. Exact blocking preserves the long-distance predictions; truncating the generated interaction space introduces an approximation.

Define the dimensionless free energy per site $F(u,C)=-N^{-1}\log Z(u,C,N)=f(u)+\beta C$. Preservation of $Z$ gives $F(u_0,C_0)=b^{-pD}F(u_p,C_p)$. For one step, removing the explicitly additive constant gives

$$
f(u_j)=b^{-D}f(u_{j+1})+g(u_j),\qquad g(u_j)=\beta\bigl[b^{-D}C_{j+1}-C_j\bigr].
$$

The function $g$ records the additive [free-energy density](../../../statistical-physics.md#free-energy-density) generated by eliminated degrees of freedom; it is usually regular near a finite blocking step's critical point. Iteration proves

$$
\boxed{f(u_0)=b^{-pD}f(u_p)+\sum_{j=0}^{p-1}b^{-jD}g(u_j).}
$$

This is the [additive free-energy recursion under blocking](../../../critical-phenomenon.md#additive-free-energy-recursion-under-blocking). After removing regular backgrounds, its singular part obeys homogeneous scaling.

A [renormalization-group fixed point](../../../critical-phenomenon.md#renormalization-group-fixed-point) satisfies $R_b(u^*)=u^*$. Linearizing the map gives scaling coordinates $v_i'=b^{\lambda_i}v_i$. A [relevant operator](../../../critical-phenomenon.md#relevant-operator) has $\lambda_i>0$, an [irrelevant operator](../../../critical-phenomenon.md#irrelevant-operator) has $\lambda_i<0$, and a marginal operator has $\lambda_i=0$ and needs nonlinear analysis. The [critical surface](../../../critical-phenomenon.md#critical-surface) consists of points flowing into the critical fixed point after all relevant directions are tuned. An outgoing or repulsive trajectory lies in the unstable manifold and describes perturbations that grow under coarse-graining.

<a id="2/image-renormalization-group-flow-near-a-critical-surface"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-41-rg-flow.png)

**[Figure 1](#2/image-renormalization-group-flow-near-a-critical-surface). Renormalization-group flow near a critical surface**.

With relevant thermal and magnetic coordinates $t,h$, the singular [free-energy density](../../../statistical-physics.md#free-energy-density) obeys $F_s(t,h)=b^{-D}F_s(b^{\lambda_t}t,b^{\lambda_h}h)$. Choose $b=|t|^{-1/\lambda_t}$ to obtain

$$
\boxed{F_s(t,h)=|t|^{D/\lambda_t}f_\pm\left(\frac h{|t|^{\lambda_h/\lambda_t}}\right).}
$$

Here $\lambda_t,\lambda_h$ are the positive scaling eigenvalues, and $f_\pm$ refer to the signs of $t$. Since $\xi(t,h)=b\xi(b^{\lambda_t}t,b^{\lambda_h}h)$, the correlation-length exponent is $\nu=1/\lambda_t$. Two temperature derivatives of $F_s(t,0)$ give $\alpha=2-D/\lambda_t$, establishing the [hyperscaling relation](../../../critical-phenomenon.md#hyperscaling-relation)

$$
\boxed{\alpha=2-D\nu.}
$$

The magnetization exponent similarly is $\beta=(D-\lambda_h)/\lambda_t$. These expressions assume no additional dangerous scaling variables.

For the [Gaussian field theory](../../../critical-phenomenon.md#gaussian-field-theory), decompose the field into low and high [Fourier modes](../../../fourier-analysis.md#fourier-mode), integrate out $\Lambda/b<|p|<\Lambda$, and restore the cutoff using $x=bx'$ and $\phi(x)=b^{-(D-2)/2}\phi'(x')$. The gradient coefficient remains fixed, the mass coefficient transforms as $m'^2=b^2m^2$, and the uniform source as $h'=b^{(D+2)/2}h$. Hence $\lambda_t=2$, $\lambda_h=(D+2)/2$, and the [Gaussian momentum-shell scaling](../../../critical-phenomenon.md#gaussian-momentum-shell-scaling) gives

$$
\boxed{\alpha=\frac{4-D}{2},\qquad\beta=\frac{D-2}{4}.}
$$

The sign convention $+h\phi$ reverses the magnetization's sign but not these exponents. For $2<D<4$, these are Gaussian scaling predictions, not the exponents of a generic interacting scalar critical point: the quartic interaction is relevant there. The free quadratic Hamiltonian also has no stable ordered phase at negative $m^2$, so the quoted $\beta$ is its formal order-parameter scaling index, not a spontaneously magnetized state of the unstabilized Gaussian integral. The relevance distinction is also explained in [Tong's renormalization-group lecture notes](https://www.damtp.cam.ac.uk/user/tong/sft/sfthtml/S3.html).

## 3

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The ultraviolet cutoff specifies which fluctuations remain explicit. Changing it integrates out some modes; to preserve long-distance predictions, their effect must be absorbed into the mass, interactions, and other couplings. Thus bare coefficients depend on $\Lambda$. The long-distance inverse [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function) has the form $\widetilde\Gamma(p)\simeq Z^{-1}(p^2+\xi^{-2})$. After fixing the gradient normalization, the infrared mass is an inverse [correlation length](../../../critical-phenomenon.md#correlation-length). With the question's unrescaled gradient coefficient, $\xi^{-2}=\alpha m^2$ at Gaussian level, so proportionality rather than literal equality is appropriate until that normalization is chosen.

As a concrete [momentum-shell renormalization group](../../../critical-phenomenon.md#momentum-shell-renormalization-group) step, split $\phi=\phi_<+\phi_>$ into modes below $\Lambda/b$ and in the shell $\Lambda/b<|p|<\Lambda$, and define

$$
e^{-H_{\rm eff}[\phi_<]}=\int\mathcal D\phi_>\,e^{-H[\phi_<+\phi_>]}.
$$

Then rescale coordinates and the field to restore the cutoff and gradient coefficient. A [local derivative expansion](../../../critical-phenomenon.md#local-derivative-expansion) of $H_{\rm eff}$ gives new quadratic, quartic, and higher even couplings. If the system has short-range interactions, the field varies slowly, the effective potential is analytic, and remaining fluctuations are small, retaining the leading gradient and lowest stabilizing powers and minimizing the resulting functional gives [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory). Suppressing the omitted fluctuations is the substantive [Landau approximation](../../../critical-phenomenon.md#landau-approximation); it is justified sufficiently far from the narrow fluctuation region or above the appropriate [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension).

The truncated two-point function in this question is the [one-particle-irreducible two-point vertex](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-two-point-vertex), $\widetilde\Gamma(p)=\widetilde G(p)^{-1}$. It is the Hessian of the Legendre effective action, not merely the connected two-point function. In perturbation theory,

$$
\widetilde\Gamma(p)=\widetilde G_0(p)^{-1}+\delta m^2+\Sigma(p).
$$

Here $\widetilde G_0$ is the Gaussian propagator about the chosen reference mass, $\delta m^2$ is the mass [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) or bare-to-reference mass shift, and $\Sigma$ is the interaction [self-energy](../../../perturbative-quantum-field-theory.md#self-energy), computed from proper diagrams. Fix the gradient normalization so $\widetilde G_0(p)=(p^2+M^2)^{-1}$, and choose the infrared reference mass $M^2=m^2(0,T)$. Then $\delta m^2=m^2(\Lambda,T)-M^2$ at this order. The mass renormalization condition is $\widetilde\Gamma(0)=M^2$.

At one loop the only two-point diagram is the quartic [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram). There are $4\cdot3$ choices for attaching its two external lines, leaving the other pair contracted; dividing by $4!$ gives its factor $1/2$. It is independent of external momentum, so

$$
\Sigma^{(1)}(p)=\frac g2\int_{|q|<\Lambda}\frac{d^Dq}{(2\pi)^D}\frac1{q^2+M^2}.
$$

The renormalization condition therefore gives the self-consistent one-loop equation

$$
\boxed{M^2=m^2(\Lambda,T)+\frac g2\int_{|q|<\Lambda}\frac{d^Dq}{(2\pi)^D}\frac1{q^2+M^2}.}
$$

Using $M$ inside the loop is a self-consistent resummation; replacing it by the bare mass gives the same formal first-order expansion away from infrared problems.

Subtract the equation at $T_c$, where $M=0$, and absorb regular temperature dependence of $g$ into the thermal coefficient. Let $\tau=m^2(\Lambda,T)-m^2(\Lambda,T_c)\propto T-T_c$ and $I(M)=\int_{|q|<\Lambda}d^Dq/(2\pi)^D(q^2+M^2)^{-1}$. Then

$$
\tau=M^2+\frac g2[I(0)-I(M)],\qquad I(0)-I(M)=\int_{|q|<\Lambda}\frac{d^Dq}{(2\pi)^D}\frac{M^2}{q^2(q^2+M^2)}.
$$

For $D>4$, the integral divided by $M^2$ tends to a finite cutoff-dependent constant, since its small-momentum radial integrand is $q^{D-5}$. Thus $\tau$ is proportional to $M^2$, consistent with the Landau prediction. For $2<D<4$, set $q=Mz$: the correction instead scales as $M^{D-2}$ and dominates $M^2$. At $D=4$ it is proportional to $M^2\log(\Lambda/M)$. Hence a pure linear Landau mass law without logarithmic modification is consistent only above

$$
\boxed{D_c=4.}
$$

For $D\leq2$, the massless integral itself is infrared divergent, so the subtraction already needs additional care. The sub-four-dimensional self-consistent approximation locates the breakdown of mean-field behavior; it is not an exact calculation of interacting critical exponents.

At a [tricritical point](../../../critical-phenomenon.md#tricritical-point) the quartic coupling is tuned away and the leading stabilizing interaction is $g_6\phi^6$. At the [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point), the field has [engineering dimension](../../../critical-phenomenon.md#engineering-dimension) $(D-2)/2$, so the sextic coefficient rescales as $g_6'=b^{D-3(D-2)}g_6=b^{6-2D}g_6$. It changes from irrelevant to relevant at

$$
\boxed{D_c^{\rm tricritical}=3.}
$$

This is the sextic case of the [upper critical dimension of an even scalar interaction](../../../critical-phenomenon.md#upper-critical-dimension-of-an-even-scalar-interaction); marginality at three dimensions allows logarithmic corrections.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
