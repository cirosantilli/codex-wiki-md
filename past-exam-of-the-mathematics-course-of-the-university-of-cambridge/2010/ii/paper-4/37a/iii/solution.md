<h1 id="37a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Divide the two outer boundary equations respectively by $z$ and leave the derivative equation as written:

$$
A/z^2+B+Cz+Dz^3=0,\qquad
-A/z^2+B+2Cz+4Dz^3=0.
$$

Their difference gives $Cz+3Dz^3=2A/z^2$. As $z\to\infty$, the inner equations require $A,B\to1/4$. The two outer equations at leading order thus give $Cz+Dz^3=-1/4$ and $Cz+3Dz^3=0$, so

$$
C=-\frac3{8z}+O(z^{-2}),\qquad
D=\frac1{8z^3}+O(z^{-4}).
$$

The inner equations also give $A+B=1/2-C-D$ and $B-A=-2C-4D$. Solving and substituting yields

$$
\boxed{A=\frac14-\frac3{16z}+O(z^{-2}),\quad
B=\frac14+\frac9{16z}+O(z^{-2}),\quad
C\sim-\frac3{8z},\quad D\sim\frac1{8z^3}.}
$$

Replacing $z$ by $b/a$ gives all four requested approximations.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [37A](../../37a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
