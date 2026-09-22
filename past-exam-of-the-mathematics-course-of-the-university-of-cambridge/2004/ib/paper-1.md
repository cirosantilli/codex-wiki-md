# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2004/PaperIB_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2004/PaperIB_1.pdf)

**Table of contents**

- [1H](#1h)
  - [Solution](#1h/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3G](#3g)
  - [Solution](#3g/solution)
- [4G](#4g)
  - [Solution](#4g/solution)
  - [i](#4g/i)
    - [Solution](#4g/i/solution)
  - [ii](#4g/ii)
    - [Solution](#4g/ii/solution)
  - [iii](#4g/iii)
    - [Solution](#4g/iii/solution)
- [5A](#5a)
  - [i](#5a/i)
    - [Solution](#5a/i/solution)
  - [ii](#5a/ii)
    - [Solution](#5a/ii/solution)
  - [iii](#5a/iii)
    - [Solution](#5a/iii/solution)
- [6B](#6b)
  - [Solution](#6b/solution)
- [7B](#7b)
  - [Solution](#7b/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
- [10H](#10h)
  - [Solution](#10h/solution)
- [11H](#11h)
  - [a](#11h/a)
    - [Solution](#11h/a/solution)
  - [b](#11h/b)
    - [Solution](#11h/b/solution)
  - [Solution](#11h/solution)
- [12H](#12h)
  - [Solution](#12h/solution)
- [13F](#13f)
  - [Solution](#13f/solution)
- [14G](#14g)
  - [Solution](#14g/solution)
- [15G](#15g)
  - [Solution](#15g/solution)
- [16A](#16a)
  - [Solution](#16a/solution)
- [17B](#17b)
  - [Solution](#17b/solution)
- [18B](#18b)
  - [Solution](#18b/solution)
- [19D](#19d)
  - [Solution](#19d/solution)
- [20C](#20c)
  - [Solution](#20c/solution)
- [21H](#21h)
  - [Solution](#21h/solution)
- [22H](#22h)
  - [Solution](#22h/solution)

## 1H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1h/solution">Solution</h3>

↑ **Parent:** [1H](#1h)

Expand $e_{r+1}$ in the given [spanning set](../../../vector-space.md#spanning-set):

$$
e_{r+1}=\sum_{i=1}^ra_ie_i+\sum_{j=r+1}^mb_jf_j.
$$

Some $b_j$ must be nonzero, since otherwise $e_{r+1}$ would lie in the span of the earlier $e_i$, contradicting [linear independence](../../../vector-space.md#linear-independence). Reorder the remaining $f_j$ so $b_{r+1}\ne0$. Solving this equation for $f_{r+1}$ expresses it in terms of $e_1,\ldots,e_{r+1},f_{r+2},\ldots,f_m$. Every member of the old [spanning set](../../../vector-space.md#spanning-set) is therefore in the new span, so **the replacement set still spans $V$**. This proves the needed step of the [Steinitz exchange lemma](../../../vector-space.md#steinitz-exchange-lemma) directly.

Starting with $f_1,\ldots,f_m$, apply that replacement successively to $e_1,e_2,\ldots$. After $r\leq m$ steps the spanning list is $e_1,\ldots,e_r$ together with $m-r$ unreplaced $f$'s. If $n>m$, after $m$ replacements the list $e_1,\ldots,e_m$ spans $V$, forcing $e_{m+1}$ to be a [linear combination](../../../vector-space.md#linear-combination) of it. That contradicts [linear independence](../../../vector-space.md#linear-independence). Hence **$\boxed{n\leq m}$**.

## 2F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

The [normalizer](../../../group-theory.md#normalizer) is $N_G(H)=\{g\in G:gHg^{-1}=H\}$. It is a [subgroup](../../../group.md#subgroup): the identity normalizes $H$, products of normalizing elements normalize it, and conjugating the equality by $g^{-1}$ proves inverse closure. The map

$$
G/N_G(H)\longrightarrow\{\text{conjugates of }H\},\qquad gN_G(H)\longmapsto gHg^{-1}
$$

is well-defined and onto. Two images are equal exactly when $g_2^{-1}g_1\in N_G(H)$, exactly the condition that their [cosets](../../../group-theory.md#coset) coincide. Thus **the number of conjugates is $\boxed{[G:N_G(H)]}$**.

By the permitted conjugacy assertion for [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup), the number $n_p$ of Sylow $p$-[subgroups](../../../group.md#subgroup) equals $[G:N_G(P)]$ for one such [subgroup](../../../group.md#subgroup) $P$. [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) makes this divide $|G|$, and $P\subseteq N_G(P)$ also makes it divide $|G|/|P|$.

For order $72=8\cdot9$, a Sylow $3$-[subgroup](../../../group.md#subgroup) has order nine, so $n_3$ divides eight. To obtain the required congruence without assuming an additional Sylow counting theorem, let $P$ act by conjugation on the set of Sylow $3$-[subgroups](../../../group.md#subgroup). Its orbit sizes are powers of three. A fixed [subgroup](../../../group.md#subgroup) $Q$ is normalized by $P$, so $PQ$ is a [subgroup](../../../group.md#subgroup) and its order $|P||Q|/|P\cap Q|$ is a power of three. Since nine is the largest power of three dividing $72$, this forces $PQ=P=Q$. There is exactly one fixed point, namely $P$ itself. All other orbits have sizes divisible by three, giving $n_3\equiv1\pmod3$. Among $1,2,4,8$, only one and four satisfy this. Therefore **$\boxed{n_3\in\{1,4\}}$**.

## 3G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3g/solution">Solution</h3>

↑ **Parent:** [3G](#3g)

For a piecewise continuously differentiable curve $\gamma(t)=(x(t),y(t))$ in the [upper half-plane model](../../../geometry-and-topology.md#poincare-half-plane-model), the given [Riemannian metric](../../../differential-geometry.md#riemannian-metric) gives [hyperbolic length](../../../geometry-and-topology.md#hyperbolic-length-in-the-poincare-disc)

$$
\boxed{L(\gamma)=\int\frac{\sqrt{\dot x(t)^2+\dot y(t)^2}}{y(t)}\,dt.}
$$

The metric matrix has determinant $y^{-4}$, so its area element is $y^{-2}\,dx\,dy$. Thus a measurable region $D$ has [hyperbolic area](../../../geometry-and-topology.md#hyperbolic-area) $\int_Dy^{-2}\,dx\,dy$. For the specified strip the integral is

$$
\boxed{\int_0^1\int_1^\infty\frac{dy\,dx}{y^2}=1.}
$$

The infinite Euclidean height is compatible with finite [hyperbolic area](../../../geometry-and-topology.md#hyperbolic-area) because the area density decreases quadratically with height.

## 4G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4g/solution">Solution</h3>

↑ **Parent:** [4G](#4g)

[Uniform convergence](../../../real-analysis.md#uniform-convergence) means that for every $\varepsilon>0$ there is an integer $N$, independent of $x$, such that $|F_n(x)-F(x)|<\varepsilon$ for all $n\geq N$ and every $x\in(0,1)$. Equivalently $\sup_{0<x<1}|F_n(x)-F(x)|\to0$. In [pointwise convergence](../../../real-analysis.md#pointwise-convergence), the required $N$ may depend on the chosen $x$.

<h3 id="4g/i">i</h3>

↑ **Parent:** [4G](#4g)

<h4 id="4g/i/solution">Solution</h4>

↑ **Parent:** [I](#4g/i)

At every fixed $x$, $F_n(x)=e^x/n\to0$. Moreover $\sup_{0<x<1}e^x/n=e/n\to0$. Thus **the [pointwise limit](../../../real-analysis.md#pointwise-limit) is zero and convergence is uniform**.

<h3 id="4g/ii">ii</h3>

↑ **Parent:** [4G](#4g)

<h4 id="4g/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4g/ii)

For every fixed $x>0$, $nx^2\to\infty$, so the [pointwise limit](../../../real-analysis.md#pointwise-limit) is zero. But $\sup_{0<x<1}e^{-nx^2}=1$ for every $n$, since $x$ can approach zero. Hence **convergence is not uniform**. For an explicit moving-point test take $x_n=n^{-1/2}$ for $n>1$, which gives $F_n(x_n)=e^{-1}$.

<h3 id="4g/iii">iii</h3>

↑ **Parent:** [4G](#4g)

<h4 id="4g/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4g/iii)

The finite [geometric series](../../../real-analysis.md#geometric-series) gives $F_n(x)=(1-x^{n+1})/(1-x)$, so the [pointwise limit](../../../real-analysis.md#pointwise-limit) is $F(x)=1/(1-x)$. The error is $x^{n+1}/(1-x)$, unbounded as $x\uparrow1$ for every fixed $n$. Thus **convergence is not uniform on $(0,1)$**. It is uniform on any smaller interval bounded away from one, since the error is at most $b^{n+1}/(1-b)$ for $0<x\leq b<1$.

## 5A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5a/i">i</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/i/solution">Solution</h4>

↑ **Parent:** [I](#5a/i)

Factor the denominator as $z^2(1+z^2)$. Near zero,

$$
\frac1{z^2(1+z^2)}=z^{-2}-1+z^2-\cdots,
$$

so zero is a [double pole](../../../isolated-singularity.md#double-pole) with [residue](../../../analysis.md#residue) zero. At $z=\pm i$ the [poles](../../../isolated-singularity.md#pole) are simple and the denominator derivative is $2z+4z^3=-2z$. Therefore

$$
\boxed{\operatorname{Res}_{0}=0,\qquad\operatorname{Res}_{i}=\frac i2,\qquad\operatorname{Res}_{-i}=-\frac i2.}
$$

These are all the [poles](../../../isolated-singularity.md#pole).

<h3 id="5a/ii">ii</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5a/ii)

The only [pole](../../../isolated-singularity.md#pole) is the simple one at $z=1$, with **$\boxed{\operatorname{Res}_{1}=e}$**. The point $z=0$ is an [essential singularity](../../../isolated-singularity.md#essential-singularity), not another [pole](../../../isolated-singularity.md#pole): multiplying $e^{1/z^2}$ by a nonvanishing analytic factor cannot remove its infinite principal part. For completeness its [residue](../../../analysis.md#residue) can also be read from

$$
-\left(\sum_{j\geq0}z^j\right)\left(\sum_{k\geq0}\frac{z^{-2k}}{k!}\right),\qquad0<|z|<1.
$$

The coefficient of $z^{-1}$ is $-\sum_{k\geq1}1/k!=1-e$. This extra [residue](../../../analysis.md#residue) belongs to the [essential singularity](../../../isolated-singularity.md#essential-singularity); it does not change the list of [poles](../../../isolated-singularity.md#pole).

<h3 id="5a/iii">iii</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5a/iii)

The zeros of the denominator satisfy $e^z=\ell\pi$ with nonzero integer $\ell$, since an exponential never vanishes. Equivalently the [poles](../../../isolated-singularity.md#pole) are

$$
z_{m,k}=\log(m\pi)+ik\pi,\qquad m\geq1,\quad k\in\mathbb Z.
$$

At such a point $e^{z_{m,k}}=(-1)^km\pi$, and the derivative of the denominator is $e^z\cos(e^z)=(-1)^{m+k}m\pi\ne0$. All these [poles](../../../isolated-singularity.md#pole) are simple, with

$$
\boxed{\operatorname{Res}_{z_{m,k}}\frac1{\sin(e^z)}=\frac{(-1)^{m+k}}{m\pi}.}
$$

## 6B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6b/solution">Solution</h3>

↑ **Parent:** [6B](#6b)

In three dimensions, the general rank-two [isotropic tensor](../../../linear-algebra.md#isotropic-tensor) is $a\delta_{ij}$ and the general rank-three [tensor](../../../linear-algebra.md#tensor) invariant under proper rotations is $b\epsilon_{ijk}$. Here $\delta$ is the [Kronecker delta](../../../linear-algebra.md#kronecker-delta) and $\epsilon$ the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol). The latter is orientation-sensitive: an ordinary third-rank [tensor](../../../linear-algebra.md#tensor) invariant under all orthogonal transformations is zero instead. This distinction does not change the stress conclusion.

For an isotropic material, the constitutive [tensor](../../../linear-algebra.md#tensor) must consequently have $A_{ijk}=b\epsilon_{ijk}$ in the proper-rotation convention. Hence $\sigma_{ij}=b\epsilon_{ijk}B_k=-\sigma_{ji}$. Mechanical stress in the model is also symmetric, so $\sigma_{ij}=-\sigma_{ij}$ and every component vanishes. Thus **nonzero stress linear in the field requires anisotropic material coefficients**. This is the [isotropic linear magnetostriction vanishes](../../../continuum-mechanics.md#isotropic-linear-magnetostriction-vanishes) restriction, not a claim that all higher-order [magnetostriction](../../../continuum-mechanics.md#magnetostriction) is impossible in isotropic materials.

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/solution">Solution</h3>

↑ **Parent:** [7B](#7b)

In vacuum SI notation, [Maxwell's equations](../../../electromagnetism.md#maxwell-equations) are

$$
\nabla\cdot E=\rho/\epsilon_0,\quad\nabla\cdot B=0,\quad
\nabla\times E=-\partial_tB,\quad
\nabla\times B=\mu_0J+\mu_0\epsilon_0\partial_tE.
$$

Taking the [divergence](../../../calculus.md#divergence) of the last equation, using that the [divergence](../../../calculus.md#divergence) of a [curl](../../../calculus.md#curl) vanishes and then the first equation, gives

$$
0=\mu_0\nabla\cdot J+\mu_0\partial_t\rho,\qquad
\boxed{\partial_t\rho+\nabla\cdot J=0.}
$$

This is local [conservation of electric charge](../../../electromagnetism.md#charge-conservation). For spatially uniform [electrical conductivity](../../../electromagnetism.md#electrical-conductivity), [Ohm's law](../../../electromagnetism.md#ohm-s-law) $J=\sigma E$ gives $\nabla\cdot J=\sigma\rho/\epsilon_0$, so

$$
\boxed{\rho(x,t)=\rho(x,0)e^{-\sigma t/\epsilon_0},\qquad\text{decay rate }\sigma/\epsilon_0.}
$$

For a homogeneous dielectric conductor with permittivity $\epsilon$, replace $\epsilon_0$ by $\epsilon$. This [charge relaxation](../../../electromagnetism.md#charge-relaxation) is a statement about bulk charge; charge transported to a boundary is still accounted for by the conservation law.

## 8D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

For a real potential, the [Time-dependent Schrödinger equation](../../../physics.md#time-dependent-schrodinger-equation) and its [complex conjugate](../../../complex-analysis.md#complex-conjugate) give

$$
\partial_t|\psi|^2=\frac{i\hbar}{2m}(\psi^*\psi_{xx}-\psi\psi^*_{xx}).
$$

The potential terms cancel. The expression on the right is a total derivative, giving

$$
\boxed{\rho=|\psi|^2,\qquad j=\frac{\hbar}{2mi}(\psi^*\psi_x-\psi\psi_x^*)=\frac\hbar m\operatorname{Im}(\psi^*\psi_x),\qquad\rho_t+j_x=0.}
$$

For the [plane wave](../../../quantum-mechanics.md#plane-wave), $\psi_t=-i\omega\psi$ and $\psi_{xx}=-k^2\psi$. With zero potential, substitution gives

$$
\boxed{\omega(k)=\frac{\hbar k^2}{2m},\qquad\rho=1,\qquad j=\frac{\hbar k}{m}.}
$$

It is a free-particle [momentum eigenstate](../../../quantum-mechanics.md#momentum-eigenstate) with momentum $\hbar k$, [energy](../../../classical-mechanics.md#energy) $\hbar\omega$ and uniform [probability](../../../probability-theory.md#probability) flux. On the whole real line it is a generalized state, not a normalized square-integrable [wavefunction](../../../quantum-mechanics.md#wave-function); wave packets or box normalization give the corresponding physical interpretation.

## 9C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

The general [continuity equation](../../../physics.md#continuity-equation) is $\rho_t+\nabla\cdot(\rho u)=0$, or $D\rho/Dt+\rho\nabla\cdot u=0$. An [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) has $D\rho/Dt=0$, so for positive density **$\boxed{\nabla\cdot u=0}$**.

For the displayed velocity field, on $x^2+y^2>0$,

$$
\partial_x\frac{y}{x^2+y^2}=-\frac{2xy}{(x^2+y^2)^2},\qquad
\partial_y\frac{-x}{x^2+y^2}=\frac{2xy}{(x^2+y^2)^2}.
$$

The sum is zero. A [stream function](../../../fluid-mechanics.md#stream-function) with the required sign convention is

$$
\boxed{\psi(x,y)=\frac12\log(x^2+y^2)+C.}
$$

Its derivatives give exactly $u=(\psi_y,-\psi_x)$. The origin is excluded because the prescribed velocity is singular there.

## 10H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10h/solution">Solution</h3>

↑ **Parent:** [10H](#10h)

Assume independent samples $X_1,\ldots,X_n$ and $Y_1,\ldots,Y_m$, each consisting of independent [normal random variables](../../../probability-theory.md#gaussian-random-variable), with respective means $\mu_1,\mu_2$ and a common unknown [variance](../../../variance.md) $\sigma^2>0$. Take $n,m\geq2$. Normality, independence and equal variances are the assumptions giving the exact pooled [Student's t-test](../../../statistical-modelling.md#student-s-t-test); unequal variances would require a different test. We test $H_0:\mu_1=\mu_2$ against an unrestricted difference.

Put $N=n+m$ and

$$
W=\sum_i(X_i-\bar X)^2+\sum_j(Y_j-\bar Y)^2,\qquad
B=\frac{nm}{N}(\bar X-\bar Y)^2.
$$

The normal likelihood is proportional to $(\sigma^2)^{-N/2}\exp[-S/(2\sigma^2)]$, where $S$ is the residual sum of squares. Under the unrestricted model, the maximizing means are $\bar X,\bar Y$ and $S=W$. Under $H_0$, the maximizing common mean is $(n\bar X+m\bar Y)/N$ and decomposition about the [sample means](../../../variance.md#sample-mean) gives $S=W+B$. For either model, maximizing over [variance](../../../variance.md) gives $\widehat\sigma^2=S/N$. Thus the [generalized likelihood-ratio test](../../../statistical-modelling.md#generalized-likelihood-ratio-test) statistic is

$$
\Lambda=\left(\frac{W}{W+B}\right)^{N/2}
=\left(1+\frac{T^2}{N-2}\right)^{-N/2},\qquad
T=\frac{\bar X-\bar Y}{s_p\sqrt{1/n+1/m}},\quad s_p^2=\frac{W}{N-2}.
$$

Small $\Lambda$ is therefore equivalent to large $|T|$.

Under the null, $Z=(\bar X-\bar Y)/[\sigma\sqrt{1/n+1/m}]$ is standard normal. In each sample an orthogonal change of Gaussian coordinates separates the sample-mean coordinate from the centered residual coordinates; those coordinates are independent. Consequently $V=W/\sigma^2$ has a [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $N-2$ degrees of freedom and is independent of $Z$. Therefore $T=Z/\sqrt{V/(N-2)}$ has the [Student's t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution) with $N-2$ degrees of freedom. **At significance level $\alpha$, reject exactly when $\boxed{|T|>t_{N-2,1-\alpha/2}}$**, the two-sample pooled t-test.

## 11H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11h/a">a</h3>

↑ **Parent:** [11H](#11h)

<h4 id="11h/a/solution">Solution</h4>

↑ **Parent:** [A](#11h/a)

An [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) has the property that for every pair of states $i,j$ there is an integer $n\geq0$ with $(P^n)_{ij}>0$. Equivalently every state can reach every other state along a finite path of positive-[probability](../../../probability-theory.md#probability) transitions.

<h3 id="11h/b">b</h3>

↑ **Parent:** [11H](#11h)

<h4 id="11h/b/solution">Solution</h4>

↑ **Parent:** [B](#11h/b)

A [recurrent state](../../../markov-process.md#recurrent-state) $i$ satisfies $\Pr_i(T_i^+<\infty)=1$, where $T_i^+=\inf\{n\geq1:X_n=i\}$. Saying that the [transition matrix](../../../markov-process.md#stochastic-matrix) is recurrent means that every state is recurrent. In an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) it suffices that one state is recurrent, since recurrence is a communicating-class property.

<h3 id="11h/solution">Solution</h3>

↑ **Parent:** [11H](#11h)

Irreducibility and the presence of another state imply $P_{ii}<1$: otherwise $i$ would be absorbing and could not reach that other state. Hence the proposed matrix has nonnegative entries and row sums $\sum_{j\ne i}P_{ij}/(1-P_{ii})=1$.

Observe the original [Markov chain](../../../markov-process.md#markov-chain) only at times when it changes state. Starting from $i$, the next different state is $j\ne i$ with [probability](../../../probability-theory.md#probability)

$$
\sum_{r=0}^\infty P_{ii}^rP_{ij}=\frac{P_{ij}}{1-P_{ii}}.
$$

Each holding run has a finite geometric length almost surely. The [Strong Markov property](../../../markov-process.md#strong-markov-property) at the successive change times therefore identifies the observed process as the [discrete-time jump chain](../../../markov-process.md#jump-chain-of-a-discrete-time-markov-chain) with [transition matrix](../../../markov-process.md#stochastic-matrix) $\widetilde P$.

Any positive-[probability](../../../probability-theory.md#probability) path of the original chain gives a path of this new chain after repeated consecutive states are deleted. Every remaining edge has positive $\widetilde P$ [probability](../../../probability-theory.md#probability), so **$\widetilde P$ is irreducible**. For recurrence, starting at any state $i$, repeated application of the Markov property at return times shows that the original recurrent chain visits $i$ infinitely often almost surely. A single sojourn cannot account for infinitely many visits, because every sojourn is finite almost surely. There must therefore be infinitely many separate visits to $i$ in the observed chain too. Thus **$\widetilde P$ is recurrent**, proving that [recurrence survives deletion of self-transitions](../../../markov-process.md#recurrence-survives-deletion-of-self-transitions).

## 12H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12h/solution">Solution</h3>

↑ **Parent:** [12H](#12h)

Both candidate sets contain zero. The [sum of subspaces](../../../vector-space.md#sum-of-vector-subspaces) is closed under [linear combinations](../../../vector-space.md#linear-combination) because $a(u_1+w_1)+b(u_2+w_2)=(au_1+bu_2)+(aw_1+bw_2)$, with the two terms in $U$ and $W$. The intersection is closed because any [linear combination](../../../vector-space.md#linear-combination) of vectors lying in both subspaces still lies in both. Thus each is a [vector subspace](../../../vector-space.md#vector-subspace).

Take a [basis](../../../vector-space.md#basis) $s_1,\ldots,s_r$ of the intersection, extend it by $u_1,\ldots,u_a$ to a [basis](../../../vector-space.md#basis) of $U$, and by $w_1,\ldots,w_b$ to a [basis](../../../vector-space.md#basis) of $W$. The combined list $s,u,w$ spans $U+W$. To prove independence, a zero combination makes the $u$ combination equal a vector in both $U$ and $W$, so it is a combination of the $s$'s. Independence of the [basis](../../../vector-space.md#basis) of $U$ makes all $u$ coefficients zero; independence of the [basis](../../../vector-space.md#basis) of $W$ then makes all remaining coefficients zero. Hence $\dim(U+W)=r+a+b$, giving the [dimension formula for a sum of subspaces](../../../vector-space.md#dimension-formula-for-a-sum-of-subspaces)

$$
\boxed{\dim U+\dim W=\dim(U+W)+\dim(U\cap W).}
$$

For the concrete kernels, the equations $Ax=0$ give

$$
x=\left(\frac{5s-5t}{3},\frac{-s+7t}{3},s,t\right).
$$

Applying the two rows of $B$ to this expression gives $4(s-t)$ and $5(s-t)/3$. Thus the intersection has [basis](../../../vector-space.md#basis) $v_0=(0,2,1,1)$. Choose $v_1=(5,-1,3,0)$ in $U$ and $v_2=(-4,-2,1,0)$ in $W$. Then

$$
\boxed{\mathcal B_{U\cap W}=(v_0),\quad\mathcal B_U=(v_0,v_1),\quad
\mathcal B_{U+W}=(v_0,v_1,v_2).}
$$

Indeed $U$ has dimension two because $A$ has rank two, and $v_0,v_1$ are independent. Likewise $W$ has dimension two and $v_0,v_2$ are independent, so the last list spans the sum. Its first three coordinates have determinant $-48$, confirming independence and dimension three.

## 13F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13f/solution">Solution</h3>

↑ **Parent:** [13F](#13f)

The [Fundamental theorem of finitely generated abelian groups](../../../group.md#fundamental-theorem-of-finitely-generated-abelian-groups) states that every such [group](../../../group.md) is isomorphic to

$$
\mathbb Z^r\oplus\mathbb Z/d_1\mathbb Z\oplus\cdots\oplus\mathbb Z/d_s\mathbb Z,
\qquad 1<d_1\mid d_2\mid\cdots\mid d_s,
$$

with uniquely determined rank and invariant factors, allowing an empty finite part. Modulo $pA$, the free summand contributes $(\mathbb Z/p\mathbb Z)^r$. If $A/pA=0$ for some prime, this forces $r=0$, so $A$ is finite. Conversely, if $A$ is finite, choose a prime $p$ coprime to $|A|$. Bezout's identity gives an integer $b$ with $bp\equiv1\pmod{|A|}$. Since $|A|$ kills every element, multiplication by $p$ is onto, with inverse multiplication by $b$. Hence $pA=A$. This proves **$\boxed{A\text{ finite}\iff A/pA=0\text{ for some prime }p}$** under finite generation.

For the requested nonzero example use the additive [divisible group](../../../group.md#divisible-group) $A=\mathbb Q$. Each rational $q$ equals $p(q/p)$, so $p\mathbb Q=\mathbb Q$ for every prime. It is not finitely generated: a finite list of rational generators has a common denominator $D$, and every integral combination then lies in $D^{-1}\mathbb Z$. The rational $1/(2D)$ does not lie there. This proves non-finite-generation directly and shows why the hypothesis in [finite generation detected by a prime quotient](../../../group.md#finite-generation-detected-by-a-prime-quotient) is essential.

## 14G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14g/solution">Solution</h3>

↑ **Parent:** [14G](#14g)

In the [upper half-plane model](../../../geometry-and-topology.md#poincare-half-plane-model), a [hyperbolic line](../../../geometry-and-topology.md#hyperbolic-line) is either a vertical line or a Euclidean semicircle perpendicular to the real axis. For the vertical line $x=a$, set $R_L(z)=2a-\bar z$. For the circle $|z-a|=r$ with real $a$, set

$$
\boxed{R_L(z)=a+\frac{r^2}{\bar z-a}.}
$$

The vertical formula preserves $y$ and Euclidean speed. For the circular formula, $\operatorname{Im}R_L(z)=r^2\operatorname{Im}z/|z-a|^2$, while its local Euclidean length multiplier is $r^2/|z-a|^2$. Thus both preserve $|dz|/\operatorname{Im}z$, the [hyperbolic metric](../../../geometry-and-topology.md#hyperbolic-metric), and consequently all curve lengths and distances. Each is an involution preserving the half-plane; each fixes its specified line pointwise and moves points off that line. This establishes the required [hyperbolic reflection](../../../geometry-and-topology.md#hyperbolic-reflection) explicitly.

To factor an arbitrary [isometry](../../../riemannian-geometry.md#isometry) $g$, first recall why a bisector reflection exchanges any distinct points $P,Q$. The [hyperbolic distance](../../../geometry-and-topology.md#hyperbolic-distance) formula is

$$
\cosh d(x+iy,a+ib)=\frac{(x-a)^2+y^2+b^2}{2yb}.
$$

Equating the distances to $P$ and $Q$ yields a vertical line or a circle with centre on the real axis, hence a [hyperbolic line](../../../geometry-and-topology.md#hyperbolic-line). Substitution in the reflection formulas above shows that its reflection exchanges $P$ and $Q$. Choose a base point $P$. If $gP\ne P$, compose $g$ on the left with their bisector reflection, obtaining $h$ that fixes $P$; otherwise take $h=g$.

Choose $Q\ne P$. The points $hQ,Q$ have the same distance from $P$, so their bisector contains $P$. If they differ, its reflection corrects $hQ$ while retaining $P$. We obtain an [isometry](../../../riemannian-geometry.md#isometry) $k$ fixing both $P,Q$ after at most two reflections.

An [isometry](../../../riemannian-geometry.md#isometry) fixing two points is either the identity or reflection in their joining line. To see this directly, a point with prescribed distances from $P,Q$ lies at the intersection of two [hyperbolic circles](../../../geometry-and-topology.md#hyperbolic-circle); these are Euclidean circles in this model and have at most two intersections. When there are two, reflection in the line $PQ$ interchanges them. Pick a third point off that line. Either $k$ fixes it, or composing $k$ with that line reflection fixes it. An [isometry](../../../riemannian-geometry.md#isometry) fixing three noncollinear points is the identity: the first two distances leave only the reflected pair, and the distance to the third point distinguishes that pair. Thus $k$ is the identity or one additional reflection. Reversing the compositions proves **every [isometry](../../../riemannian-geometry.md#isometry) is a product of at most three [hyperbolic reflections](../../../geometry-and-topology.md#hyperbolic-reflection)**.

## 15G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15g/solution">Solution</h3>

↑ **Parent:** [15G](#15g)

A [norm](../../../functional-analysis.md#norm) $p$ is nonnegative with $p(x)=0$ exactly when $x=0$, satisfies $p(ax)=|a|p(x)$, and obeys $p(x+y)\leq p(x)+p(y)$. The [Euclidean norm](../../../functional-analysis.md#euclidean-norm) has positivity and absolute homogeneity immediately. For the [triangle inequality](../../../topological-analysis.md#triangle-inequality), positivity of $\|x-ty\|_2^2$ for all real $t$ gives the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) $|x\cdot y|\leq\|x\|_2\|y\|_2$ (with $y=0$ immediate). Hence

$$
\|x+y\|_2^2\leq\|x\|_2^2+2\|x\|_2\|y\|_2+\|y\|_2^2,
$$

which proves the [triangle inequality](../../../topological-analysis.md#triangle-inequality) after taking square roots.

For the prescribed set, use the [Minkowski functional](../../../topological-vector-space.md#minkowski-functional)

$$
\boxed{p_U(x)=\inf\{t>0:x\in tU\}.}
$$

Since $U$ is open and contains zero, some [Euclidean ball](../../../functional-analysis.md#euclidean-ball) of radius $r>0$ lies inside it. Since it is bounded, it lies inside a ball of radius $R$. These inclusions imply $\|x\|_2/R\leq p_U(x)\leq\|x\|_2/r$, so the functional is finite and positive for nonzero $x$; it is zero at zero. Symmetry gives $p_U(-x)=p_U(x)$, and substitution in the infimum gives $p_U(ax)=a p_U(x)$ for $a>0$, hence absolute homogeneity for all real scalars.

Convexity and $0\in U$ imply $sU\subseteq U$ for $0\leq s\leq1$. Consequently, for $a>p_U(x)$ and $b>p_U(y)$, one has $x/a,y/b\in U$. Convexity then gives

$$
\frac{x+y}{a+b}=\frac a{a+b}\frac xa+\frac b{a+b}\frac yb\in U,
$$

so $p_U(x+y)\leq a+b$. Letting $a\downarrow p_U(x)$ and $b\downarrow p_U(y)$ proves the [triangle inequality](../../../topological-analysis.md#triangle-inequality).

Finally, if $p_U(x)<1$, there is a $t<1$ with $x\in tU\subseteq U$. Conversely, if $x\in U$ and $x\ne0$, openness permits $(1+\delta)x\in U$ for some $\delta>0$, so $p_U(x)\leq1/(1+\delta)<1$; zero is immediate. Thus **$\boxed{U=\{x:p_U(x)<1\}}$**, completing the [norm from a bounded symmetric convex neighbourhood](../../../topological-vector-space.md#norm-from-a-bounded-symmetric-convex-neighbourhood) construction.

## 16A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16a/solution">Solution</h3>

↑ **Parent:** [16A](#16a)

Let $F(z)=p(z)/q(z)$. Its only possible finite [poles](../../../isolated-singularity.md#pole) are the distinct nonreal roots $\alpha_j$, and the [residue](../../../analysis.md#residue) of $F(z)e^{iz}$ there is $p(\alpha_j)e^{i\alpha_j}/q'(\alpha_j)$; this is zero if the numerator cancels that [pole](../../../isolated-singularity.md#pole). Close the real segment by a positively oriented semicircle in the upper half-plane, where $|e^{iz}|=e^{-\operatorname{Im}z}$ decays.

For sufficiently large radius $R$, all roots lie strictly inside or outside the contour as appropriate, and the degree bound gives $|F(z)|\leq C/R$ uniformly on the arc. Parametrizing by $z=Re^{i\theta}$ bounds the arc integral by

$$
C\int_0^\pi e^{-R\sin\theta}\,d\theta
\leq2C\int_0^{\pi/2}e^{-2R\theta/\pi}\,d\theta\leq\frac{C\pi}{R}\longrightarrow0.
$$

Here $\sin\theta\geq2\theta/\pi$ on $[0,\pi/2]$, and symmetry handles the other half. The [residue theorem](../../../analysis.md#residue-theorem) therefore gives

$$
\boxed{\int_{-\infty}^{\infty}\frac{p(x)}{q(x)}e^{ix}\,dx
=2\pi i\sum_{\operatorname{Im}\alpha_j>0}\frac{p(\alpha_j)e^{i\alpha_j}}{q'(\alpha_j)}.}
$$

To justify that this is the ordinary improper integral rather than just its symmetric principal value, note $F(x)=O(|x|^{-1})$ and $F'(x)=O(|x|^{-2})$. On either tail, [integration by parts](../../../calculus.md#integration-by-parts) writes the integral as a vanishing endpoint term $F(x)e^{ix}/i$ minus an absolutely convergent integral involving $F'$. Thus both one-sided limits exist. When the degree bound is stricter the original integral is already absolutely convergent. This proves the [Fourier integral of a rational function with simple nonreal poles](../../../analysis.md#fourier-integral-of-a-rational-function-with-simple-nonreal-poles) formula with all tail and arc limits accounted for.

## 17B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17b/solution">Solution</h3>

↑ **Parent:** [17B](#17b)

The fixed-end [wave equation](../../../wave-equation.md) has spatial modes $\sin(n\pi x)$ and temporal factors $\cos(n\pi t),\sin(n\pi t)$. The zero initial velocity removes every temporal sine term. Expand the initial displacement in a [Fourier sine series](../../../fourier-series.md#fourier-sine-series), whose coefficients are

$$
b_n=2\int_0^1x(1-x)\sin(n\pi x)\,dx
=\frac{4[1-(-1)^n]}{\pi^3n^3}.
$$

Two integrations by parts give the last equality; the endpoint terms from $x(1-x)$ vanish and the remaining derivative endpoints distinguish even from odd $n$. Consequently

$$
\boxed{y(x,t)=\frac8{\pi^3}\sum_{\substack{n\geq1\\n\text{ odd}}}\frac{\sin(n\pi x)\cos(n\pi t)}{n^3}.}
$$

This solves the initial-boundary problem in the finite-[energy](../../../classical-mechanics.md#energy) sense, with convergent first-derivative series. At $t=0$ the [energy](../../../classical-mechanics.md#energy) in the question is $\int_0^1(1-2x)^2dx=1/3$. At any time, sine/cosine [orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives the contribution of mode $n$ as $(n\pi)^2b_n^2/2$: its kinetic and elastic pieces have factors $\sin^2(n\pi t)$ and $\cos^2(n\pi t)$ summing to one. Therefore

$$
\frac13=\frac{32}{\pi^4}\sum_{\substack{n\geq1\\n\text{ odd}}}\frac1{n^4},\qquad
\boxed{\sum_{\substack{n\geq1\\n\text{ odd}}}n^{-4}=\frac{\pi^4}{96}.}
$$

The square summability of the derivative coefficients justifies the [orthogonality](../../../linear-algebra.md#orthogonal-vectors) calculation and its limit.

## 18B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18b/solution">Solution</h3>

↑ **Parent:** [18B](#18b)

Using $E=-\nabla\phi$ and the electrostatic [Poisson equation](../../../partial-differential-equation.md#poisson-equation), $\rho=-\epsilon_0\nabla^2\phi$, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
W=-\frac{\epsilon_0}{2}\int_D\phi\nabla^2\phi\,dV
=\frac{\epsilon_0}{2}\int_D|\nabla\phi|^2dV
-\frac{\epsilon_0}{2}\int_{\partial D}\phi\,\partial_n\phi\,dS.
$$

The boundary potential is zero, so the surface term vanishes. Hence **$\boxed{W=(\epsilon_0/2)\int_DE^2dV}$**.

For the [capacitor](../../../electromagnetism.md#capacitor) use the usual parallel-plate approximation, neglecting edge fields. The two gaps have widths $H+a$ and $H-a$, and their field magnitudes are $V/(H+a)$ and $V/(H-a)$. The field-[energy](../../../classical-mechanics.md#energy) expression gives

$$
\boxed{W=\frac{\epsilon_0AV^2}{2}\left(\frac1{H+a}+\frac1{H-a}\right)
=\frac{\epsilon_0AV^2H}{H^2-a^2}.}
$$

The two faces of the middle plate carry charges $Q_-=\epsilon_0AV/(H+a)$ and $Q_+=\epsilon_0AV/(H-a)$. Its total charge is their sum; the grounded plates have zero potential and contribute zero to $\frac12\sum Q_j\phi_j$. The charge-potential expression therefore gives $W=\frac12V(Q_-+Q_+)$, exactly the same result. Since $H^2-a^2$ is largest at $a=0$, **the [energy](../../../classical-mechanics.md#energy) at fixed $V$ is minimized when the middle plate is centered**, with value $\epsilon_0AV^2/H$.

This is the [electrostatic energy of a three-plate capacitor](../../../electromagnetism.md#electrostatic-energy-of-a-three-plate-capacitor) in the intended uniform-field model. Finite circular plates have fringing corrections; no small-gap-to-radius ratio is explicitly stated in the source, so the simple formula should not be described as an exact finite-disc solution.

## 19D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19d/solution">Solution</h3>

↑ **Parent:** [19D](#19d)

The [angular momentum commutation relations](../../../quantum-mechanics.md#angular-momentum-commutation-relations) are $[L_i,L_j]=i\hbar\epsilon_{ijk}L_k$. The [commutator](../../../lie-algebra.md#commutator) product rule gives

$$
[L_i,L^2]=i\hbar\sum_{j,k}\epsilon_{ijk}(L_kL_j+L_jL_k)=0,
$$

since the bracketed expression is symmetric in $j,k$ and $\epsilon_{ijk}$ is antisymmetric. Also

$$
L_-L_+=L_1^2+L_2^2+i[L_1,L_2]=L_1^2+L_2^2-\hbar L_3,
$$

proving **$\boxed{L^2=L_-L_++L_3^2+\hbar L_3}$**.

For [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum), $L_i=-i\hbar\epsilon_{ijk}x_j\partial_k$. A differentiable radial function has $\partial_kf(r)=f'(r)x_k/r$, so its contraction with the antisymmetric symbol vanishes: $Lf(r)=0$. Put $s=x_1+ix_2$. The coordinate differential operators give $L_3s=\hbar s$, while

$$
L_+=\hbar\left[x_3(\partial_1+i\partial_2)-s\partial_3\right]
$$

annihilates every power of $s$, because $(\partial_1+i\partial_2)s=0$. Since all $L_i$ annihilate the radial factor, the product rule yields

$$
\boxed{L_3[s^nf(r)]=n\hbar s^nf(r),\qquad L_+[s^nf(r)]=0.}
$$

Substitution into the expression for $L^2$ gives the [highest-weight complex-coordinate orbital wavefunction](../../../quantum-mechanics.md#highest-weight-complex-coordinate-orbital-wavefunction) result

$$
\boxed{L^2[s^nf(r)]=\hbar^2n(n+1)s^nf(r).}
$$

As $[L^2,L_-]=0$, lowering preserves this [eigenvalue](../../../linear-operator-theory.md#eigenvalue) whenever the lowered function is nonzero. Explicitly,

$$
\boxed{L_-[s^nf(r)]=-2n\hbar x_3s^{n-1}f(r),\qquad
\text{unchanged eigenvalue }\hbar^2n(n+1).}
$$

For $n=0$ the lowered function is zero, so it is not an [eigenfunction](../../../linear-operator-theory.md#eigenfunction). For $n\geq0$ the original nonzero function has the usual regular angular dependence. The PDF's “any integer” differential identities also hold locally for negative $n$ where $s\ne0$, but those negative powers are singular on the axis and are not square-integrable regular angular eigenstates. The converted TeX incorrectly writes $L_4$ in place of the PDF's $L_+$.

## 20C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="20c/solution">Solution</h3>

↑ **Parent:** [20C](#20c)

In the inviscid incompressible irrotational model, write the total velocity as $(U+\phi_x,\phi_y)$. The perturbation potential obeys [Laplace's equation](../../../partial-differential-equation.md#laplace-equation) in $-h<y<\eta(x,t)$. The complete boundary conditions, neglecting surface tension and taking the air pressure constant, are

$$
\phi_y=0\quad\text{at }y=-h,
$$



$$
\eta_t+(U+\phi_x)\eta_x=\phi_y,\qquad
\phi_t+U\phi_x+\frac12(\phi_x^2+\phi_y^2)+g\eta=0
\quad\text{at }y=\eta(x,t).
$$

The first surface condition expresses that the [free surface](../../../fluid-mechanics.md#free-surface) is material; the second is the [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) with atmospheric pressure and the constant background kinetic [energy](../../../classical-mechanics.md#energy) absorbed into the potential's time gauge.

At first order, evaluation is on $y=0$ and products of perturbations vanish. Hence

$$
\boxed{\eta_t+U\eta_x=\phi_y,\qquad\phi_t+U\phi_x+g\eta=0\quad(y=0),\qquad\phi_y=0\quad(y=-h).}
$$

For a mode $e^{i(\omega t-kx)}$, the bottom condition selects $\phi=C\cosh[k(y+h)]e^{i(\omega t-kx)}$. Let $\Omega=\omega-kU$. The linear surface conditions are

$$
i\Omega a=Ck\sinh(kh),\qquad i\Omega C\cosh(kh)+ga=0.
$$

Eliminating $C$ gives the [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{(\omega-kU)^2=gk\tanh(kh).}
$$

It is the intrinsic gravity-wave frequency squared, with the uniform current supplying the Doppler shift. For either sign of real $k$, $k\tanh(kh)$ is nonnegative.

## 21H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="21h/solution">Solution</h3>

↑ **Parent:** [21H](#21h)

The [Rao-Blackwell theorem](../../../probability-and-statistics.md#rao-blackwell-theorem) states that if an estimator $D$ has finite second moment and $T$ is a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic), then $D^*(T)=\mathbb E[D\mid T]$ can be chosen without knowing the parameter. It has the same expectation as $D$ and no larger [variance](../../../variance.md). In particular an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) remains unbiased and its squared-error risk cannot increase. Sufficiency makes the [conditional distribution](../../../probability-theory.md#conditional-distribution), hence the function of $T$ used here, parameter-independent.

The tower property gives $\mathbb E D^*=\mathbb E D$. The [law of total variance](../../../probability-theory.md#law-of-total-variance) gives

$$
\operatorname{Var}(D)=\operatorname{Var}(\mathbb E[D\mid T])+\mathbb E[\operatorname{Var}(D\mid T)],
$$

so the [variance](../../../variance.md) decreases, with equality exactly when $D$ is already a function of $T$ almost surely. Since the bias is unchanged, the same identity proves the squared-error risk claim. More generally the corresponding convex-loss inequality follows from conditional [Jensen's inequality](../../../real-analysis.md#jensen-s-inequality).

For the given [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution), the joint mass is $(1-p)^np^{\sum x_j-n}$ on positive-integer sample vectors. Thus $T=\sum_jX_j$ is a one-dimensional [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic). Directly, conditional on $T=t$, every positive-integer composition of $t$ into $n$ parts has the same [probability](../../../probability-theory.md#probability); there are $\binom{t-1}{n-1}$ such compositions, independently of $p$.

The simple estimator $D=1_{\{X_1>1\}}$ is unbiased for $p$, since $\Pr(X_1>1)=p$. For $n\geq2$, compositions with $X_1>1$ are counted by subtracting one from their first part, giving $\binom{t-2}{n-1}$ when $t>n$. Consequently the [Rao-Blackwell estimator of a geometric failure probability](../../../probability-and-statistics.md#rao-blackwell-estimator-of-a-geometric-failure-probability) is

$$
\boxed{\widehat p=\mathbb E[D\mid T]=\frac{T-n}{T-1},\qquad n\geq2.}
$$

At $T=n$ its value is zero, as it must be when all observations are one. For the possible one-observation case, use $\widehat p=1_{\{T>1\}}$; the displayed fraction would otherwise be undefined at $T=1$. The conditional-expectation argument proves unbiasedness without needing to sum the negative-binomial mass explicitly.

## 22H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="22h/solution">Solution</h3>

↑ **Parent:** [22H](#22h)

The directed positive-transition graph gives the [communicating classes](../../../markov-process.md#communicating-class) $\{1,3,6\}$, $\{2,4\}$ and $\{5\}$. **The first and last classes are closed; $\{2,4\}$ is open.** In particular the PDF's fourth row has all six entries equal to $1/6$. The converted TeX incorrectly drops the last entry; that incomplete row is not a transition distribution.

The finite irreducible closed class $C=\{1,3,6\}$ reaches state six almost surely. For example, from every state in $C$ there is a uniformly positive [probability](../../../probability-theory.md#probability) of hitting six within a bounded number of steps, so the [probability](../../../probability-theory.md#probability) of avoiding it for successive blocks tends to zero. Put $h_i=\Pr_i(T_6<\infty)$, with $h_1=h_3=h_6=1$ and $h_5=0$. First-step conditioning at states two and four gives

$$
h_2=\frac{2+h_2+h_4}{5},\qquad h_4=\frac{3+h_2+h_4}{6}.
$$

Solving $4h_2-h_4=2$ and $5h_4-h_2=3$ yields **$\boxed{h_2=13/19}$**, with $h_4=14/19$.

Starting in state three, the chain remains in $C$. In the order $(1,3,6)$ its [transition matrix](../../../markov-process.md#stochastic-matrix) is

$$
M=\begin{pmatrix}0&1/2&1/2\\1/3&1/3&1/3\\1/4&1/2&1/4\end{pmatrix}.
$$

Its characteristic polynomial is $(\lambda-1)(\lambda+1/4)(\lambda+1/6)$. Thus, by the [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem), $q_n=(M^n)_{2,3}$ is a [linear combination](../../../vector-space.md#linear-combination) of $1,(-1/4)^n,(-1/6)^n$. The initial values are $q_0=0$, $q_1=1/3$, and $q_2=(1/3)(1/2+1/3+1/4)=13/36$. Solving for the three coefficients gives

$$
\boxed{\Pr_3(X_n=6)=\frac{12}{35}+\frac45\left(-\frac14\right)^n-\frac87\left(-\frac16\right)^n,\qquad n\geq1.}
$$

The limiting value $12/35$ agrees with the state-six [probability](../../../probability-theory.md#probability) of the [stationary distribution](../../../markov-process.md#stationary-distribution) $(8/35,3/7,12/35)$ of this closed class.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
