<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

A [canonical transformation](../../../../../canonical-transformation.md) is a differentiable invertible change of phase-space coordinates preserving the [symplectic form](../../../../../symplectic-form.md), equivalently the canonical [Poisson brackets](../../../../../poisson-bracket.md). At each fixed time, let $D$ be its Jacobian in the ordering $(q,p)\mapsto(Q,P)$ and put $J=\begin{pmatrix}0&I\\-I&0\end{pmatrix}$. The condition is

$$
\boxed{DJD^T=J,}
$$

which is equivalent to $D^TJD=J$. Time dependence changes the [Hamiltonian](../../../../../hamiltonian.md) by a generating-function time derivative, but not this fixed-time symplectic condition.

The [Hamilton-Jacobi equation](../../../../../hamilton-jacobi-equation.md) is $S_t+\tfrac12[(S_q)^2+\omega^2q^2]=0$. Separating $S=W(q,E)-Et$ gives $(W_q)^2=2E-\omega^2q^2$. On the positive-momentum branch, therefore,

$$
\boxed{W(q,E)=\int^q\sqrt{2E-\omega^2s^2}\,ds,\qquad S=W-Et.}
$$

Choose the integration constant so that the given angle relation is obtained. For $E>0$, $\beta=S_E$ yields $q=\sqrt{2E}\sin[\omega(t+\beta)]/\omega$, while $p=S_q=\sqrt{2E-\omega^2q^2}$ on this branch. Continuing the angle across the turning points gives the full orbit

$$
\boxed{q=\frac{\sqrt{2\alpha}}\omega\sin[\omega(t+\beta)],\qquad p=\sqrt{2\alpha}\cos[\omega(t+\beta)],\qquad\alpha=E.}
$$

The square-root expression is locally the positive branch; the cosine formula correctly changes sign on the rest of the orbit.

The generating function has differential $dS=p\,dq+\beta\,d\alpha-H\,dt$. At fixed time, taking an exterior derivative gives $dq\wedge dp=d\beta\wedge d\alpha$. Thus **the canonical new coordinate is $Q=\beta$ and its conjugate momentum is $P=\alpha$**. Directly, $\alpha=(p^2+\omega^2q^2)/2$ and $\beta=\operatorname{atan2}(\omega q,p)/\omega-t$ locally imply

$$
\beta_q=\frac p{p^2+\omega^2q^2},\qquad\beta_p=-\frac q{p^2+\omega^2q^2},\qquad\boxed{\{\beta,\alpha\}=1.}
$$

The angle is a local chart or a periodic variable, and is undefined at the zero-energy point. The source's phrase “variables $(\alpha,\beta)$” lists the new momentum before its coordinate: if interpreted instead as the conventional coordinate-then-momentum ordering, that ordered pair would have $\{\alpha,\beta\}=-1$ and be anti-canonical.

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
