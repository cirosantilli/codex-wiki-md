<h1 id="13c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With $\xi=x+ct$ and $\eta=x-ct$,

$$
\partial_x=\partial_\xi+\partial_\eta,
\qquad
\partial_t=c\partial_\xi-c\partial_\eta,
$$

so the [wave equation](../../../../../../wave-equation-split.md) becomes

$$
u_{tt}-c^2u_{xx}=-4c^2u_{\xi\eta}=0.
$$

Thus $u=F(\xi)+G(\eta)$. At $t=0$ the initial data give

$$
F(x)+G(x)=\phi(x),
\qquad
cF'(x)-cG'(x)=\psi(x).
$$

Solving for $F'$ and $G'$ and integrating gives [d'Alembert's formula](../../../../../../d-alembert-s-formula.md)\>

$$
\boxed{
u(x,t)=\frac{\phi(x+ct)+\phi(x-ct)}2
+\frac1{2c}\int_{x-ct}^{x+ct}\psi(s)\,ds }.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13C](../../13c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
