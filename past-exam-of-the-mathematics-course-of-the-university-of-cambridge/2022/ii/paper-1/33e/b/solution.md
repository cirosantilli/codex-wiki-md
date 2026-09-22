<h1 id="33e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiating the first auxiliary equation in $t$, the second in $x$, and equating $\psi_{xt}$ and $\psi_{tx}$ leaves precisely

$$
q_t+q_{xxx}=0,
$$

so the [Airy equation](../../../../../../airy-equation.md) is their [compatibility condition](../../../../../../compatibility-condition-for-an-overdetermined-linear-system.md).

Multiplication of $\psi_x-ik\psi=q$ by $e^{-ikx}$ gives

$$
(e^{-ikx}\psi)_x=e^{-ikx}q.
$$

Hence

$$
\psi_+(x,t,k)=e^{ikx}\int_{-\infty}^{x}e^{-iky}q(y,t)\,dy.
$$

For $\operatorname{Im}k\geq0$, the kernel $e^{ik(x-y)}$ is bounded when $y\leq x$; dominated differentiation makes $\psi_+$ analytic for $\operatorname{Im}k>0$. Rapid decrease gives

$$
\lim_{x\to+\infty}e^{-ikx}\psi_+(x,t,k)=\widehat q(k,t).
$$

For real $k$, multiply the time equation by $e^{-ikx}$ and let $x\to+\infty$. The rapidly decreasing terms on its right vanish, leaving

$$
\widehat q_t-ik^3\widehat q=0.
$$

Therefore

$$
\widehat q(k,t)=e^{ik^3t}\widehat q(k,0),
$$

and the [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) gives

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}
e^{i(kx+k^3t)}\widehat q(k,0)\,dk}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [33E](../../33e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
