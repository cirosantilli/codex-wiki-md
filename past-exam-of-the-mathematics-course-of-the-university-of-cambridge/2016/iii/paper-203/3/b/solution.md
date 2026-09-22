<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the following deterministic boundary fact from the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md). For a continuous [trace of a Loewner chain](../../../../../../trace-of-a-loewner-chain.md) started at zero and generating its hulls, the real flow at $b>0$ has a [boundary swallowing time](../../../../../../boundary-point-swallowing-time-for-a-loewner-chain.md) $T_b$. Until that time it is the reflected boundary value of $g_t$, and

$$
X_t=g_t(b)-\xi_t>0.
$$

A finite $T_b$ is its first collision with the driver, $X_t\to0$ as $t\uparrow T_b$. Topologically, the boundary point $b$ is then visited or separated from infinity precisely when the trace has reached some point in $[b,\infty)$. A boundary crosscut can swallow an interval, so this is not a claim that the trace visits the particular point $b$.

Consequently the [SLE boundary swallowing criterion](../../../../../../sle-boundary-swallowing-criterion.md) is

$$
\boxed{\{\gamma\text{ hits }[b,\infty)\}=\{T_b<\infty\}.}
$$

For the [SLE](../../../../../../schramm-loewner-evolution.md) driver this real flow obeys

$$
dX_t=\frac2{X_t}\,dt-\sqrt\kappa\,dW_t,\qquad X_0=b,
$$

up to its first hit of zero. This is the [Boundary-point Bessel flow for SLE](../../../../../../boundary-point-bessel-flow-for-sle.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
