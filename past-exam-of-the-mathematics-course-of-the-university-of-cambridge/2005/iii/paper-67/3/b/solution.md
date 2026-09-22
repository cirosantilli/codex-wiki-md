<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix counterclockwise arclength on each side and take the outward [normal derivative](../../../../../../normal-derivative.md). Write

$$
h=\frac l{2\sqrt3},\qquad z^{(j)}(s)=c_j(h+is),\qquad
(c_1,c_2,c_3)=(1,\bar a,a),\quad a=e^{2\pi i/3}.
$$

The unit tangent is $ic_j$ and the outward unit normal is $c_j$. On side $j$ this gives the chain-rule identity

$$
i c_jq_z=\frac12q_s^{(j)}+\frac i2q_N^{(j)}.
$$

Put $w=c_jk$. The exponential in the [closed differential one-form](../../../../../../closed-differential-one-form.md) pulls back to

$$
W(z^{(j)}(s),k)=E(-iw)e^{(w+\lambda/w)s},\qquad
\boxed{E(k)=\exp\left[\frac l{2\sqrt3}\left(k+\frac\lambda k\right)\right].}
$$

Also $-\lambda q\,d\bar z/(ik)=(\lambda/w)q^{(j)}ds$. Consequently the contribution of side $j$ is $\rho_j(c_jk)$, where the required local side spectra are

$$
\boxed{\begin{aligned}
\Psi_j(k)&=\int_{-l/2}^{l/2}e^{(k+\lambda/k)s}q_N^{(j)}(s)ds,\\
\Phi_j(k)&=\int_{-l/2}^{l/2}e^{(k+\lambda/k)s}
\left[\frac12q_s^{(j)}(s)+\frac\lambda kq^{(j)}(s)\right]ds,\\
\rho_j(k)&=E(-ik)\left[\frac i2\Psi_j(k)+\Phi_j(k)\right].
\end{aligned}}
$$

These are spectral [integral transforms](../../../../../../integral-transform.md) in the local coordinate of each side. Keeping the tangential-derivative term is important: premature [integration by parts](../../../../../../integration-by-parts.md) in a single side integral would leave corner values, which cannot simply be discarded. At the special samples used below, those endpoint terms do vanish for the rotationally invariant solution.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
