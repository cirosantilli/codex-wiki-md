<h1 id="1/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After separating the conserved horizontal factor as $\psi=e^{ipx}f(z)$, the [Helmholtz equation](../../../../../../../helmholtz-equation.md) becomes

$$
f''+q_0^2f=-\alpha q_0^2H(-z)f,
$$

where $H$ is the [Heaviside step function](../../../../../../../heaviside-step-function.md). The outgoing [Green function](../../../../../../../green-s-function.md) for $d^2/dz^2+q_0^2$ is

$$
G(z,z')=\frac{e^{iq_0|z-z'|}}{2iq_0}.
$$

The [Born approximation](../../../../../../../born-approximation.md) at first order replaces $f$ on the right-hand side by the incident profile $f_i(z')=e^{-iq_0z'}$. For $z>0$ this gives

$$
f_{s,B}(z)
=-\alpha q_0^2\int_{-\infty}^{0}
\frac{e^{iq_0(z-z')}}{2iq_0}e^{-iq_0z'}\,dz'.
$$

The integral is understood with the usual outgoing-wave convergence factor. Since

$$
\int_{-\infty}^{0}e^{-2iq_0z'}\,dz'=-\frac{1}{2iq_0},
$$

we obtain

$$
f_{s,B}(z)=-\frac{\alpha}{4}e^{iq_0z}.
$$

Therefore the Born reflected field is

$$
\boxed{\psi_{r,B}(x,z)=-\frac{\alpha}{4}e^{i(px+q_0z)}}.
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [1](../../../1.md)
4. [Paper 335](../../../../paper-335-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
