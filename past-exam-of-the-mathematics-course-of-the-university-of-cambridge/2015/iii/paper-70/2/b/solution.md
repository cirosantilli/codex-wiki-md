<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) applied to $e^{-ikz}q_z$ yields the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md)

$$
G_1(k)+G_2(k)+G_3(k)=0.
$$

Initially this follows for $\operatorname{Im}k\leq0$, where the far vertical closing segment vanishes. The identities below can be compared on the real axis, and then continued wherever the respective transforms are analytic.

Define the characteristic factor of the [symmetric Robin strip transform](../../../../../../symmetric-robin-strip-transform.md)

$$
D(k)=(k-\gamma)-(k+\gamma)e^{k\ell}.
$$

Substituting part (a) into the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) gives

$$
\phi(k)=iD(k)\psi(-ik)-iH(k)-\frac c2(1-e^{k\ell}).
$$

Reflection symmetry gives $H(-k)=e^{-k\ell}H(k)$ and $\phi(-k)=-e^{-k\ell}\phi(k)$, because $q_y(0,\ell-y)=-q_y(0,y)$. Also $D(-k)=e^{-k\ell}D(k)$. Use the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) at $-k$ and multiply by $-e^{k\ell}$ to obtain

$$
\phi(k)=-iD(k)\psi(ik)+iH(k)-\frac c2(1-e^{k\ell}).
$$

Comparison therefore proves

$$
\boxed{\psi(-ik)=\frac{2H(k)}{D(k)}-\psi(ik),\qquad\phi(k)=iH(k)-iD(k)\psi(ik)-\frac c2(1-e^{k\ell}).}
$$

At a zero of $D$, this identity is interpreted through the necessary solvability condition and a removable limit when a decaying solution exists. For $\gamma>0$, $D$ has no real zeros, so no such qualification is needed on the two real integration rays.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
