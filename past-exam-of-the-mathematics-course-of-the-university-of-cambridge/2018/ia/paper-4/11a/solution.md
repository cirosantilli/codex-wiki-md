<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

The [Lorentz force law](../../../../../lorentz-force.md) is $\mathbf F=q(\mathbf E+\mathbf v\times\mathbf B)$. Before impact the acceleration toward the wall is $a=qE/m$, so the first-impact speed is **$v_0=\sqrt{2qEh/m}$**.

After the $n$th bounce, the outward speed is $\gamma^nv_0$, so the outward height is $\gamma^{2n}h$ and that excursion contributes twice this distance. Hence

$$
L=h+2h\sum_{n\geq1}\gamma^{2n}
=\boxed{h\frac{1+\gamma^2}{1-\gamma^2}},
$$

so $q_1(\gamma)=1+\gamma^2$ and $q_2(\gamma)=1-\gamma^2$.

With quadratic drag, put $w=-\dot z\geq0$. Then

$$
m\dot w=qE-\alpha w^2,\qquad w(0)=0,
$$

whose solution is $w=\sqrt{qE/\alpha}\tanh(\sqrt{\alpha qE}\,t/m)$. Integration gives

$$
\boxed{z(t)=h-\frac m\alpha\log\cosh\left(\frac{\sqrt{\alpha qE}}m\,t\right).}
$$

Thus $A=m/\alpha$, $B=\sqrt{\alpha qE}/m$, and $f(s)=\log\cosh s$.

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
