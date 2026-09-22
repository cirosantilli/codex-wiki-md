<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Forward Euler method](../../../../../../euler-method.md) gives

$$
u_m^{n+1}=u_m^n
+r(u_{m-1}^n-2u_m^n+u_{m+1}^n)
+s(u_{m+1}^n-u_{m-1}^n),
$$

where

$$
r=\frac{\Delta t}{\Delta x^2},
\qquad
s=\frac{\alpha\Delta t}{2\Delta x}.
$$

Its [amplification factor](../../../../../../amplification-factor.md) is

$$
G(\vartheta)=1-4r\sin^2\frac\vartheta2
+i\frac{\alpha\Delta t}{\Delta x}\sin\vartheta.
$$

Writing $X=\sin^2(\vartheta/2)$, the condition $|G|^2\leq1$ for every $0\leq X\leq1$ is equivalent to

$$
r\leq\frac12,
\qquad
\left(\frac{\alpha\Delta t}{\Delta x}\right)^2\leq2r.
$$

Therefore

$$
\boxed{
0\leq\Delta t\leq
\min\left\{\frac{\Delta x^2}{2},\frac2{\alpha^2}\right\}
}
$$

with the second bound omitted when $\alpha=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
