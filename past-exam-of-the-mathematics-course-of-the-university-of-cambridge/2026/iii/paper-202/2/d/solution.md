<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put

$$
f_n(x)=\frac1n\log\cosh(nx).
$$

Then $f_n\to|\mathord\cdot|$ uniformly, $f_n'(x)=\tanh(nx)$, and $f_n''(x)=n\operatorname{sech}^2(nx)$. [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
f_n(X_t)=f_n(X_0)+\int_0^t\tanh(nX_s)\,dX_s
+\frac12\int_0^t n\operatorname{sech}^2(nX_s)\,d[X]_s.
$$

The bounded predictable integrands $\tanh(nX)$ converge pointwise to $\operatorname{sgn}(X)$, with $\operatorname{sgn}(0)=0$. Part (c) therefore makes the stochastic integrals converge u.c.p. The left-hand side converges u.c.p. to $|X|$, so the increasing continuous processes

$$
A_t^{(n)}=\frac12\int_0^t n\operatorname{sech}^2(nX_s)\,d[X]_s
$$

also converge u.c.p. Their limit $A$ has a continuous increasing version: extract almost-sure locally uniform convergence from each compact interval and use a diagonal argument. We obtain

$$
|X_t|=|X_0|+\int_0^t\operatorname{sgn}(X_s)\,dX_s+A_t,
$$

the [Tanaka formula](../../../../../../tanaka-s-formula.md) with $A=L_t^0(X)$. It expresses $|X|$ as a continuous local martingale plus a continuous finite-variation process, so $|X|$ is a continuous semimartingale.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
