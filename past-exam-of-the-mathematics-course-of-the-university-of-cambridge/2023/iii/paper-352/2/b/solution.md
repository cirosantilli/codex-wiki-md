<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The convected terms are quadratic in the disturbance. Linear response requires small strain and small rate-based Weissenberg numbers, in particular

$$
\frac{\dot\gamma_0}{\omega}\ll1,
\qquad
\lambda_1\dot\gamma_0\ll1,
\qquad
\lambda_2\dot\gamma_0\ll1.
$$

The constitutive equation then reduces to

$$
\tau+\lambda_1\dot\tau
=\eta(\dot\gamma+\lambda_2\ddot\gamma).
$$

For $\dot\gamma=\dot\gamma_0\cos\omega t$, its periodic stress response is

$$
\tau(t)=\frac{\eta\dot\gamma_0}{1+\omega^2\lambda_1^2}
\left[
(1+\omega^2\lambda_1\lambda_2)\cos\omega t
+\omega(\lambda_1-\lambda_2)\sin\omega t
\right].
$$

Since $\gamma=(\dot\gamma_0/\omega)\sin\omega t$, comparison with $\tau=\gamma_0[G'\sin\omega t+G''\cos\omega t]$ gives

$$
\boxed{G'(\omega)=
\frac{\eta\omega^2(\lambda_1-\lambda_2)}{1+\omega^2\lambda_1^2},
\qquad
G''(\omega)=
\frac{\eta\omega(1+\omega^2\lambda_1\lambda_2)}{1+\omega^2\lambda_1^2}.}
$$

The condition $\lambda_1\geq\lambda_2$ makes the storage modulus nonnegative.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
