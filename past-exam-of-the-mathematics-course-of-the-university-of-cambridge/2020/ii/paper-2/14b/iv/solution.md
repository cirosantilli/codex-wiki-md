<h1 id="14b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $L_z=L_3(1-\epsilon^2/2)$ and seek $\theta=O(\epsilon)$. Using $\cos\theta=1-\theta^2/2+O(\theta^4)$ and $\sin^2\theta=\theta^2+O(\theta^4)$, the $\theta$-dependent part of the effective potential is

$$
V_{\mathrm{eff}}(\theta)
=\text{constant}
+\frac{L_3^2-4MglI_1}{8I_1}\theta^2
+\frac{L_3^2\epsilon^4}{8I_1\theta^2}
+O(\epsilon^4).
$$

It has a local minimum precisely when

$$
\boxed{L_3^2>4MglI_1},
$$

which is the [gyroscopic stabilization of an inverted symmetric top](../../../../../../gyroscopic-stabilization-of-an-inverted-symmetric-top.md) condition. Differentiating the displayed approximation gives

$$
\theta_{\mathrm{eq}}^4
=\frac{L_3^2\epsilon^4}{L_3^2-4MglI_1},
$$

and hence

$$
\boxed{\theta_{\mathrm{eq}}
=\epsilon\left(\frac{L_3^2}{L_3^2-4MglI_1}\right)^{1/4}}.
$$

Taking $L_3>0$ without loss of orientation, the steady [precession](../../../../../../precession.md) rate is

$$
\dot\phi
=\frac{L_z-L_3\cos\theta_{\mathrm{eq}}}
{I_1\sin^2\theta_{\mathrm{eq}}}
=\frac{L_3}{2I_1}
\left(1-\frac{\epsilon^2}{\theta_{\mathrm{eq}}^2}\right)+O(\epsilon^2),
$$

so

$$
\boxed{\dot\phi
=\frac{L_3-\sqrt{L_3^2-4MglI_1}}{2I_1}
+O(\epsilon^2)}.
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [14B](../../14b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
