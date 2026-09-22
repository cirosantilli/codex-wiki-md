<h1 id="33a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Lax's equation](../../../../../../isospectral-lax-equation.md) in the convention used here is

$$
\boxed{\dot{\mathcal L}=[\mathcal L,\mathcal A]
=\mathcal L\mathcal A-\mathcal A\mathcal L.}
$$

Let $\mathcal L\psi=\lambda\psi$ with $(\psi,\psi)=1$. Since $\mathcal L$ is [self-adjoint](../../../../../../self-adjoint-operator.md) and $\mathcal A$ is [anti-self-adjoint](../../../../../../skew-adjoint-generator.md), differentiating $\lambda=(\psi,\mathcal L\psi)$ gives

$$
\dot\lambda
=(\dot\psi,\mathcal L\psi)
+(\psi,\dot{\mathcal L}\psi)
+(\psi,\mathcal L\dot\psi).
$$

The first and third terms equal $\lambda,d(\psi,\psi)/dt=0$. For the middle term,

$$
(\psi,[\mathcal L,\mathcal A]\psi)
=(\mathcal L\psi,\mathcal A\psi)
-(\psi,\mathcal A\mathcal L\psi)=0.
$$

Thus $\dot\lambda=0$, proving the [Isospectral Lax equation](../../../../../../isospectral-lax-equation.md) property: **every eigenvalue is independent of $t$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [33A](../../33a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
