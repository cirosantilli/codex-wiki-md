<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For any observable $f$, the [Markov jump-process generator](../../../../../../../markov-jump-process-generator.md) identity gives

$$
\frac d{dt}\langle f\rangle=\langle\mathcal Lf\rangle.
$$

Set $m(t)=\langle x_2\rangle$ and $s(t)=\langle x_2^2\rangle$. With $\alpha_7=0$, reaction 2 changes $x_2$ by $+1$ and reaction 3 changes it by $-1$. Therefore

$$
\boxed{\dot m=\alpha_2\langle x_1\rangle-\alpha_3\langle x_2^2\rangle}
$$

and, using $(x_2+1)^2-x_2^2=2x_2+1$ and $(x_2-1)^2-x_2^2=-2x_2+1$,

$$
\boxed{\dot s
=\alpha_2\left(2\langle x_1x_2\rangle+\langle x_1\rangle\right)
-2\alpha_3\langle x_2^3\rangle
+\alpha_3\langle x_2^2\rangle.}
$$

The equation for the second [moment](../../../../../../../moment.md) contains the third, whose equation contains the fourth, and so on. This is an infinite [moment hierarchy](../../../../../../../moment-hierarchy.md).

Reaction 1 eventually leaves the odd initial copy number at $x_1^*=1$. Put

$$
\mu=\langle x_2^*\rangle,\qquad
q=\frac{\alpha_2}{\alpha_3}.
$$

The stationary first-moment equation gives

$$
\langle(x_2^*)^2\rangle=q.
$$

The stationary second-moment equation then gives

$$
\langle(x_2^*)^3\rangle=q(\mu+1).
$$

Under the prescribed [central-moment closure](../../../../../../../central-moment-closure.md),

$$
0=\left\langle(x_2^*-\mu)^3\right\rangle
=\langle(x_2^*)^3\rangle
-3\mu\langle(x_2^*)^2\rangle+2\mu^3.
$$

Substitution yields the requested [polynomial equation](../../../../../../../polynomial-equation.md)

$$
\boxed{2\mu^3-2\frac{\alpha_2}{\alpha_3}\mu
+\frac{\alpha_2}{\alpha_3}=0.}
$$

This cubic comes from the closure approximation; it is not an exact equation for the stationary mean.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 356](../../../../paper-356-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
