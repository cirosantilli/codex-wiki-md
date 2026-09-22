<h1 id="18c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a steady flow independent of $y$, [geostrophic balance](../../../../../../geostrophic-balance.md) gives

$$
u=0,
\qquad
v=\frac gf\frac{d\eta}{dx}.
$$

Hence $\zeta=v_x=(g/f)\eta''$, and the definition of $q$ becomes

$$
q=\frac gf\eta''-\frac fh\eta.
$$

Equivalently,

$$
\boxed{\eta''-\frac{f^2}{gh}\eta=\frac fgq}.
$$

With the [Rossby deformation radius](../../../../../../rossby-deformation-radius.md) $R=\sqrt{gh}/f$, the bounded solution for the stated potential-vorticity step is

$$
\eta(x)=
\begin{cases}
-\dfrac{hq_1}{f}+A e^{x/R},&x<0,\\
-\dfrac{hq_2}{f}+B e^{-x/R},&x>0.
\end{cases}
$$

Continuity of $\eta$ and $v=(g/f)\eta'$ at $x=0$ gives

$$
A=\frac{h(q_1-q_2)}{2f},
\qquad
B=-\frac{h(q_1-q_2)}{2f}.
$$

Therefore

$$
\boxed{
\eta(x)=
\begin{cases}
-\dfrac{hq_1}{f}+\dfrac{h(q_1-q_2)}{2f}e^{x/R},&x<0,\\
-\dfrac{hq_2}{f}-\dfrac{h(q_1-q_2)}{2f}e^{-x/R},&x>0,
\end{cases}}
$$

and

$$
\boxed{v(x)=\frac{R(q_1-q_2)}2e^{-|x|/R}}.
$$

When $q_1>q_2$, the surface height increases smoothly from $-hq_1/f$ to $-hq_2/f$, while $v$ is a positive eastward jet with its maximum at the discontinuity and [exponential decay](../../../../../../exponential-decay.md) on the Rossby-radius scale:

<a id="18c/c/image-free-surface-and-jet-for-a-potential-vorticity-step"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4-potential-vorticity-step.png)

**[Figure 2](#18c/c/image-free-surface-and-jet-for-a-potential-vorticity-step). Free surface and jet for a potential-vorticity step**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18C](../../18c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
