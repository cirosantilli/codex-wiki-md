<h1 id="37d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In coordinates $x^\mu$, write the type-$(1,1)$ tensor as

$$
T=T^\mu{}_{\nu}\,
\partial_\mu\otimes dx^\nu.
$$

For a covector $\eta=\eta_\mu dx^\mu$ and vector $V=V^\nu\partial_\nu$,

$$
T(\eta,V)=T^\mu{}_{\nu}\eta_\mu V^\nu.
$$

Since this must equal $\eta(V)=\eta_\nu V^\nu$ for every $\eta$ and $V$, the components are

$$
\boxed{T^\mu{}_{\nu}=\delta^\mu{}_{\nu}}.
$$

Thus $T$ is the [identity tensor](../../../../../../identity-tensor.md).

The [tensor component transformation law](../../../../../../tensor-component-transformation-law.md) gives

$$
\begin{aligned}
T^{\mu'}{}_{\nu'}
&=\frac{\partial x^{\mu'}}{\partial x^\alpha}
\frac{\partial x^\beta}{\partial x^{\nu'}}
T^\alpha{}_{\beta}\\
&=\frac{\partial x^{\mu'}}{\partial x^\alpha}
\frac{\partial x^\alpha}{\partial x^{\nu'}}\\
&=\delta^{\mu'}{}_{\nu'}.
\end{aligned}
$$

The components are therefore the same [Kronecker delta](../../../../../../kronecker-delta.md) in every coordinate system.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [37D](../../37d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
