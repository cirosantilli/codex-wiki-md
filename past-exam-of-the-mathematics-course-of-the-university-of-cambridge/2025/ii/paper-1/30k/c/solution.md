<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume first that $D=b^TV^{-1}b>0$. Since $X_M=\theta_M^TZ$,

$$
\mathbb EX_M=D,\qquad \operatorname{Var}(X_M)=D,
$$

and for $Y=\phi^TZ$,

$$
\mathbb EY=\phi^Tb,\qquad
\operatorname{Cov}(X_M,Y)=\theta_M^TV\phi=b^T\phi.
$$

The least-squares affine-regression coefficients are therefore

$$
\beta=\frac{b^T\phi}{D},\qquad
\alpha=\mathbb EY-\beta\mathbb EX_M=0.
$$

The minimum is

$$
\operatorname{Var}(Y)-\frac{\operatorname{Cov}(X_M,Y)^2}{\operatorname{Var}(X_M)}
=\phi^TQ\phi,
$$

where

$$
\boxed{Q=V-\frac{bb^T}{b^TV^{-1}b}}.
$$

This [matrix](../../../../../../matrix.md) is symmetric and positive semidefinite. If $b=0$, then $X_M=0$, one may take $\alpha=0$ and arbitrary $\beta$, and the minimum is $\phi^TV\phi$, corresponding to $Q=V$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
