<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For real $\alpha,\beta$, the equilibrium equations are $-\beta^2x-\alpha z=0$, $y=0$ and $\alpha x-(\beta^2+1)z=\beta$. The determinant of the coefficient matrix is $-D$, where $D=\alpha^2+\beta^2(\beta^2+1)>0$ whenever $(\alpha,\beta)\ne(0,0)$. Solving the two-by-two system, including cases with one parameter zero, gives

$$
\boxed{s_*=(x_*,y_*,z_*)^T=\frac1D(\alpha\beta,0,-\beta^3)^T}.
$$

Substitution verifies the first equation by cancellation of $-\alpha\beta^3$ and $+\alpha\beta^3$, and the third because $\alpha^2\beta+\beta^3(\beta^2+1)=\beta D$. The nonzero determinant proves uniqueness. Its squared length is $\beta^2(\alpha^2+\beta^4)/D^2$, and

$$
D^2-4\beta^2(\alpha^2+\beta^4)=(\alpha^2+\beta^4-\beta^2)^2\ge0.
$$

Thus $\|s_*\|\le1/2$, which is inside the qubit physical [Bloch vector](../../../../../../bloch-vector.md) body; in the Hilbert-Schmidt normalization of part (b), that body has radius $1/\sqrt2$.

The $y$ mode has eigenvalue $-1$. The $xz$ block has characteristic polynomial $(\lambda+\beta^2)(\lambda+\beta^2+1)+\alpha^2$, so the other eigenvalues are

$$
\boxed{\lambda_\pm=-\beta^2-\frac12\pm\sqrt{\frac14-\alpha^2}}.
$$

If $|\alpha|>1/2$, they have real part $-\beta^2-1/2<0$. If $|\alpha|\le1/2$, the square root is at most $1/2$, with equality only when $\alpha=0$; the larger eigenvalue is still negative unless $\alpha=\beta=0$. At $|\alpha|=1/2$ an eventual Jordan factor does not change decay because its eigenvalue is negative. Therefore for every allowed parameter pair all eigenvalues have negative real part, and $\boxed{s_*\text{ is globally attractive}}$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
