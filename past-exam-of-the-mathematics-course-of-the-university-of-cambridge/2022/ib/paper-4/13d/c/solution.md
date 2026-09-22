<h1 id="13d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The Euler-Lagrange equation is

$$
y^{(4)}-2y''-y=0.
$$

Put $A=\sqrt{1+\sqrt2}$, $B=\sqrt{\sqrt2-1}$, and $L=\pi/2$. The conditions at zero reduce the general solution to

$$
y=C(\cosh Ax-\cos Bx)
+D\left(\sinh Ax-\frac AB\sin Bx\right).
$$

Define

$$
U=\cosh(AL)-\cos(BL),
\quad V=\sinh(AL)-\frac AB\sin(BL),
$$



$$
U'=A\sinh(AL)+B\sin(BL),
\quad V'=A(\cosh(AL)-\cos(BL)).
$$

The remaining boundary conditions give

$$
\boxed{C=\frac{LV'-V}{UV'-U'V},
\qquad D=\frac{U-LU'}{UV'-U'V}},
$$

which determines the unique extremal explicitly.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13D](../../13d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
