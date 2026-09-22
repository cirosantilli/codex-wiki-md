<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [multiplication of a distribution by a smooth function](../../../../../../multiplication-of-a-distribution-by-a-smooth-function.md) is $\langle\psi T,\varphi\rangle=\langle T,\psi\varphi\rangle$. If $\psi$ is a [Schwartz function](../../../../../../schwartz-function.md), the [Leibniz rule](../../../../../../leibniz-rule.md) shows that $\varphi\mapsto\psi\varphi$ is a continuous map $\mathcal S\to\mathcal S$, so $\psi T$ is a [tempered distribution](../../../../../../tempered-distribution.md). When both $\psi$ and $T$ are radial, $\psi\circ R^t=\psi$, and

$$
\langle(\psi T)\circ R,\varphi\rangle
=\langle T,\psi(\varphi\circ R^t)\rangle
=\langle T,(\psi\varphi)\circ R^t\rangle
=\langle T,\psi\varphi\rangle.
$$

Thus **Multiplication by a radial [Schwartz function](../../../../../../schwartz-function.md) preserves [radial tempered distributions](../../../../../../radial-tempered-distribution.md)**.

For the [convolution of a tempered distribution with a Schwartz function](../../../../../../convolution-of-a-tempered-distribution-with-a-schwartz-function.md), set

$$
(T*\psi)(x)=\langle T_y,\psi(x-y)\rangle.
$$

Translations of $\psi$ depend smoothly on $x$ in the [Schwartz space](../../../../../../schwartz-space.md), so this is a [smooth function](../../../../../../smooth-function.md) with $\partial^\alpha(T*\psi)(x)=\langle T_y,\partial^\alpha\psi(x-y)\rangle$. The bound for $T$ by finitely many [seminorms](../../../../../../seminorm.md), together with $1+|y|\leq(1+|x|)(1+|x-y|)$, proves

$$
|\partial^\alpha(T*\psi)(x)|\leq C_\alpha(1+|x|)^m.
$$

Thus the function also defines a [tempered distribution](../../../../../../tempered-distribution.md). For a [radial function](../../../../../../radial-function.md) $\psi$, put $g_x(y)=\psi(x-y)$. Then $\psi(Rx-y)=\psi(x-R^ty)=g_x(R^ty)$, so

$$
(T*\psi)(Rx)=\langle T,g_x\circ R^t\rangle
=\langle T\circ R,g_x\rangle=(T*\psi)(x).
$$

Hence **[Convolution](../../../../../../convolution.md) with a radial [Schwartz function](../../../../../../schwartz-function.md) preserves [radial tempered distributions](../../../../../../radial-tempered-distribution.md)**.

Smoothing alone need not give a [Schwartz function](../../../../../../schwartz-function.md): for the constant [tempered distribution](../../../../../../tempered-distribution.md) $T=1$ and a [Schwartz function](../../../../../../schwartz-function.md) with integral one, $T*\psi=1$. The [radial Schwartz approximation of tempered distributions](../../../../../../radial-schwartz-approximation-of-tempered-distributions.md) therefore combines smoothing with a large-radius cutoff. Choose a nonnegative radial [mollifier](../../../../../../mollifier.md) $\rho\in C_c^\infty$, supported in the unit ball with integral one, and a radial [cutoff function](../../../../../../cutoff-function.md) $\chi\in C_c^\infty$ equal to one on the unit ball. Put

$$
\rho_\varepsilon(x)=\varepsilon^{-n}\rho(x/\varepsilon),\qquad
\chi_j(x)=\chi(x/j),\qquad
\boxed{f_j(x)=\chi_j(x)(T*\rho_{1/j})(x).}
$$

Each $f_j$ is a [smooth function](../../../../../../smooth-function.md) of [compact support](../../../../../../compact-support.md), hence a [Schwartz function](../../../../../../schwartz-function.md), and the two invariance calculations above make it radial.

It remains to prove convergence, including the simultaneous changes of both scales. With $\check\rho(x)=\rho(-x)$, the distributional [convolution](../../../../../../convolution.md) pairing is

$$
\langle f_j,\varphi\rangle
=\left\langle T,\check\rho_{1/j}*(\chi_j\varphi)\right\rangle.
$$

For every fixed $m$, the [Leibniz rule](../../../../../../leibniz-rule.md), rapid decay outside the radius-$j$ ball, and the [chain rule](../../../../../../chain-rule.md) for $\chi(x/j)$ give

$$
q_m((\chi_j-1)\varphi)\leq \frac{C_m}{j}q_{m+1}(\varphi).
$$

Convolution by $\check\rho_\varepsilon$ is uniformly bounded in $q_m$ for $0<\varepsilon\leq1$, because its shifts have size at most one. The [mean value theorem](../../../../../../mean-value-theorem.md) applied to $\varphi(x-y)-\varphi(x)$ similarly gives

$$
q_m(\check\rho_\varepsilon*\varphi-\varphi)\leq C_m\varepsilon q_{m+1}(\varphi).
$$

Splitting the error into the convolved cutoff error and the [approximate identity](../../../../../../approximate-identity.md) error proves

$$
q_m\!\left(\check\rho_{1/j}*(\chi_j\varphi)-\varphi\right)
\leq \frac{C_m'}j q_{m+1}(\varphi).
$$

If $|\langle T,\theta\rangle|\leq Cq_m(\theta)$, this yields

$$
|\langle f_j-T,\varphi\rangle|\leq \frac{C''}j q_{m+1}(\varphi).
$$

Consequently

$$
\boxed{f_j\longrightarrow T\quad\text{in }\mathcal S'}
$$

weakly, and even in the [strong dual topology](../../../../../../strong-dual-topology.md), since $q_{m+1}$ is uniformly bounded on every subset of the [Schwartz space](../../../../../../schwartz-space.md) that is a [bounded set in a topological vector space](../../../../../../bounded-set-in-a-topological-vector-space.md). No assertion that $T*\rho_{1/j}$ itself is rapidly decreasing is needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
