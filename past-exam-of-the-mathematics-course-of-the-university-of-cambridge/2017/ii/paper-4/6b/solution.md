<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

At an [endemic equilibrium](../../../../../endemic-equilibrium.md), $I_*>0$, so $\beta S_*=\mu+\nu$. Substitution into the susceptible equation gives

$$
\boxed{S_*=\frac N{R_0},\qquad I_*=\frac{\mu N}{\mu+\nu}\left(1-\frac1{R_0}\right).}
$$

These values are physically positive exactly when $R_0>1$. The [Jacobian matrix](../../../../../jacobian-matrix.md) at this equilibrium is

$$
J=\begin{pmatrix}-\mu R_0&-(\mu+\nu)\\\mu(R_0-1)&0\end{pmatrix},\qquad
\operatorname{tr}J=-\mu R_0<0,\quad\det J=\mu(\mu+\nu)(R_0-1)>0.
$$

Both [eigenvalues](../../../../../eigenvalue.md) have negative real parts, so the [endemic equilibrium](../../../../../endemic-equilibrium.md) is locally asymptotically stable. Its decay exponents are

$$
\lambda_\pm=-\frac{\mu R_0}{2}\pm\sqrt{\frac{\mu^2R_0^2}{4}-\mu(\mu+\nu)(R_0-1)}.
$$

The regime $\nu\gg\mu$ means recovery is rapid compared with demographic replacement. For fixed $R_0>1$ away from the threshold, the exponents form a [complex conjugate](../../../../../complex-conjugate.md) pair with frequency approximately $\sqrt{\mu\nu(R_0-1)}$. Hence

$$
\boxed{T\simeq\frac{2\pi}{\sqrt{\mu\nu(R_0-1)}}.}
$$

Strictly, oscillations require $\mu(\mu+\nu)(R_0-1)>\mu^2R_0^2/4$; $\nu\gg\mu$ alone does not ensure this uniformly for every $R_0$ arbitrarily close to one or arbitrarily large.

Vaccinating a fraction $v$ of newborns replaces the susceptible input by $\mu N(1-v)$. The effective [basic reproduction number](../../../../../basic-reproduction-number.md) is $R_v=(1-v)R_0$, and the same calculation replaces $R_0$ by $R_v$. Provided $R_v>1$ and the oscillatory approximation remains applicable, **vaccination lengthens the [oscillation period](../../../../../period-of-an-oscillation.md)**, because $R_v-1$ is smaller. Extremely near eradication the exponents become real and there is no [oscillation period](../../../../../period-of-an-oscillation.md) to extrapolate indefinitely.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
