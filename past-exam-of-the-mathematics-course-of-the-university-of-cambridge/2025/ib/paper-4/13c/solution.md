<h1 id="13c/solution">Solution</h1>

↑ **Parent:** [13C](../13c.md)

The Euler--Lagrange equation is

$$
2ma^2(1-\cos\phi)\ddot\phi+ma^2\sin\phi\,\dot\phi^2-mga\sin\phi=0.
$$

Putting $u=\cos(\phi/2)$ and simplifying gives

$$
\ddot u+\omega^2u=0,\qquad \omega^2=\frac{g}{4a}.
$$

Since $1-\cos\phi=2(1-u^2)$, $1+\cos\phi=2u^2$, and $\dot u^2=(1-u^2)\dot\phi^2/4$, the transformed functional is

$$
\widehat S[u]=\int_0^T(8ma^2\dot u^2-2mga u^2)dt.
$$

Its Euler--Lagrange equation is $\ddot u+(g/4a)u=0$, exactly the preceding equation.

For endpoint-vanishing $\eta$, the [second variation](../../../../../second-variation.md) is

$$
\delta^2\widehat S(\eta)=16ma^2\int_0^T(\dot\eta^2-\omega^2\eta^2)dt.
$$

Writing $\eta=\sum_{n\geq1}c_ne_n$ and using orthonormality gives

$$
\delta^2\widehat S=16ma^2\sum_{n\geq1}\left[\left(\frac{n\pi}{T}\right)^2-\omega^2\right]c_n^2.
$$

It is positive definite when $T<\pi/\omega$ and has a negative $e_1$ direction when $T>\pi/\omega$. Therefore

$$
\boxed{t_0=\frac\pi\omega=2\pi\sqrt{\frac ag}.}
$$

## ↑ Ancestors (10)

1. [13C](../13c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
