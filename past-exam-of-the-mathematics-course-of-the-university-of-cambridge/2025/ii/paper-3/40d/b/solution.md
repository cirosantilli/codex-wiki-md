<h1 id="40d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert

$$
u_m^n=G^n e^{im\theta}
$$

into the diffusion scheme. Since

$$
e^{i\theta}-2+e^{-i\theta}
=-4\sin^2\left(\frac\theta2\right),
$$

we obtain

$$
G\left(1+2\mu\sin^2\frac\theta2\right)
=1-2\mu\sin^2\frac\theta2.
$$

Thus the [Crank-Nicolson diffusion scheme](../../../../../../crank-nicolson-diffusion-scheme.md) has

$$
G(\theta)=
\frac{1-2\mu\sin^2(\theta/2)}
{1+2\mu\sin^2(\theta/2)}.
$$

For $\mu\geq0$, the denominator is positive and

$$
|1-2\mu s|\leq1+2\mu s
\qquad(0\leq s\leq1).
$$

Hence

$$
\boxed{\text{the method is stable for every }\mu>0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40D](../../40d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
