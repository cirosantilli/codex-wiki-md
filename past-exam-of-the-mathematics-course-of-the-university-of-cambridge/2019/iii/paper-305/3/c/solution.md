<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Fierz rearrangement](../../../../../../fierz-identity.md) puts the charged-current operator in the same current ordering as the neutral-current operator. Accounting for the interchange of fermionic fields, the combined amplitude is

$$
\mathcal M=\frac{G_F}{\sqrt2}
[\bar u(k')\gamma^\alpha(1-\gamma^5)u(k)]
[\bar u(p')\gamma_\alpha(C_V-C_A\gamma^5)u(p)],
\qquad C_V=c_V+1,\quad C_A=c_A+1.
$$

Sum over final spins and average over the initial electron spin. The [fermion spin sum](../../../../../../fermion-spin-sum.md) and [gamma-matrix trace](../../../../../../gamma-matrix-trace.md) identities give

$$
\overline{|\mathcal M|^2}
=4G_F^2\left[(C_V+C_A)^2s^2+(C_V-C_A)^2u^2\right].
$$

For massless two-body scattering in the [centre-of-momentum frame](../../../../../../center-of-momentum-frame.md), $d\sigma/dt=\overline{|\mathcal M|^2}/(16\pi s^2)$ and $u=-s-t$. Integrating $-s\leq t\leq0$ therefore yields

$$
\begin{aligned}
\sigma
&=\frac{G_F^2s}{4\pi}\left[(c_V+c_A+2)^2+\frac13(c_V-c_A)^2\right]\\
&=\boxed{\frac{G_F^2s}{3\pi}\left(c_V^2+c_A^2+c_Vc_A+3c_V+3c_A+3\right)}.
\end{aligned}
$$

Consequently

$$
\boxed{H(s)=\frac{s}{3\pi},\qquad B=1,\quad C=1,\quad D=3,\quad E=3,\quad F=3.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
