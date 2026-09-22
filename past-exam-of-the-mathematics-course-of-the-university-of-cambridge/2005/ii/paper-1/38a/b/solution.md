<h1 id="38a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the Fourier mode $u_m^n=g^ne^{im\xi}$, substitution gives

$$
\left(1-\frac{i\mu}2\sin\xi\right)g=1+\frac{i\mu}2\sin\xi,\qquad \boxed{g=\frac{1+i\mu\sin\xi/2}{1-i\mu\sin\xi/2}.}
$$

The denominator is never zero for real $\mu,\xi$, and numerator and denominator are complex conjugates, so $|g|=1$. Parseval's identity therefore makes each step norm-preserving on square-summable grid data. **The method is von Neumann stable for every $\mu>0$**, with no upper Courant restriction. It is an implicit nondissipative scheme; unconditional [stability](../../../../../../stability-of-a-numerical-method.md) does not remove phase error or guarantee accuracy at a large time step.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38A](../../38a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
