<h1 id="14d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose ordered particle angles $q_1,q_2,q_3$ with

$$
\alpha=q_2-q_1,\qquad
\beta=q_3-q_2,\qquad
\gamma=2\pi-\alpha-\beta,
$$

and put $\Phi=(q_1+q_2+q_3)/3$. Solving for the individual angles gives

$$
q_1=\Phi-\frac{2\alpha+\beta}{3},\qquad
q_2=\Phi+\frac{\alpha-\beta}{3},\qquad
q_3=\Phi+\frac{\alpha+2\beta}{3}.
$$

The [kinetic energy](../../../../../../kinetic-energy.md) is therefore

$$
T=\frac{mr^2}{2}\sum_{j=1}^3\dot q_j^2
=\frac{3mr^2}{2}\dot\Phi^2
+\frac{mr^2}{3}
 \left(\dot\alpha^2+\dot\alpha\dot\beta+\dot\beta^2\right).
$$

The collective angle is an [ignorable coordinate](../../../../../../ignorable-coordinate.md) and decouples from the gaps, so its term may be omitted from the relative [Lagrangian](../../../../../../lagrangian-mechanics.md). Substituting $\gamma=2\pi-\alpha-\beta$ into the [potential energy](../../../../../../potential-energy.md) gives

$$
\boxed{
L_{\rm rel}
=\frac{mr^2}{3}
 \left(\dot\alpha^2+\dot\alpha\dot\beta+\dot\beta^2\right)
-V_0\left(
e^{-2\alpha}+e^{-2\beta}+e^{-4\pi+2\alpha+2\beta}
\right).
}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14D](../../14d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
