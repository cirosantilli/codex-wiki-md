<h1 id="14b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For zero products, put $A=k_1+k'_1+k_2$ and

$$
\lambda_\pm=\frac12\left(A\pm\sqrt{A^2-4k_1k_2}\right).
$$

The initial conditions are $E_0(0)=1$ and $C_0(0)=0$. Eliminating $E_0$ gives

$$
\ddot C_0+A\dot C_0+k_1k_2C_0=0,
\qquad \dot C_0(0)=k_1.
$$

Therefore

$$
C_0(t)=\frac{k_1}{\lambda_+-\lambda_-}
\left(e^{-\lambda_-t}-e^{-\lambda_+t}\right),
$$

and using $E_0=(\dot C_0+(k'_1+k_2)C_0)/k_1$ gives

$$
\boxed{E_0(t)=\frac{(k'_1+k_2-\lambda_-)e^{-\lambda_-t}
-(k'_1+k_2-\lambda_+)e^{-\lambda_+t}}
{\lambda_+-\lambda_-}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14B](../../14b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
