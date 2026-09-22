<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [density operators](../../../../../../density-matrix.md) are Hermitian, so their squared [Hilbert-Schmidt distance](../../../../../../hilbert-schmidt-distance.md) is $2V=\operatorname{Tr}(\rho^2)+\operatorname{Tr}(\rho_d^2)-2\operatorname{Tr}(\rho\rho_d)$. Both [purity of a density operator](../../../../../../purity-of-a-density-operator.md) values are constant under their respective [unitary time evolution](../../../../../../unitary-time-evolution.md): cyclicity gives $\operatorname{Tr}(\rho[H,\rho])=0$ for every Hermitian $H$. Consequently

$$
\dot V=-\operatorname{Tr}(\dot\rho\rho_d)-\operatorname{Tr}(\rho\dot\rho_d)=-f\operatorname{Tr}\bigl(\rho_d[-iH_1,\rho]\bigr).
$$

The terms containing $H_0$ cancel because $\operatorname{Tr}([-iH_0,\rho]\rho_d)=-\operatorname{Tr}(\rho[-iH_0,\rho_d])$. The quantity $F=\operatorname{Tr}(\rho_d[-iH_1,\rho])$ is real: $[-iH_1,\rho]$ is Hermitian, and the [trace](../../../../../../matrix-trace.md) of the product of two [Hermitian matrices](../../../../../../hermitian-operator.md) equals its conjugate. The [Lyapunov quantum control](../../../../../../lyapunov-quantum-control.md) choice $f=F$ therefore gives $\boxed{\dot V=-f^2\le0}$. For $t_2\ge t_1$, integration yields $V(t_2)=V(t_1)-\int_{t_1}^{t_2}f(t)^2\,dt\le V(t_1)$. Since the distance is $\sqrt{2V}$, it is **monotonically nonincreasing**. The decrease need not be strict when $f=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
