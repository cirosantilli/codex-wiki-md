<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $A$ for the population [matrix](../../../../matrix.md) and assume $\Lambda_1,\Lambda_2>0$. Its [characteristic polynomial](../../../../characteristic-polynomial.md) is

$$
\det(sI-A)=(s+\Lambda_1)(s+\Lambda_2)-2\Lambda_1\Lambda_2
=s^2+(\Lambda_1+\Lambda_2)s-\Lambda_1\Lambda_2.
$$

The two [eigenvalues](../../../../eigenvalue.md) have opposite signs. The [dominant eigenvalue](../../../../dominant-eigenvalue.md) is

$$
\boxed{\mu=\frac{\sqrt{\Lambda_1^2+6\Lambda_1\Lambda_2+\Lambda_2^2}-\Lambda_1-\Lambda_2}{2}>0,}
$$

and the other [eigenvalue](../../../../eigenvalue.md) is $\nu=-(\Lambda_1+\Lambda_2)-\mu<0$. A positive [eigenvector](../../../../eigenvector.md) for $\mu$ satisfies

$$
\boxed{\frac{N_2}{N_1}\longrightarrow\frac{\Lambda_1}{\mu+\Lambda_2}
=\frac{\mu+\Lambda_1}{2\Lambda_2}.}
$$

For any nonzero nonnegative population vector in this constant-coefficient system, the coefficient of the positive [eigenvector](../../../../eigenvector.md) is positive: a positive left [eigenvector](../../../../eigenvector.md) annihilates the other [eigenvector](../../../../eigenvector.md) and has positive pairing with that population vector. Thus $N_i(t)=C_i e^{\mu t}+O(e^{\nu t})$, with $C_i>0$, and $N_i'/N_i\to\mu$. The long-time leading term therefore obeys $N_i'=\mu N_i$.

Substituting that exponential mode into the [age-structured population equation](../../../../age-structured-population-equation.md) gives

$$
f_i'(\tau)=-[\mu+\Gamma_i(\tau)]f_i(\tau).
$$

Define the phase-residence [survival function](../../../../survival-function.md) and its discounted integral by

$$
S_i(\tau)=\exp\left[-\int_0^\tau\Gamma_i(a)\,da\right],\qquad
Z_i(\mu)=\int_0^\infty e^{-\mu a}S_i(a)\,da.
$$

Then the normalized [cell-cycle age densities](../../../../cell-cycle-age-density.md) are

$$
\boxed{f_i(\tau)=\frac{e^{-\mu\tau}S_i(\tau)}{Z_i(\mu)},\qquad i=1,2.}
$$

Since [integration](../../../../integral-split.md) of $f_i'=-(\mu+\Gamma_i)f_i$ gives $f_i(0)=\mu+\Lambda_i$, this is equivalently

$$
\boxed{f_i(\tau)=(\mu+\Lambda_i)\exp\left[-\mu\tau-\int_0^\tau\Gamma_i(a)\,da\right].}
$$

The constants must be consistent with both incoming [fluxes](../../../../flux.md). Put

$$
H_i(\mu)=\int_0^\infty\Gamma_i(a)e^{-\mu a}S_i(a)\,da
=1-\mu Z_i(\mu).
$$

The [boundary conditions](../../../../boundary-condition.md) for amplitudes $n_i=e^{\mu t}\phi_i$ give $\phi_1(0)=2H_2\phi_2(0)$ and $\phi_2(0)=H_1\phi_1(0)$. Hence the [Two-stage Euler-Lotka equation](../../../../two-stage-euler-lotka-equation.md) is

$$
\boxed{2H_1(\mu)H_2(\mu)=1.}
$$

It determines $\mu$ directly from the [hazard functions](../../../../hazard-function.md); the formula in terms of $\Lambda_i$ is not permission to choose those constants independently of the profiles. If each phase is eventually left with probability one, $H_i(0)=1$ and $H_i(\mu)$ decreases to zero, giving a unique positive root under the usual finite, non-instantaneous residence-time assumptions. More generally positive growth requires $2H_1(0)H_2(0)>1$. Nonnegative [hazard functions](../../../../hazard-function.md) alone do not ensure it: if one phase has zero exit [hazard function](../../../../hazard-function.md), growth cannot have the asserted positive exponent. Convergence of the complete age distribution to these profiles needs the usual mixing assumptions on phase-residence times; the two-dimensional [eigenvalue](../../../../eigenvalue.md) calculation establishes the long-time claim for the fixed-profile system.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further mathematical biology course of the University of Oxford](../../../split.md)
5. [Further mathematical biology course of the University of Oxford](../../../../further-mathematical-biology-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
